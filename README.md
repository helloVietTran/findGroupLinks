Cần cài thư viện dành cho testing playwright

Input: 
- Tên các nhóm
 
Output:
- Link tương ứng của group

Logic đơn giản:
- Có một danh sách các link group
- Playwright giả lập người dùng truy cập từng link, tìm selector chứa tên group sau đó so sánh chuỗi

Fail mode: selector của thẻ chứa tên nhóm đang được mã hóa, nếu Whatsapp bảo trì và tiến hành build lại => tên class thay đổi, playwright sẽ không truy cập vào selector cũ => Đổi lại selector theo thực tế
