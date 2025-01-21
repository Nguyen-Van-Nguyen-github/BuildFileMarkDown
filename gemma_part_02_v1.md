# Gemma
Người viết: Nguyễn Văn Nguyễn  <br>
Email: nguyenvannguyen192402@gmail.com  <br>
A. Các phần chi tiết của báo cáo này. <br>
1. Xây dựng dataset cho huấn luyện Gemma với chủ đề du lịch và địa lý. <br>
2. Nghiên cứu Research system role + system prompt.<br>
B. Nội dung.<br>
I. Xây dựng dataset cho huấn luyện Gemma với chủ đề du lịch và địa lý.<br>
Gồm<br>
- Bước 1: thu thập dữ liệu thô từ wikipedia về chủ đề du lịch với địa lý (bước này sử dụng code python).<br>
- Bước 2: sử dụng chatgpt xử lý từ text thô ban đầu chuyển thành dạng dataset cho huấn luyện gemma.<br>
{"instruction": "câu hỏi", "context":"", "response": "câu trả lời", "category": "du_lich"}<br>
- câu hỏi: là câu hỏi mà mô hình chatgpt sinh ra sau khi xử lý nội dung text đầu vào.<br>
- câu trả lời: là câu trả lời mà mô hình trích xuất từ text ban đầu để trả lời câu hỏi.<br>
* Ví dụ cho cách tạo dữ liệu:<br>

