# Meta Lead Automation

Tự động nhận tin nhắn và bình luận Facebook, dùng AI (Gemini) phân loại khách hàng,
lưu vào Notion CRM và báo cho Sale qua Telegram.

## Các workflow
| # | Tên | Chức năng |
|---|-----|-----------|
| 02 | Meta Messenger Intake | Nhận tin nhắn Messenger, gộp tin nhắn liên tiếp, đọc ảnh, phân loại và trả lời |
| 03 | Meta Sale Actions | Sale bấm "Nhận lead" trên Telegram, bot tạm dừng |
| 04 | Meta Comment Polling | Quét comment mỗi phút, ghi lead, trả lời comment |

## Công nghệ
n8n, Meta Graph API, Google Gemini, Notion API, Telegram Bot

## Cách cài đặt
1. Trong n8n chọn Import from file, nạp từng file trong thư mục `workflows/`.
2. Tạo credentials: Notion, Telegram, Google Gemini, Meta Page Access Token.
3. Thay các placeholder `YOUR_...` bằng giá trị thật của bạn.
4. Tạo database Notion theo các cột mà workflow sử dụng.