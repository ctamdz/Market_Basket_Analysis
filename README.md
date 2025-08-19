# 🛒 Market Basket Analysis

##  Tổng quan dự án

Dự án **Market Basket Analysis** (Phân tích Giỏ hàng) nhằm xác định các sản phẩm thường được mua cùng nhau để tối ưu hóa chiến lược kinh doanh và cải thiện trải nghiệm khách hàng.

##  Mục tiêu

- **Xác định sự tương quan giữa các sản phẩm**: Tìm hiểu các sản phẩm nào thường được mua cùng nhau
- **Tối ưu hóa chiến lược bán hàng**: Đưa ra khuyến nghị về bố trí sản phẩm và gói sản phẩm
- **Cải thiện hệ thống gợi ý**: Phát triển hệ thống đề xuất sản phẩm thông minh

##  Công nghệ sử dụng

- **Python 3.x**
- **Pandas**: Xử lý và phân tích dữ liệu
- **Matplotlib**: Tạo biểu đồ
- **Seaborn**: Trực quan hóa dữ liệu nâng cao
- **Jupyter Notebook**: Môi trường phát triển

##  Dataset

Dữ liệu được sử dụng từ: https://raw.githubusercontent.com/sca-programming-school/datasets/main/transactions.csv

**Cấu trúc dữ liệu:**
- `TransactionID`: Mã giao dịch
- `Product`: Tên sản phẩm
- `Amount`: Số lượng sản phẩm

## 🔬 Phương pháp phân tích

### 1. Chuẩn bị dữ liệu
- Tải dữ liệu giao dịch từ nguồn trực tuyến
- Tạo Pivot Table với giao dịch làm hàng và sản phẩm làm cột

### 2. Tính toán ma trận tương quan
- Sử dụng phương pháp correlation để tính toán mối quan hệ giữa các sản phẩm
- Phân tích các giá trị tương quan dương và âm

### 3. Trực quan hóa
- Sử dụng Seaborn heatmap để hiển thị ma trận tương quan
- Tạo biểu đồ màu sắc dễ hiểu

##  Kết quả chính

### Tương quan tích cực mạnh
- **Bánh mì và Bơ**: Thường được mua cùng nhau
- **Phô mai và Mứt**: Có mối quan hệ bổ sung tự nhiên

### Tương quan tiêu cực
- **Phô mai và Sữa**: Khách hàng thường chọn một trong hai sản phẩm sữa
- **Mứt và Sữa**: Mô hình thay thế tương tự

### Tương quan yếu/không có
- Hầu hết các cặp sản phẩm có tương quan yếu, cho thấy hành vi mua sắm đa dạng

##  Ứng dụng kinh doanh

###  Bố trí cửa hàng
- Đặt các sản phẩm có tương quan cao gần nhau
- Tạo khu vực riêng cho sản phẩm bổ sung
- Sử dụng kệ cuối để giới thiệu gói sản phẩm

###  Chiến lược gói sản phẩm
- Phát triển gói sản phẩm từ các mặt hàng có tương quan tích cực
- Tạo "giải pháp bữa ăn" kết hợp nhiều sản phẩm
- Thiết kế chiến dịch quảng cáo nhấn mạnh sự kết hợp tự nhiên

###  Quản lý kho hàng
- Dự trữ sản phẩm bổ sung với số lượng tương tự
- Phối hợp chu kỳ mua hàng cho các mặt hàng có tương quan
- Sử dụng mô hình tương quan để dự báo nhu cầu

###  Hệ thống gợi ý
- Triển khai "khách hàng mua X cũng mua Y"
- Tập trung gợi ý vào các cặp sản phẩm có tương quan cao
- Tránh gợi ý các mặt hàng có tương quan tiêu cực



##  Phát triển tương lai

- [ ] Thêm các thuật toán Market Basket Analysis nâng cao (Apriori, FP-Growth)
- [ ] Tích hợp dữ liệu thời gian để phân tích xu hướng
- [ ] Phát triển dashboard tương tác
- [ ] Áp dụng Machine Learning để dự đoán hành vi mua sắm
- [ ] Phân tích theo nhóm khách hàng



⭐ *Dự án được thực hiện nhằm mục đích học tập và nghiên cứu về phân tích giỏ hàng thị trường*
