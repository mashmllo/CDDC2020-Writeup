# Description 
What kind of lousy photographer takes terrible pictures like these?
MD5(“img.jpg”): 4bdba9f047cb651b3645cfe6a41666ba
# Attached file 

# Solution 
When the image was opened, it was just a black picture with no content. Exiftools is then used next to determine if there is anything hidden in the metadata. 
````
ExifTool Version Number         : 11.92
File Name                       : img.jpg
Directory                       : .
File Size                       : 1517 kB
File Modification Date/Time     : 2020:07:03 17:37:22+08:00
File Access Date/Time           : 2020:07:11 15:34:12+08:00
File Inode Change Date/Time     : 2020:07:03 17:37:27+08:00
File Permissions                : rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
Exif Byte Order                 : Big-endian (Motorola, MM)
Image Description               : WOOO_MY_AWESOME_PHOTO
Orientation                     : Horizontal (normal)
X Resolution                    : 72
Y Resolution                    : 72
Resolution Unit                 : inches
Modify Date                     : 2019:11:04 13:57:06
Artist                          : me myself and i
Y Cb Cr Positioning             : Centered
Exposure Time                   : 1/17
F Number                        : 1.7
Date/Time Original              : 2019:11:04 13:57:06
Create Date                     : 2019:11:04 13:57:06
Components Configuration        : Y, Cb, Cr, -
Shutter Speed Value             : 1/17
Aperture Value                  : 1.7
Brightness Value                : 3
Focal Length                    : 4.1 mm
Sub Sec Time                    : 509944
Sub Sec Time Original           : 509944
Sub Sec Time Digitized          : 509944
Flashpix Version                : 0100
Color Space                     : sRGB
Exif Image Width                : 2592
Exif Image Height               : 4608
Sensing Method                  : One-chip color area
Scene Type                      : Directly photographed
Exposure Mode                   : Auto
Offset Schema                   : 4216
XP Title                        : WOOO_MY_AWESOME_PHOTO
XP Comment                      : 02CDDC{yhp4rg07ohp_5i_EmOs3wa}
XP Author                       : me myself and i
XP Keywords                     : heheh;:)
XP Subject                      : I wonder if anyone will find this hmm
Padding                         : (Binary data 1980 bytes, use -b option to extract)
Compression                     : JPEG (old-style)
Make                            : OnePlus
Camera Model Name               : ONEPLUS A5000
Thumbnail Offset                : 5366
Thumbnail Length                : 1350
XMP Toolkit                     : Adobe XMP Core 5.1.0-jc003
Capture Mode                    : Photo
Scene                           : AutoHDR
Is HDR Active                   : False
Is Night Mode Active            : False
Lens Facing                     : Back
Subject                         : heheh, :)
Creator                         : me myself and i
Title                           : WOOO_MY_AWESOME_PHOTO
Description                     : WOOO_MY_AWESOME_PHOTO
Warning                         : [minor] Fixed incorrect URI for xmlns:MicrosoftPhoto
Last Keyword XMP                : heheh, :)
Image Width                     : 2592
Image Height                    : 4608
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Aperture                        : 1.7
Image Size                      : 2592x4608
Megapixels                      : 11.9
Shutter Speed                   : 1/17
Create Date                     : 2019:11:04 13:57:06.509944
Date/Time Original              : 2019:11:04 13:57:06.509944
Modify Date                     : 2019:11:04 13:57:06.509944
Thumbnail Image                 : (Binary data 1350 bytes, use -b option to extract)
Focal Length                    : 4.1 mm
````
Indeed, there is a text that looks like the flag but it is mirrored. By flipping the text, we got the flag. 
````
02CDDC{yhp4rg07ohp_5i_EmOs3wa} - > CDDC20{pho70gr4phy_i5_aw3sOmE}
````
