# Nhận Diện Xe Bằng Deep Learning

## Giới Thiệu
Dự án này sử dụng **Deep Learning (CNN)** để nhận diện và phân loại xe thành hai danh mục:
- **Xe Máy**  
- **Xe Tải**  

Mô hình được huấn luyện trên TensorFlow/Keras và dữ liệu hình ảnh được xử lý từ Google Drive.

## Cài Đặt
### 1. Clone Repository
```bash
git clone https://github.com/your-username/vehicle-classification.git
cd vehicle-classification
```

### 2. Cài Đặt Thư Viện Yêu Cầu
Cài đặt các package cần thiết:
```bash
pip install tensorflow numpy opencv-python scikit-learn matplotlib
```

## Hướng Dẫn Sử Dụng
### 1. Chuẩn Bị Dữ Liệu
Lưu trữ dữ liệu hình ảnh vào Google Drive theo cấu trúc:
```
DataMoto/
├── xe_may/
│   ├── img1.jpg
│   ├── img2.jpg
│   └── ...
├── xe_tai/
│   ├── img1.jpg
│   ├── img2.jpg
│   └── ...
```

**Số lượng ảnh đề xuất:**
- **Tối thiểu 1000 ảnh cho mỗi loại** để đảm bảo mô hình học đủ đặc trưng.
- **Tỷ lệ train/test:** 80% train - 20% test.
- Nếu có ít dữ liệu, có thể sử dụng **Data Augmentation** để tăng dữ liệu.
Lưu trữ dữ liệu hình ảnh vào Google Drive theo cấu trúc:
```
DataMoto/
├── xe_may/
│   ├── img1.jpg
│   ├── img2.jpg
│   └── ...
├── xe_tai/
│   ├── img1.jpg
│   ├── img2.jpg
│   └── ...
```

### 2. Chạy Notebook
Mở Google Colab, tải notebook **Nhận_diện_xe.ipynb**, sau đó chạy từng cell.

## Mô Hình Deep Learning
Mô hình CNN bao gồm:
- **2 lớp Conv2D** (tích chập) + MaxPooling2D
- **Flatten Layer** (chuyển ma trận thành vector)
- **2 Dense Layers** (Fully Connected)
- **Hàm Loss**: `categorical_crossentropy`
- **Optimizer**: `adam`

**Lưu ý:**
- Với tập dữ liệu nhỏ (<1000 ảnh mỗi loại), có thể dùng Transfer Learning với mô hình như MobileNetV2 hoặc ResNet50 để tăng độ chính xác.
Mô hình CNN bao gồm:
- **2 lớp Conv2D** (tích chập) + MaxPooling2D
- **Flatten Layer** (chuyển ma trận thành vector)
- **2 Dense Layers** (Fully Connected)
- **Hàm Loss**: `categorical_crossentropy`
- **Optimizer**: `adam`

## Kết Quả Dự Kiến
Dự án có thể được mở rộng để nhận diện nhiều loại xe hơn, kèm theo các tính năng AI như phát hiện biển số xe, nhận diện hành vi giao thông...

## Liên Hệ
- **Author**: khuonglun69
- **Email**: khuong140702@gmail.com

# deep-learning-vehicle-recognition
