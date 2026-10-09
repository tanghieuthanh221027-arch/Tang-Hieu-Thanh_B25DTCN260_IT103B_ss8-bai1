Phân tích lỗi 
Lỗi 1 : sai về cơ chế FIFO : đoạn code dùng pop() thay vì shift() để lấy xe ở đầu mảng
Lỗi 2 : Sai về điều kiện vòng lặp => các giá trị bị ăn giá trị undefined

Bảng testcase
Test Case 1 : 
Trường hợp kiểm thử : TC-01 : Điều phối xe FIFO
Dữ liệu đầu vào : ['29A-112.33', '30E-889.12', '51K-678.99']
Kết quả sai thực tế : dùng pop() => '51K-678.99' ở cuối được lên sạc trước
Kết quả đúng mong đợi : dùng shift() => '29A-112.33'

Test Case 2 :
Trường hợp kiểm thử : TC-02 : Tính tổng điện và doanh thu
Dữ liệu đầu vào : [45.2, 30.5, 62.8, 28.0], đơn giá 4500 VNĐ/kWh
Kết quả sai thực tế : Đều tra về NaN
Kết quả đúng mong đợi : Tổng điện năng: 166.5 kWh; tổng doanh thu: 749250 VNĐ