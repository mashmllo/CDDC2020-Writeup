# MD5 hash of the file 
5f76953e753ffd56eae5532d63b7a391
# Attached file 
[analyze.pcap](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/attachment/network/analyse.pcap)
# Solution 
Using WireShark, it can be determined there was a FTP connection and users are transferring files. A particular file, secret.bin stands out. The file was then retrieved. 
Steps on how to retrive the FTP file can be found [here](https://unit42.paloaltonetworks.com/using-wireshark-exporting-objects-from-a-pcap/).
![ftp connection](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/network/Something%20Goes%20On/ftp%20connections.jpg)
When the file is opened using cat in a linux machine, it looks as though the file is encrypted. 
<br>
Further investigation in the network transaction shows that the User-agent of the http request is not the usual User-agent such as Firefox or Google but [struts-pwn](https://github.com/mazen160/struts-pwn_CVE-2018-11776).
![http request]https://github.com/mashmllo/CDDC2020-Writeup/blob/master/network/Something%20Goes%20On/http%20request%20.jpg)
Research is done on this exploit and it is found that this exploit has a remote code execution. The document can be found [here](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2018-11776).
Upon further investigation on the TCP transaction, it is shown that the attacker has compromised the machine and is a root user. Thus, we start to follow the TCP stream and found a pair of SSH keys 
![TCP Stream](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/network/Something%20Goes%20On/follow%20stream.jpg)
After copying out the SSH private key and using the Openssl command in linux, we got the flag.
```openssl rsautl -decrypt -inkey priv.pem -in secret.bin -out flag.txt```
