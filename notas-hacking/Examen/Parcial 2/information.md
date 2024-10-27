# Solucion
Descargar el archivo y ejecutar 
```
┌──(kali㉿kali)-[~/Downloads]
└─$ exiftool cat.jpg                                                             
ExifTool Version Number         : 12.76
File Name                       : cat.jpg
Directory                       : .
File Size                       : 878 kB
File Modification Date/Time     : 2024:10:26 22:43:19-04:00
File Access Date/Time           : 2024:10:26 22:43:18-04:00
File Inode Change Date/Time     : 2024:10:26 22:43:19-04:00
File Permissions                : -rw-rw-r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.02
Resolution Unit                 : None
X Resolution                    : 1
Y Resolution                    : 1
Current IPTC Digest             : 7a78f3d9cfb1ce42ab5a3aa30573d617
Copyright Notice                : PicoCTF
Application Record Version      : 4
XMP Toolkit                     : Image::ExifTool 10.80
License                         : cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9
Rights                          : PicoCTF
Image Width                     : 2560
Image Height                    : 1598
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 2560x1598
Megapixels                      : 4.1
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ exiftool cat.jpg | grep License | sed -e 's/.*: //' | base64 -d
picoCTF{the_m3tadata_1s_modified}                                                                                                                                                                                                   

```
