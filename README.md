# EduSkill-Ledger

# tên: EduSkill Ledger
# mô tả: EduSkill Ledger (ESL) là một nền tảng xác thực chứng chỉ số phi tập trung được xây dựng trên mạng lưới blockchain Stellar.
#Dự án cung cấp giải pháp để các tổ chức giáo dục, câu lạc bộ hoặc ban tổ chức sự kiện chuyển đổi các thành tích, kỹ năng thực tế, hoặc chứng nhận tham gia workshop của người dùng thành các tài sản số định danh (Soulbound Tokens - SBT). ESL tạo ra một hệ sinh thái minh bạch, nơi người học có thể xây dựng một "Hồ sơ năng lực số" không thể làm giả, và các bên thứ ba (nhà tuyển dụng, đối tác) có thể xác minh thông tin ngay lập tức với chi phí gần như bằng không.

# chức năng:
#Dựa trên 4 hàm chính đã viết trong file lib.rs, hệ thống có các chức năng vận hành sau:

#Khởi tạo & Phân quyền quản trị (init): Chức năng thiết lập định danh on-chain cho các đơn vị phát hành (nhà trường, trung tâm đào tạo, ban tổ chức). Tính năng này khóa quyền kiểm soát, đảm bảo chỉ những tổ chức uy tín, được xác thực mới có quyền cấp phát chứng chỉ, loại bỏ hoàn toàn rủi ro giả mạo nguồn gốc.

#Đúc & Cấp phát chứng chỉ số (mint_cert):
#Cho phép tổ chức phát hành ghi nhận một kỹ năng cụ thể (Ví dụ: "Lãnh đạo đội nhóm", "Giải nhất cuộc thi học thuật") và đẩy trực tiếp vào ví kỹ thuật số của người đạt được. Các chứng nhận này được thiết kế theo chuẩn Soulbound (không thể mua bán, chuyển nhượng), gắn chặt vĩnh viễn với danh tính người nhận.

#Thu hồi & Quản trị rủi ro (revoke_cert):
#Tính năng tuân thủ (Compliance) quan trọng giúp nền tảng giữ được sự trong sạch. Nếu phát hiện sai sót trong khâu nhập liệu hoặc người nhận vi phạm quy chế (gian lận thi cử), quản trị viên có quyền thu hồi và xóa bỏ chứng chỉ đó khỏi sổ cái blockchain.

#Tra cứu & Xác minh tức thì (verify_cert):
#Cổng tra cứu công cộng dành cho nhà tuyển dụng hoặc các tổ chức đối tác. Chỉ cần nhập địa chỉ ví của ứng viên và tên kỹ năng, hệ thống sẽ đối chiếu trực tiếp với dữ liệu blockchain và trả về kết quả hợp lệ/không hợp lệ chỉ trong vài giây, thay vì phải liên hệ trực tiếp với đơn vị cấp bằng để xác minh giấy tờ như trước đây.

#<img width="1729" height="690" alt="image" src="https://github.com/user-attachments/assets/96975b20-7f8d-4c23-b7a7-308a2c5e0a8b" />
