# Gemma
Người viết: Nguyễn Văn Nguyễn  <br>
Email: nguyenvannguyen192402@gmail.com  <br>
# A. Các phần chi tiết của báo cáo này. <br>
1. Xây dựng dataset cho huấn luyện Gemma với chủ đề du lịch và địa lý. <br>
2. Nghiên cứu Research system role + system prompt.<br>
# B. Nội dung.<br>
I. Xây dựng dataset cho huấn luyện Gemma với chủ đề du lịch và địa lý.<br>
Gồm<br>
- Bước 1: thu thập dữ liệu thô từ wikipedia về chủ đề du lịch với địa lý (bước này sử dụng code python).<br>
- Bước 2: sử dụng chatgpt xử lý từ text thô ban đầu chuyển thành dạng dataset cho huấn luyện gemma.<br>
{"instruction": "câu hỏi", "context":"", "response": "câu trả lời", "category": "du_lich"}<br>
- câu hỏi: là câu hỏi mà mô hình chatgpt sinh ra sau khi xử lý nội dung text đầu vào.<br>
- câu trả lời: là câu trả lời mà mô hình trích xuất từ text ban đầu để trả lời câu hỏi.<br>
* Ví dụ cho cách tạo dữ liệu:<br>
![Hình 1.1](Hinh1_1.png)
Hình ảnh trên là dữ liệu thô ban đầu thu thập được trên internet như wiki và các website du lịch. <br><br>
![Hình 1.2](Hinh1_2.png) <br>
Yêu cầu mà người dùng (user) truyền vào mô hình. <br><br>
![Hình 1.3](Hinh1_3.png) 
Kết quả mô hình ChatGPT trả về. <br><br>
* file dữ liệu hiện tại 15 nghìn dòng file jsonl.<br>
Xem file chi tiết tại [link](https://drive.google.com/file/d/1Hy_1WjY7aIDTOuLcEO3iZ7Dh3xm6q7WZ/view) <br>
# II. Research system role + system prompt  <br>
# System Prompt: lời nhắc hệ thống. <br>
+ Là những hướng dẫn do các nhà phát triển mô hình AI cung cấp cho các mô hình AI.<br>
+ Được thiết lập ngữ cảnh, giọng điệu, ranh giới cho các lời phản hồi. <br>
=> Lời nhắc hệ thống hoạt động như một khuôn khổ hướng dẫn, định hình hành vi và phong cách của AI trong suốt quá trình tương tác, để đảm bảo rằng mô hình phù hợp với mục tiêu cụ thể cung cấp trải nghiệm người dùng mong đợi, duy trì tính nhất quán trong phản hồi.
# 1. Ví dụ Prompt <br>
- Prompt cơ bản (Prompt đơn) mà người dùng thường nhập thông tin cho mô hình. <br>
![Hình 2.1](Hinh2_1.png)

![Hình 2.2](Hinh2_2.png)

![Hình 2.3](Hinh2_3.png)

# 2. Ví dụ System Prompt. <br>
- System Prompt chứa ngữ cảnh, hướng dẫn và mô tả nhiệm vụ chi tiết cho mô hình.
![Hình 2.1.1](Hinh2_1_1.png) 

![Hình 2.1.2](Hinh2_1_2.png)

![Hình 2.1.3](Hinh2_1_3.png)

![Hình 2.1.4](Hinh2_1_4.png)

![Hình 2.1.5](Hinh2_1_5.png)

![Hình 2.1.6](Hinh2_1_6.png)

# 3. System Prompt kết hợp với ví dụ minh họa.
- System Prompt chứa ngữ cảnh, hướng dẫn và mô tả nhiệm vụ chi tiết cho mô hình với ví dụ minh họa đính kèm.
![Hình 2.2.1](Hinh2_2_1.png)
Kết Luận: Một System Prompt thường có các đặc điểm sau.
- Hướng dẫn nhiệm vụ và mục tiêu.
- Đặc điểm tính cách, vai trò và hướng dẫn giai điệu.
- Thông tin theo ngữ cảnh cho đầu vào của người dùng
- Những hạn chế về sáng tạo và hướng dẫn về phong cách.
- KIến thức, dữ liệu hoặc tài liệu tham khảo bên ngoài.
- Các quy tắc, hướng dẫn và rào cản cần thiết.
- Tiêu chuẩn và yêu cầu xác minh đầu ra.
# System Role.
#  1. Ví dụ System Role.
- Xác định và quản lý các vai trò khác nhau trong cuộc trò chuyện.
- Ví dụ minh họa với ChatGPT.
# 2. Vai trò người dùng Role user
- Đại diện cho con người tương tác với mô hình AI.
- 























