

Sơ lược về hệ thống:

- class User kế thừa public class Information và "has-a" class Account
- class Console "has-a" class User, chứa tài khoản của manager và dùng để thực hiện các năng hệ thống.
- namespace Cloud dùng để sử dụng để sao lưu và phục hồi dữ liệu hệ thống trên GitHub
- namespace gotp dùng để tạo, hiện thị và xác thực OTP.
- namespace Menu dùng để hiện thị các chức năng hệ thống.
- một file main.cpp dùng để chạy chương trình khi double click vào run.bat
- các file còn lại trừ folder thư viện băm kiểu brcypt cho mật khẩu (thư viện này tải bên ngoài về).
- 1 folder data:
	- folder: store_information: lưu trữ đối tượng class Information(với tên file là "user_name" của class Account)
	- folder: store_password: lưu trữ mật khẩu(với tên file là "user_name" của class Account)
	- folder: store_walet: lưu trữ tiền(với tên file là "ID" của class Information) và trong này lưu trữ ví tổng (tên là "total_wallet.txt") sẽ trích ra radom từ 0 - > giá trị lớn nhất 	của kiểu dữ liệu unsigned short.
	- folder: user_transaction_history: lưu trữ lịch sử giao dịch của từng người dùng (với tên file là "ID" của class Information)
	- file: transaction_log : lưu trữ lịch sử giao dịch của hệ thống.
- mọi thay đổi điều được sao lưu và khi gặp lỗi thì lỗi hệ thống sẽ tự restore.
- hệ thống này chưa được tối ưu về mặt thuật toán và bộ nhớ nên sẽ có đôi lúc khá chậm.




