# Khắc phục lỗi khai báo biến số trong prompt mẫu

## Bước 1: Phân tích lỗi

Prompt ban đầu dùng hai kiểu ký hiệu khác nhau cho biến: `[language]` và `{audience}`. Sự thiếu nhất quán này có thể gây khó khăn khi tự động hóa vì:

- Công cụ thay thế biến thường được cấu hình để tìm một quy ước cụ thể. Nếu quy ước không thống nhất, một biến có thể bị bỏ sót.
- Hệ thống hoặc người dùng khó phân biệt đâu là chỗ cần thay thế, đâu là ký hiệu có ý nghĩa khác trong prompt.
- Tên biến viết thường và bằng tiếng Anh (`language`) cũng kém rõ ràng hơn tên biến được chuẩn hóa, dễ đọc với người sử dụng prompt.

## Bước 2: Prompt đã đồng bộ biến số

> Hãy viết một bài chia sẻ về **Cấu trúc Prompt Tiêu chuẩn & Định dạng** bằng ngôn ngữ **[NGÔN_NGỮ]**. Dành cho đối tượng **[ĐỐI_TƯỢNG]**.

Cả hai biến đều dùng ngoặc vuông, viết hoa và đặt tên rõ nghĩa. Khi tự động hóa, hãy thay `[NGÔN_NGỮ]` và `[ĐỐI_TƯỢNG]` bằng các giá trị tương ứng trước khi gửi prompt cho AI.
