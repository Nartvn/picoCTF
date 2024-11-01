***Verify***

![image](https://github.com/user-attachments/assets/1757572e-d620-406a-9207-1e08874ad0b5)

Khi tải file về chúng ta được 1 file nén giải nén ra và theo đường dẫn ```\\wsl.localhost\Ubuntu\home\nart\home\ctf-player\drop-in```. 
Chúng ta sẽ có 3 file:

```linux
nart@LAPTOP-4KTO77CJ:~/home/ctf-player/drop-in$ ls
checksum.txt  decrypt.sh  files
```
Chúng ta sẽ xem file ```checksum.txt``` trong đó có

```cat checksum.txt
b09c99c555e2b39a7e97849181e8996bc6a62501f0149c32447d8e65e205d6d2```

Lệnh ```sha256sum``` có thể được sử dụng trên một tệp để lấy tổng kiểm tra.

```linux
sha256sum files/* | grep b09c99c555e2b39a7e97849181e8996bc6a62501f0149c32447d8e65e205d6d2
b09c99c555e2b39a7e97849181e8996bc6a62501f0149c32447d8e65e205d6d2  files/451fd69b
```
dùng lệnh sau để tìm lá cờ trong opensll data.

```linux
nart@LAPTOP-4KTO77CJ:~/home/ctf-player/drop-in$ openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -salt -in files/451fd69
b -k picoCTF
picoCTF{trust_but_verify_451fd69b}
```

flag : ```picoCTF{trust_but_verify_451fd69b}```
