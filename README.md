
Tiến hành Scan dirb

![image](https://user-images.githubusercontent.com/72652376/126429754-d2a78bf4-9a24-4f74-906c-5d99db1f1ab5.png)

Web sử dụng WPS

![image](https://user-images.githubusercontent.com/72652376/126429729-307948b9-9ba3-4cc9-a4ea-467fd76dba19.png)

Sử dụng wps để can thêm thì thấy được /robots.txt

![image](https://user-images.githubusercontent.com/72652376/126429481-b9ebcccb-b6e6-4013-84d5-16e5d4983e04.png)

Có được cờ đầu tiên và một wordlist có vẻ dài:

![image](https://user-images.githubusercontent.com/72652376/126429536-59cf65c2-a23c-4038-9ef8-08e6f7874561.png)


Sắp xếp lại wordlist và lọc những từ trùng nhau để wordlist giảm đi:

![image](https://user-images.githubusercontent.com/72652376/126425224-ab306e29-a694-4e3d-81ab-9fa23d2d4a1d.png)

![image](https://user-images.githubusercontent.com/72652376/126425290-a8edb7d0-025d-4430-8b8d-f10c1defe878.png)

Lọc được rất nhiều chuỗi trùng nhau

![image](https://user-images.githubusercontent.com/72652376/126425328-1ef14a6f-73d2-4ccb-b055-78a0f55ac8d0.png)

Buruce thành công với user elliot (cái này mk đọc hint chứ k tìm được user :v )

![image](https://user-images.githubusercontent.com/72652376/126425388-75cc1bd0-e520-4f25-b173-7c5f77b6397d.png)

Tạo ra 1 payload sử dụng msfvenom 

![image](https://user-images.githubusercontent.com/72652376/126428288-a38667e8-3f20-4006-8af5-b785f1f15995.png)

Insert payload vào file 404.php

![image](https://user-images.githubusercontent.com/72652376/126428410-36cbbe57-081c-442e-8876-e4135a74ec58.png)

![image](https://user-images.githubusercontent.com/72652376/126428445-4ead7ea1-742c-4d11-b9be-1a7dcdb3aca9.png)

Tại kali sử dụng multi/handler lắng nghe:

![image](https://user-images.githubusercontent.com/72652376/126428523-09c2bb5e-89a3-49ca-8c32-b276e50bedc6.png)

![image](https://user-images.githubusercontent.com/72652376/126428614-a30e2867-b3e4-479b-bcef-6bb05fefa0a7.png)

Có key thứ 2 và pass của user robot ở dạng md5 

![image](https://user-images.githubusercontent.com/72652376/126428664-8c310603-1027-4dd2-9ae2-0860af15dad2.png)

Pass được decode ra tại https://crackstation.net/

Sử dụng lệnh <code> python -c 'import pty; pty.spawn("/bin/bash")' </code> để trở về dạng bash tiến hành login vào user robot

![image](https://user-images.githubusercontent.com/72652376/126428745-ae69eb7f-f9c8-4a4d-9cb3-a5033e5d40af.png)

Tìm kiếm cách leo thang đặc quyền:

![image](https://user-images.githubusercontent.com/72652376/126428930-9d7d43f7-730f-424d-b841-599343e30c88.png)

![image](https://user-images.githubusercontent.com/72652376/126428969-9bd17ce3-e9b1-4f9c-9140-88be30d593c4.png)

Kiểm tra xem nmap có dùng được không:

![image](https://user-images.githubusercontent.com/72652376/126429019-5427199a-43f6-4236-bf04-19e7529cd4e2.png)

Leo thang thành công và có được key thứ 3

![image](https://user-images.githubusercontent.com/72652376/126429359-d9e83e1c-7cbc-4fb2-8f60-4107fe784f2f.png)


DONE....!

