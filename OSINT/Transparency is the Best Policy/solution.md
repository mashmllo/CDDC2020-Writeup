# Transparency is the Best Policy

## Description 

The website looks state-of-the-art. As expected of a evil mega conglomerate. <br>
Okay, they’re using HTTPS certificate, very secure. Is there any way we can discover what other domains they are hosting? <br>
Note: <br>
This challenge does not require brute-forcing. There is no need to do so.

## Solution 

Using a [subdomain finder](https://subdomainfinder.c99.nl/), 3 domains were found. 
![subdomain](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/OSINT/Transparency%20is%20the%20Best%20Policy/subdomain.jpg) <br>
By going to the ```flag``` subdomain, the flag is found. <br>
![flag](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/OSINT/Transparency%20is%20the%20Best%20Policy/flag_subdomain.jpg)

## Flag
 CDDC20{CERT_TR4SP4RENCY}
