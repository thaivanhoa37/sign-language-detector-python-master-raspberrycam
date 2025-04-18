# sign-language-detector-python-master-raspberrycam



# Hướng dẫn cài đặt OpenCV, MediaPipe và Scikit-learn trên Raspberry Pi

Để chạy code trên Raspberry Pi, bạn cần cài đặt một số thư viện Python. Dưới đây là các bước chi tiết để cài đặt OpenCV, MediaPipe và Scikit-learn.

## 1. Cài đặt OpenCV,Picammera2
Để cài đặt Picammera2 qua `apt`, chạy các lệnh sau:

```bash
sudo apt update
sudo apt install -y python3-picamera2
```

Sau khi cài đặt, kiểm tra xem Picammera2 đã được cài đặt thành công chưa bằng cách:

```bash
python3 -c "from picamera2 import Picamera2; print('Picamera2 is installed and working\!')"
```
để kiểm tra version picammera2 
```bash
pip show picamera2
```


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














# Hướng dẫn SSH  để VNC 
# SSH and VNC Setup Guide for Raspberry Pi

## 1. Check SSH Status

```bash
sudo systemctl status ssh
```

## 2. Install SSH (if not already installed)

```bash
sudo apt-get update
sudo apt-get install openssh-server
```

## 3. Enable and Start SSH Service

```bash
sudo systemctl enable ssh
sudo systemctl start ssh
```

## 4. Enable VNC on Raspberry Pi

```bash
sudo raspi-config
```

### In the menu, navigate to:

- **Interface Options**
- **VNC**
- Select **Yes** to enable

## 5. Start VNC Server

```bash
vncserver
```


