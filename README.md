<h1 align = "center">
  <br>
  <a href="https://github.com/TruongThach2006/Tbomb-spam"> <img src = "https://i.ibb.co/F4HBKqm/TBomb.png" alt = "TBomb"> </a>
  <br>
  TBomb v3.1b
  <br>
</h1>


<p align = "center"> Ứng dụng đặt bom cuộc gọi / SMS mã nguồn mở và miễn phí </p>

## GHI CHÚ:


> ** Do lạm dụng script, một loạt API đã được đưa vào ngoại tuyến. Không sao cả nếu bạn không nhận được tất cả các tin nhắn. **


- Ứng dụng yêu cầu kết nối internet hoạt động để liên hệ với các API
- Bạn sẽ không bị tính phí cho bất kỳ SMS / cuộc gọi nào được gửi đi do hệ quả của tập lệnh này
- Để có hiệu suất tốt nhất, hãy sử dụng luồng đơn với thời gian trễ đáng kể
- Luôn đảm bảo rằng bạn đang sử dụng phiên bản mới nhất của TBomb và có Python 3
- Ứng dụng này không được sử dụng để gây hại / khó chịu / rắc rối cho người khác
- Bằng cách sử dụng này, bạn đồng ý rằng bạn không thể bắt các cộng tác viên chịu trách nhiệm về bất kỳ việc sử dụng sai mục đích nào

## Khả năng tương thích
Kiểm tra phiên bản Python của bạn bằng cách nhập vào
`` shell script
$ python - phiên bản
``
Nếu bạn nhận được những điều sau đây
`` shell script
Python 3.8.3
``
hoặc bất kỳ phiên bản nào lớn hơn hoặc bằng 3.4, tập lệnh này đã được kiểm tra và xác nhận là được hỗ trợ. Đối với các phiên bản Python lỗi thời (ví dụ 2.7), hãy tùy ý sử dụng trong khi thực thi tập lệnh vì nó chưa được kiểm tra ở đó.

## Đặc trưng

- Hơn 15 API nhắn tin và gọi điện tích hợp đi kèm với JSON
- Không giới hạn (với bảo vệ chống lạm dụng) và ném bom siêu nhanh với đa luồng
- Khả năng hỗ trợ API quốc tế (API ngoại tuyến)
- Linh hoạt với việc bổ sung các API mới hơn với sự trợ giúp của các tài liệu JSON
- Được hỗ trợ tích cực bởi các nhà phát triển với các bản cập nhật và sửa lỗi thường xuyên
- Bao gồm tính năng tự động cập nhật trực quan và tính năng tìm nạp thông báo
- Gần đây được tạo miễn phí và mã nguồn mở để đóng góp cho cộng đồng
- Cơ sở mã mô-đun và đoạn mã có thể dễ dàng nhúng vào chương trình khác


## Sử dụng:

### Cài đặt bởi PIP (Khuyến nghị)

Trước khi tiếp tục, hãy đảm bảo đáp ứng các yêu cầu sau:

- Phiên bản Python lớn hơn hoặc bằng 3.4 được cài đặt
- pip được cài đặt cho Python 3

Cài đặt gói `tbomb` bằng cách chạy:

`` shell script
pip3 cài đặt tbomb
``

Chạy TBomb chỉ bằng cách gõ:
`` shell script
tbomb
``

### Cài đặt từ GIT

#### GHI CHÚ 

