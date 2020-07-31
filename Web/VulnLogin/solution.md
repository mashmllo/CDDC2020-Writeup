# VulnLogin

## Description 

This is not how you log someone in! <br> 
http://vulnlogin.chall.cddc2020.nshc.sg:8090/ <br>
Note: <br> 
Flag format is CDDC20{username_password}

## Solution 

When visiting the website, a login page is shown. By viewing the source code of the webpage, credentials are provided in login.js. 
![credentials in hash](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/VulnLogin/login_creds.jpg)
Since the hardcoded credentials are in hash, a [hash decrypter](https://hashes.com/en/decrypt/hash) is used to retrieve the credentials. 
![cracked](https://github.com/mashmllo/CDDC2020-Writeup/blob/master/Web/VulnLogin/flag_login.jpg)

## Flag

CDDC20{administrator_password12345678}
