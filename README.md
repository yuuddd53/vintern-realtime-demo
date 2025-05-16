# Nhận diện hình ảnh thời gian thực - mô hình Vintern 1B

## Cấu hình khuyên dùng

Mô hình Vintern rất nhẹ (1B), có thể chạy trên máy tính cá nhân mà **không cần GPU**. Khuyến khích máy tính có CPU ít nhất 8 lõi và 8GB RAM.

Tham khảo mô hình gốc tại đây: https://huggingface.co/5CD-AI/Vintern-1B-v3_5

Server chỉ cần internet để tải mô hình cho lần chạy đầu tiên. Từ lần thứ 2, bạn có thể chạy 100% **không cần internet**

## Cách thiết lập

1. Cài đặt [llama.cpp](https://github.com/ggml-org/llama.cpp)
2. Chạy lệnh `llama-server -hf ngxson/Vintern-1B-v3_5-GGUF --chat-template vicuna`  
   Lưu ý: bạn có thể cần thêm `-ngl 99` để kích hoạt GPU (nếu bạn đang sử dụng GPU NVidia/AMD/Intel)  
   Lưu ý (2): Bạn cũng có thể thử các mô hình khác [tại đây](https://github.com/ggml-org/llama.cpp/blob/master/docs/multimodal.md)
3. Mở `index.html` (hoặc có thể dùng link sau đây: https://github.ngxson.com/vintern-realtime-demo/)
4. (Tùy chọn) thay đổi hướng dẫn, ví dụ như bảo nó trả về JSON thay vì mô tả
5. Nhấn vào "Start"
