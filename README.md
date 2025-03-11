Client

# Lỗi 

# Product Filter
+ Filter theo số vé: gần trả thưởng
+ Filter theo isSpecial không truyền isOrderable và categories bị 500
+ ~~Càn lọc ra những sản phẩm đang chạy~~             
+ Có rất nhiều sản phẩm trả về totalPoint bằng 0 hoặc không trả về totalPoint
+ Sắp xếp: theo giá, theo độ yêu thích, theo lượt chơi
        
# Cược 
+ Cược vào 1 san phẩm đủ số nhưng không quay
+ Tăng thời gian playanle lên 2p        
        
# Xổ số 
+ API public bị 403
        
# Jackpot
+ API backdoor có vẻ chưa hoạt động 
- Cơ chế call backdoor (Nhắc lại)
    1. bên admin call backdoor  
    2. bên client có socket thông báo chờ quay (hoặc không có cũng được e sẽ reload lại trang thủ công)
    3. khi reload lại thì drawAt sẽ quay sau 10s (hiểu đơn giản nó giống bới khoản thời gian out of stock đến lúc draw của session)
    4. đến giờ quay thì trả socket quay như bình thường
    5. sau khi quay xong thì sẽ có phiên chơi mới sau 2p 
    6. sau khi hết thời gian khóa phiên thì tiếp tục có phiên chơi mới cho người chơi  
+ Api số người chơi bị sai: hiện tại đang trả ra danh sách người chơi bị trùng
+ ~~Public jackpot api~~
        
# Vòng quay mãy mắn     
+ API Danh sách sản phẩm bị lỗi 500
        
# Profile 
+ Update profile
--  Nếu chỉ truyền lên 1 field cần thay đổi như sdt, email, hoặc họ tên thì các field khác sẽ bị trả về rỗng
--  Nếu truyền tất cả field gồm field có thay đổi và không thay đổi thì sẽ gặp lỗi email hoặc sdt đã được sử dụng
                    
        

# Thêm
# Layout     
+ API Thông báo và socket cho thông báo 
+ API cho thanh marquee (thanh chữ chạy ngay phía dưới menu)  
+ API Bảng xếp hạng 
+ API và socket Chat 
        
# Xổ số 
+ Cần thêm api check thông tin user hiện tại có đủ để tham gia sự kiện hay không 
+ Api check user hiện tại mua được bao nhiêu vế 
+ Chưa có cơ chế nhận thưởng 
        
# Jackpot 
+ Chưa có chê chế nhận thường

# Bài viết 
+ Cần thêm tìm theo tên 
+ Cần thêm tìm theo danh mục 
        
# CSKH 
+ Cần thêm api quản lý form liên hệ 
        
# Profile 
+ Thêm api lịch sử cuợc jackpot (của user đăng nhập)
+ API Lịch sử cược xổ số 
+ API lịch sử cược jackpot 
+ lịch sử biến động số dư 
+ API nhập giftcode, lịch sử giftcode 
+ Quản lý nhận thưởng (là nơi quản lý các phần thưởng nếu người trúng chọn nhận sản phẩm)
