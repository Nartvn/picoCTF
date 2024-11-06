# **[tunn3l v1s10n](ht[tps://](https://play.picoctf.org/practice/challenge/112))**
Thì đề bài như này nè :33 

![image](https://hackmd.io/_uploads/H1ELoVTe1g.png)

Thì đầu tiên chúng ta phải tải file về ...
Làm như tuần tự mở Ubuntu lên, kiểm tra nó là gì.

![image](https://hackmd.io/_uploads/rJMmhE6e1e.png)

Và nó là file data nên tôi sẽ kiểm tra từng bước:
* Đầu tiên là xem trong file gốc có key đặc biệt không (không gì cả).
    
![image](https://hackmd.io/_uploads/rJz9nVTx1g.png)

* Tiếp theo là đến base64, hex,...

Và khi tôi mở bằng xxd lên thì tui thấy file là định dạng BMP.

![image](https://hackmd.io/_uploads/rJwdpNal1l.png)

Giờ thì đổi đuôi của nó xem thu được gì nào?

![image](https://hackmd.io/_uploads/rJ8kRN6lke.png)

Yeah như đã đoán trước nó đã bị lỗi rồi :<<
Không sao bây giờ tôi sẽ mở trình soạn văn bản lên và bắt đầu sửa nó :+1: 
Vì đây là lần đầu tôi tiếp cận với nó nên tui đã lên [đây](https://en.wikipedia.org/wiki/BMP_file_format) tham khảo 1 ít dữ liệu để có thể hoàn thành được bài này.

![image](https://hackmd.io/_uploads/ryP3ANagkg.png)

Nhìn quanh thì mọi thứ có vẻ ổn cho tới khi tôi lưới tới từ BAD mà bài tập vô tình để đó cho tôi biết :astonished: 
Nếu đã biết sai ở đầu thì lao vào fix thôi

![image](https://hackmd.io/_uploads/H1jNkSagkg.png)

WIKI để để rất rõ format file như nào và canh cứ vào vị trí tôi đã sữa nó lại nhứ thế này:

![image](https://hackmd.io/_uploads/HyRqyHpl1l.png)

Khi đã chỉnh lại như vậy thì file ảnh đã mở được tôi liền vào coi, nhưng mà nó không phải kết quả như tôi muốn (không có flag).

![image](https://hackmd.io/_uploads/Byk-gHaeyg.png)

Nhìn vào tôi và bạn đều thấy hình ảnh không hoàn chỉnh nghĩa là nó cần to hơn nên tôi sẽ tăng thêm chiều cao và rộng của ảnh.
Có vẻ khi tôi điều chỉnh chiều rộng thì ảnh của tôi đã bị vỡ nên tui sẽ chỉnh theo chiều cao.

![image](https://hackmd.io/_uploads/S1eFfB6gke.png)

thật may khi tổi điều chỉnh đã thấy 1 ít lá cờ.

![image](https://hackmd.io/_uploads/Hk32GB6gkx.png)

chỉ cần chỉnh thêm 1 xíu nữa là hoàn thành rồi

![image](https://hackmd.io/_uploads/rJGZ7HTlkl.png)

flag : picoCTF{qu1t3_a_v13W_2020}
