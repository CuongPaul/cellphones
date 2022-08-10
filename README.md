1. Tạo tài khoản GHN
   Đăng ký tài khoản GHN tại https://5sao.ghn.dev/
   Đăng nhập với tài khoản vừa tạo và truy cập vào phần "Quản lý cửa hàng"
   Chọn "Thêm cửa hàng" -> Điền đầy đủ thông tin -> Chọn "Thêm cửa hàng"
   Biến SHOP_ID trong file .env là ID của cửa hàng vừa được tạo (Lưu ý: Không dùng ID của cửa hàng mặc định)
   Biến TOKEN_GHN trong file .env là token API được lấy tại https://5sao.ghn.dev/account

2. Tạo tài khoản Cloudinary
   Đăng ký tài khoản GHN tại https://cloudinary.com/console/
   Đăng nhập với tài khoản vừa tạo và truy cập vào phần "Dashboard"
   Biến CLOUDINARY_NAME, CLOUDINARY_API_KEY, CLOUDINARY_API_SECRET trong file .env lần lượt là Cloud Name, API Key, API Secret tại phần Account Details.

3. Tạo tài khoản VNPay
   Đăng ký tài khoản VNPay tại https://sandbox.vnpayment.vn/devreg/
   Sau khi đăng ký thành công thì xác thực email, sau đó sẽ được nhận 1 email chứa thông tin của các biến VNP_TMN_CODE, VNP_HASH_SECRET, VNP_URL
   Biến VNP_RETURN_URL thì tự đặt ra (Đây là url được chuyển đến sau khi thanh toán thành công)
   Đồng bộ kiểu mã hoá ở code với shop tại https://sandbox.vnpayment.vn/merchantv2/Account/AccountDetail.htm -> tìm tên website -> Đổi kiểu mã hoá sang SHA256
   Mẫu thẻ:
   Ngân hàng: NCB
   Mật khẩu OTP: 123456
   Ngày phát hành: 07/15
   Tên chủ thẻ: NGUYEN VAN A
   Số thẻ: 9704198526191432198

4. Tạo tài khoản PayPal
   Đăng ký tài khoản VNPay tại https://www.paypal.com/vn/webapps/mpp/account-selection/
   Sau khi đăng ký thành công thì truy cập https://developer.paypal.com/developer/accounts/ tại đây đã có sẵn 2 account (1 business, 1 personal).
   Vào phần "My apps & credentials" -> chọn "Create app" -> Điền đầy đủ thông tin.
   Sau khi tạo xong thì chọn app vừa tạo biến PAYPAL_CLIENT_ID là mục "Client ID".
   Mẫu tài khoản:
   Email: sb-8oefe16220758@personal.example.com
   Mật khẩu: Ta@123456789
