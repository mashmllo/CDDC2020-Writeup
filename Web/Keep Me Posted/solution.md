# Keep Me Posted 

## Description 

Some weird page. Looks fishy. Please help. <br>
http://keepmeposted.chall.cddc2020.nshc.sg:1057/

## Solution 

When visiting the website, a message ``` Who are you? Post me a letter and I might let you in heh```.  <br>
![webpage](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/Keep%20Me%20Posted/keep%20me%20posted/webpage.jpg) <br>
Using postman, the request is changed from ```GET``` to ```POST```. <br>
![response](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/Keep%20Me%20Posted/keep%20me%20posted/header.jpg) <br>
By looking at the response header, it is shown that the value of the authorization header is encoded in base64. Using a base64 decoder, it is shown that the string is ```No```. 
Thus, by encoding ```Yes``` into base64 and replace the value of the authorization header, the flag is shown.  <br>
![flag](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/Keep%20Me%20Posted/keep%20me%20posted/flag.jpg)


## Flag 

CDDC20{YEs5SS_1_4m_aUTh0r1z3DDdD}