Các phương pháp cài đặt Git không phổ biến và có thể khác nhau giữa các bản phân phối, do đó, việc cài đặt Git theo hướng dẫn dưới đây có thể không hoạt động. Vui lòng xem cách cài đặt Git cho bản phân phối Linux của bạn [tại đây] (https://git-scm.com/). Các lệnh dưới đây cung cấp hướng dẫn cho các hệ thống dựa trên Debian.

> Chạy `TBomb.sh` khi sudo định cấu hình sai quyền sở hữu tệp. Không nên chạy nó dưới dạng sudo

Chạy các lệnh này để sao chép và chạy TBomb.

#### Đối với Termux

Để sử dụng máy bay ném bom, hãy nhập các lệnh sau trong Termux:
`` shell script
pkg cài đặt git -y 
pkg cài đặt python -y 
git clone https://github.com/TheSpeedX/TBomb.git
cd TBomb
./TBomb.sh
``

#### Đối với iSH

Để sử dụng ứng dụng, hãy nhập các lệnh sau vào iSH.
`` shell script
apk thêm git
apk thêm python3
apk thêm py3-pip
apk thêm ruby
đá quý cài đặt nhà vệ sinh
git clone https://github.com/TheSpeedX/TBomb.git
cd TBomb
pip3 install -r request.txt
chmod + x TBomb.sh
./TBomb.sh
``

#### Đối với các bản phân phối GNU / Linux dựa trên Debian

Để sử dụng ứng dụng, hãy nhập các lệnh sau vào thiết bị đầu cuối GNU / Linux.
`` shell script
sudo apt install git
git clone https://github.com/TruongThach2006/Tbomb-spam.git
cd TBomb
bash TBomb.sh
``

#### Đối với MacOS

Để sử dụng ứng dụng, hãy nhập các lệnh sau vào thiết bị đầu cuối MacOS:

##### Cài đặt Brew

`` shell script
/ usr / bin / ruby ​​-e "$ (curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
`` '

##### Cài đặt các phần phụ thuộc:

`` shell script
brew cài đặt git
pha cài đặt python3
sudo easy_install pip
sudo pip cài đặt - nâng cấp pip
git clone https://github.com/TruongThach2006/Tbomb-spam.git
cd TBomb
bash TBomb.sh
``


##### Thiếu Công cụ trên MacOS

Chưa thể cài đặt gói `toilet` trên macOS. Nhưng TBomb vẫn hoạt động.

### Video minh họa:

- Xem Phương pháp ném bom của Ấn Độ [tại đây] (https://youtu.be/9KWkwsr_QGw)  
- Xem Phương pháp ném bom quốc tế [tại đây] (https://youtu.be/JqsHkyIcnPM).  

## Người đóng góp

- Bắt ** [t0xic0der] (https://github.com/t0xic0der) ** tại https://atlasdoc.netlify.app
- Kiểm tra ** [Avinash] (https://github.com/AvinashReddy3108) ** tại https://github.com/AvinashReddy3108
- Thư ** [scpketer] (https://github.com/scpketer) ** tại scpketer@protonmail.ch
- Thư ** [0n1cOn3] (https://github.com/0n1cOn3) ** tại 0n1cOn3@gmx.ch
- Ping ** Rieltar ** tại https://t.me/RieltarReborn


### Các nhà ủng hộ:

- ** [34D30Y] (34db0y@protonmail.com) **
- ** SC AMAN **

### LÀM:

- [x] Làm cho mã dễ đọc hơn và có thể mở rộng
- [] Thêm nhiều API thư rác
- [] Thêm nhiều API thư rác SMS hơn
- [] Thêm nhiều API thư rác cuộc gọi
- [] Giải quyết vấn đề phân luồng trong một số thiết bị

## Câu hỏi thường gặp

** Q: ** Có Trang web / Ứng dụng TBomb nào không?

** A: ** Chưa có trang web / ứng dụng chính thức. Các bản phát hành chính thức duy nhất của TBomb được xuất bản trên [Github] (https://github.com/TheSpeedX/TBomb) và [PyPi] (https:// pypi .org / project / tbomb)
##
** Q: ** Phát hiện kết nối Internet kém:

** A: ** Dưới đây là một số công cụ bạn có thể thử:
- Kiểm tra kết nối của bạn.
- Đảm bảo rằng `openssl` đã được cài đặt.
- Cố gắng `ping` bất kỳ trang web / địa chỉ từ xa nào để chắc chắn.
- Cố gắng cài đặt lại nếu không có gì hoạt động.
##
** Q: ** Bạn có ủng hộ Quốc gia "X" không?

** A: ** Hầu hết các Quốc gia được hỗ trợ SMS và chỉ Ấn Độ cho các cuộc gọi. Tốc độ gửi SMS có thể khác nhau đối với các quốc gia khác nhau.
##
** Q: ** Bạn có thể thêm hỗ trợ cho Quốc gia "X" không?

** A: ** Chúng tôi làm những gì chúng tôi có thể, nhưng chúng tôi không thể hứa. Hãy theo dõi để được hỗ trợ trong tương lai. Nếu bạn sẵn sàng trợ giúp thì có lẽ chúng tôi có thể làm nhanh hơn.
##
** Q: ** Tại sao giới hạn quá thấp?

** A: ** Do số lượng yêu cầu nhiều, các API có thể chết. Để ngăn chặn sự tiêu thụ lớn hơn của TBomb, nó đã bị hạn chế.
##
** Hỏi: ** Trợ giúp, tôi gặp lỗi là các yêu cầu không được cài đặt, ngay cả khi trình cài đặt đã truy cập thành công menu chính

** A: ** Trước tiên, hãy đảm bảo rằng `python3` và` pip3` đã được cài đặt. 
- Phương pháp dễ dàng:  
   `pip3 install tbomb`  
    Sau đó thực thi bằng cách chạy `tbomb`
- Phương pháp Git:  
    Sao chép repo và Chuyển sang Thư mục TBomb và thực hiện lệnh này:  
    `pip3 install -r request.txt`
##
** Q: ** Trợ giúp, Nó nói rằng `` lệnh 'tbomb' không tìm thấy 'sau khi cài đặt phiên bản PIP!

** A: ** Thử chạy `sudo pip3 install tbomb`
##
** Hỏi: ** Giúp tôi với, tôi không thể thực thi TBomb.sh!

** A: ** Chạy TBomb Trực tiếp với `python3 bomber.py`
##
** Q: ** Tôi có nên sử dụng VPN không? 

** A: ** Không, Nếu bạn đang phải đối mặt với tỷ lệ thất bại cao vì TBomb có thể bị lỗi do thời gian phản hồi cao hoặc các hạn chế của API.
##
** Q: ** Làm thế nào để nhận được sự bảo vệ?

** A: ** Sử dụng trình chặn OTP và kích hoạt DND.
##
** Q: ** Tại sao nó không thành công?

** A: ** Do lạm dụng script, một loạt API đã được đưa vào ngoại tuyến. Không sao cả nếu bạn không nhận được tất cả các tin nhắn.
##
### Ủng hộ

Đối với các truy vấn: [Telegram Group] (https://t.me/TBombChat)  
Các đóng góp, vấn đề và yêu cầu tính năng đều được hoan nghênh!  
Cho một ★ nếu bạn thích dự án này!

<p align = "right"> Cập nhật câu hỏi thường gặp lần cuối: 08.08.2021 </p>
