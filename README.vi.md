# Weather API Application

Một ứng dụng đơn giản để kiểm tra thời tiết của bất kỳ thành phố nào. Ứng dụng được xây dựng bằng Python với giao diện PyQt5 và tích hợp API từ OpenWeatherMap để lấy dữ liệu thời tiết thực tế.

## Tính năng

- Tìm kiếm thời tiết theo tên thành phố
- Hiển thị nhiệt độ (Celsius và Fahrenheit)
- Hiển thị emoji và mô tả điều kiện thời tiết
- Xử lý lỗi cơ bản (thành phố không tìm thấy, kết nối mất, v.v.)

## Yêu cầu

- Python 3.7+
- PyQt5
- requests
- Kết nối internet

## Cài đặt

Cài đặt các thư viện phụ thuộc:
```bash
pip install PyQt5 requests
```

Chạy ứng dụng:
```bash
python main.py
```

## Cách sử dụng

1. Chạy ứng dụng: `python main.py`
2. Nhập tên thành phố vào ô input
3. Nhấn "Get Weather"
4. Xem kết quả hiển thị nhiệt độ, emoji thời tiết, và mô tả

## Cấu trúc code

**API sử dụng**: OpenWeatherMap (https://api.openweathermap.org/data/2.5/weather)

**Các hàm chính**:
- `init_ui()`: Khởi tạo giao diện
- `get_weather()`: Lấy dữ liệu thời tiết từ API
- `display_weather()`: Cập nhật kết quả lên giao diện
- `get_weather_emoji()`: Chuyển mã thời tiết thành emoji



### Xử lý lỗi

Ứng dụng xử lý các lỗi sau:
- **400**: Yêu cầu không hợp lệ (có lỗi trong câu lệnh)
- **401**: API key không hợp lệ hoặc hết hạn
- **404**: Thành phố không tìm thấy
- **Timeout**: Kết nối tới server quá lâu
- **ConnectionError**: Lỗi kết nối mạng

## Ghi chú

API key hiện được nhúng cứng trong code. Nên sử dụng biến môi trường cho các dự án sản xuất.

## Kinh nghiệm học được

Qua dự án này, tôi đã học được:
- Cách xây dựng GUI với PyQt5
- Tích hợp API bên ngoài (HTTP requests)
- Xử lý lỗi và validation dữ liệu
- Parse JSON response từ API
