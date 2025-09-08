# Unet_base
### comment: trước hết về cấu trúc mạng unet để đơn giản dễ hình dùng nó sẽ giống hình chữ U , với kích thước input sẽ đi qua downsampling (trích xuất feature quan trọng giảm chiều h, w tăng chiều kênh), upsampling để khôi phục về kích thước gốc bằng lớp tích chập và đặc biệt không thể thiếu là skip connection vì khi ta downsampling thì nó sẽ mất thông tin ở các lớp.
### 2 bài toán phổ biến là:
  + super resolution: dùng để khôi phục lại kích cỡ bản đầu và độ nét của ảnh, input thường sẽ là ảnh size nhỏ đi qua model sẽ nhận được ảnh có kích thước lớn hơn mà vẫn giữ được độ nét nhờ phép nội suy.
  + image painting: khôi phục ảnh bị làm bẩn bằng các đường khiến ảnh mất đi 1 số chỗ
### Note: việc sử dụng model đã được pretrain sẽ tốt hơn model intialization.
### link của đoạn code cuối cùng: https://drive.google.com/file/d/1b6Mjs0nODDOo5qf7JkvoLu6ZqMqq6T9l/view?usp=drive_link
