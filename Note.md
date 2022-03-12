npx json-server --watch -p 3500 json-server/db.json

Y1. Thực hiện xây dựng các màn hình quản trị (admin) để quản lý các resources

Y2. Xây dựng các trang client để hiển thị thông tin các sản phẩm cho người dùng cuối (Trang chủ, trang danh sách sản phẩm theo danh mục, tìm kiếm theo tên,...).
T       - trang chủ
        - SP theo dm,
        tìm kiếm theo tên
Y3. Xây dựng trang chi tiết sản phẩm

Y4. Xây dựng tính năng order
- Nếu chưa tồn tại order, thì sẽ hiển thị modal yêu cầu người dùng nhập thông tin khách
hàng trước, sau đó tạo ra order mới trên resource orders. Mỗi lượt sử dụng sẽ lấy records order với trạng thái chưa hoàn thành có id lớn nhất để bổ sung sản phẩm vào. Order sẽ đóng khi người dùng click vào nút thanh toán (chuyển trạng thái thành completed)
- Có thể xem, cập nhật được số lượng các sản phẩm đang có trong order

Y5. Hiển thị danh sách các order đã lưu trong resources và hiển thị doanh thu của cửa hàng


#SEARCH:
http://localhost:3500/products?name_like=AK131