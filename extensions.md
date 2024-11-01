***extensions***

![image](https://github.com/user-attachments/assets/084d06c9-c061-4e6c-ace5-bd05f5f9c176)

Ý tưởng bài này là khi tôi kiểm tra định dạng file txt thì tôi thấy file có định dạng PNG.

```linux
nart@LAPTOP-4KTO77CJ:~$ xxd flag.txt | head
00000000: 8950 4e47 0d0a 1a0a 0000 000d 4948 4452  .PNG........IHDR
00000010: 0000 06a1 0000 0260 0802 0000 0085 ad5e  .......`.......^
00000020: 9a00 0000 0173 5247 4200 aece 1ce9 0000  .....sRGB.......
00000030: 0004 6741 4d41 0000 b18f 0bfc 6105 0000  ..gAMA......a...
00000040: 0009 7048 5973 0000 1625 0000 1625 0149  ..pHYs...%...%.I
00000050: 5224 f000 0026 9549 4441 5478 5eed dd6b  R$...&.IDATx^..k
00000060: 421b 39b7 05d0 3b2e 0694 f130 9a4c 2683  B.9...;....0.L&.
00000070: f9ae 5f80 4e3d 25bb 4cb3 f15a bfba a14a  .._.N=%.L..Z...J
00000080: 7574 2413 7927 c0ff fd0f 0000 0000 4826  ut$.y'........H&
00000090: e303 0000 0080 6c32 3e00 0000 00c8 26e3  ......l2>.....&.
```

Vậy chỉ cần đổi tên và xem hình xem sao.

<img width="849" alt="flag" src="https://github.com/user-attachments/assets/aeb97587-e241-439a-b10f-1d86a9de3f88">

flag : ```picoCTF{now_you_know_about_extensions}```
