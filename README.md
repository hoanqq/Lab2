
# Nhập Môn Xử Lý Ảnh Số - Lab 2  
## **Biến Đổi Cường Độ Ảnh Grayscale & Phân Tích Bit-Plane**  
**Sinh viên thực hiện:** Nguyễn Khắc Huy Hoàng  
**MSSV:** 2374802010151  
**Môn học:** Nhập môn Xử lý ảnh số  
**Giảng viên:** Đỗ Hữu Quân  

---

## Giới thiệu

Bài lab này nhằm mục đích thực hiện **các phép biến đổi cường độ trên ảnh xám**, bao gồm:
- Biến đổi âm bản (Negative)
- Biến đổi logarit (Log Transformation)
- Biến đổi hàm mũ/Gamma
- Phân tích mặt phẳng bit (Bit-plane Slicing)

Các kỹ thuật này giúp tăng cường độ tương phản, trích xuất đặc trưng ảnh, và hỗ trợ các bài toán nâng cao trong xử lý ảnh số.

---

## Công nghệ sử dụng

- **Python**: Ngôn ngữ lập trình chính  
- **NumPy**: Xử lý ảnh dưới dạng ma trận  
- **Pillow (PIL)**: Thao tác đọc và ghi ảnh  
- **Matplotlib**: Hiển thị ảnh trực quan  
- **OpenCV (cv2)**: Một số thao tác xử lý ảnh nhanh và hiệu quả  

---

## Nội dung các phép biến đổi

### 1. Biến đổi âm bản (Negative)
- Đảo ngược giá trị pixel để làm nổi bật vùng tối/sáng
- Công thức: `s = 255 - r`

### 2. Biến đổi logarit (Log Transformation)
- Làm sáng vùng tối, giữ nguyên vùng sáng
- Công thức: `s = c * log(1 + r)`

### 3. Biến đổi gamma (Power-law)
- Điều chỉnh gamma để làm sáng hoặc tối ảnh
- Công thức: `s = c * r^γ`

### 4. Phân tích mặt phẳng bit (Bit-Plane Slicing)
- Tách ảnh thành 8 mặt phẳng bit để phân tích chi tiết đóng góp của từng bit trong ảnh

---

## Cấu trúc thư mục

```
Lab2_NguyenKhacHuyHoang_2374802010151/
├── Lab2_NguyenKhacHuyHoang_2374802010151.ipynb
├── lena.png
├── output/
│   ├── negative.png
│   ├── log.png
│   ├── gamma.png
│   ├── bit_plane_0.png
│   └── ...
└── README.md
```

---

## Hướng dẫn chạy

### 1. Cài đặt thư viện

```bash
pip install numpy pillow matplotlib opencv-python
```

### 2. Mở và chạy Notebook

- Sử dụng Jupyter Notebook hoặc Google Colab
- Chạy lần lượt từng cell để quan sát kết quả
- Có thể thay đổi các tham số như `gamma`, `bit_plane`,... để thấy hiệu ứng khác nhau

---

## Kết luận

Bài lab giúp sinh viên nắm vững các kỹ thuật cơ bản trong xử lý ảnh xám, từ đó làm nền tảng cho các bài toán nâng cao như phân đoạn, nhận dạng, nén ảnh,…

---

## Tài liệu tham khảo

- *Digital Image Processing* – Rafael C. Gonzalez  
- [https://scikit-image.org](https://scikit-image.org)  
- [https://docs.opencv.org](https://docs.opencv.org)  
- Slide bài giảng môn Nhập môn Xử lý ảnh số – Đại học Văn Lang

---
