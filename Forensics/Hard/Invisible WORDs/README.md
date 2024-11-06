# **[Invisible WORDs](https://play.picoctf.org/practice/challenge/354)**

Bài này tôi phải nhờ hướng dân của gg mới làm được ấy :33 
đọc đề thôi:

![image](https://hackmd.io/_uploads/rJldDSag1e.png)

Khi tải về thì tôi được 1 file khá màu mè, theo những thao tác cơ bản như trên mà làm tôi không thu được bất cứ gì.
Theo hướng dân thì tui nhìn vô nó có cấu trúc giống file zip nếu tách ra 2 2. Nên tôi tách nó ra bằng lệnh python sau:

```
g=open("output.zip","wb")
with open("output.bmp","rb") as f:
   hdr=f.read(0x8a)
   skip=f.read(2)
   while skip:
      keep=f.read(2)
      g.write(keep)
      skip=f.read(2)
g.close()
```
Chúng ta sẽ được file out.zip và giờ chỉ cần binwalk nó ra.

![image](https://hackmd.io/_uploads/r1QnBIxbkl.png)

Truy cập vào thì nó có những file như sau:

![image](https://hackmd.io/_uploads/HkolI8lWkl.png)

Việc cần làm bây giờ là kiếm tra file lạ đó và thật may mắn khi chung ta đã có được flag.

![image](https://hackmd.io/_uploads/SkSQUIeWkx.png)

flag : picoCTF{w0rd_d4wg_y0u_f0und_5h3113ys_m4573rp13c3_c2cdf0f5}
