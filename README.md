# sign-language-detector-python-master-raspberrycam



# Hướng dẫn cài đặt OpenCV, MediaPipe và Scikit-learn trên Raspberry Pi

Để chạy code trên Raspberry Pi, bạn cần cài đặt một số thư viện Python. Dưới đây là các bước chi tiết để cài đặt OpenCV, MediaPipe và Scikit-learn.

## 1. Cài đặt OpenCV

Để cài đặt OpenCV qua `apt`, chạy các lệnh sau:

```bash
sudo apt update
sudo apt install -y python3-opencv
```

Sau khi cài đặt, kiểm tra xem OpenCV đã được cài đặt thành công chưa bằng cách:

```bash
python3 -c "import cv2; print(cv2.__version__)"
```

## 2. Cài đặt MediaPipe

Để cài đặt MediaPipe, chạy lệnh sau:

```bash
pip install mediapipe --break-system-packages
```

Sau khi cài đặt, kiểm tra xem MediaPipe đã được cài đặt thành công chưa bằng cách:

```bash
python3 -c "import mediapipe as mp; print(mp.__version__)"
```

## 3. Cài đặt Scikit-learn

Để cài đặt Scikit-learn, chạy lệnh sau:

```bash
pip install scikit-learn --break-system-packages
```

Sau khi cài đặt, kiểm tra xem Scikit-learn đã được cài đặt thành công chưa bằng cách:

```bash
python3 -c "import sklearn; print(sklearn.__version__)"
```

## Phiên bản

Dưới đây là các phiên bản thư viện được sử dụng:

- **Python:** 3.11.2
- **OpenCV:** 4.11.0
- **MediaPipe:** 0.10.18
- **Scikit-learn:** 1.6.1

## Ghi chú

- Đảm bảo rằng bạn đã cài đặt `pip` trước khi cài đặt các thư viện bằng lệnh:
  ```bash
  sudo apt install -y python3-pip
  ```
- Sử dụng `--break-system-packages` để tránh xung đột với các gói hệ thống trên Raspberry Pi.
- Nếu gặp lỗi, hãy kiểm tra lại phiên bản hệ điều hành và cập nhật trước khi tiếp tục:
  ```bash
  sudo apt update && sudo apt upgrade -y
  ```