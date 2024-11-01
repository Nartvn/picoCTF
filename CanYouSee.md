***CanYouSee***

![image](https://github.com/user-attachments/assets/0da04009-3515-4ceb-b58f-ea2010e31c57)

tài về tôi được file ảnh như sau:

![image](https://github.com/user-attachments/assets/b94294d5-0a2e-4289-87d1-28939b7d0400)

Coi bằng hex editor tôi được 1 hướng giải.

![image](https://github.com/user-attachments/assets/ffffada0-f803-46af-b08e-7c0548c47682)

dùng ExifTool tôi được.

```linux
nart@LAPTOP-4KTO77CJ:~$ exiftool ukn_reality.jpg
ExifTool Version Number         : 12.76
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.3 MB
File Modification Date/Time     : 2024:03:12 07:05:57+07:00
File Access Date/Time           : 2024:11:01 15:13:28+07:00
File Inode Change Date/Time     : 2024:11:01 15:12:58+07:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fZDhjMzgxZmR9Cg==
Image Width                     : 4308
Image Height                    : 2875
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 4308x2875
Megapixels                      : 12.4
```
ta có đoạn base64 ```cGljb0NURntNRTc0RDQ3QV9ISUREM05fZDhjMzgxZmR9Cg==```, bây h chỉ việc decode nó.

![image](https://github.com/user-attachments/assets/d1a39924-5ab8-45ed-9d04-0641a351c565)

flag : ```picoCTF{ME74D47A_HIDD3N_d8c381fd}```
