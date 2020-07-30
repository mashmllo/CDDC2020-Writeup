# Mama Shark

## Description 


We have received a new packet for analysis.
Oh damn, there’s too much more traffic to look through.. Is there a shortcut to find what we’re looking for immediately?
MD5(“noisy.pcap”): dabae618e77eb2532d1215700deaffdc

## Attachment 

## Solution 

By viewing the pcap file given, it is noted that files are being transferred through http traffic. Thus, by exporting all the http files via the Export HTTP Object feature in WireShark, the files that are being transferred through HTTP traffic. 
To export the files, go to ```Files > Export Objects > HTTP```
<insert img>
Using the search function, we are able to locate the flag in the files.
<insert img>
  
## Flag 
CDDC20{JUST_GIVE_ME_TL:DR}
