# System Instruction in Gemma and Fine tune model Gemma using Unsloth
Người viết: Nguyễn Văn Nguyễn  <br>
Email: nguyenvannguyen192402@gmail.com  <br>
# A. Các phần chi tiết của báo cáo này. <br>
I. System Instruction in Gemma. <br>
II. Fine tune model Gemma using Unsloth.<br>
# B. Nội dung.<br>
I. System Instruction in Gemma.<br>
1. Đặc điểm mô hình Gemma 2 9B.
-đặc điểm role system: trước khi chat bot bắt đầu hội thoại, system prompt (trong gemma là system instruction) sẽ được gửi lên đầu tiên để hướng dẫn mô hình cách phản hồi yêu cầu của người dùng.
-các mô hình LLM (ví dụ: gemma) sẽ không tự quản lý role => chúng ta phải truyền role cho mô hình dưới dạng context (messages).
