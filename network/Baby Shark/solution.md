# Baby Shark 

## Description

Recently the Resistance Fighters have discovered this new thing called Wireshark, it seems to be some kind of tool used for analysing network packets.
We tried to capture a little snippet of traffic while browsing the web just to check out its capabilities. Let’s check out what it can do.
MD5(“easy.pcap”): aa16be8f7032586d5bfc675e9ac8e982

## Attached files 

## Solution
By viewing the pcap file given, it is noted that files are being transferred through http traffic. Thus, by exporting all the http files via the Export HTTP Object feature in WireShark, 
the files that are being transferred through HTTP traffic.
<br> To export the files, go to ```Files > Export Objects > HTTP``` <br>
<insert img> 
Using the searhch function, we are able to locate the flag in the files. 
<insert img>
