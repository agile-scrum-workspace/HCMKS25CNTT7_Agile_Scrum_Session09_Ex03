# KẾ HOẠCH TỔ CHỨC SPRINT REVIEW & RETROSPECTIVE (SPRINT 12 - RIKKEIASSIST)

**Người thực hiện:** Scrum Master  
**Dự án:** Trợ lý ảo CSKH RikkeiAssist  
**Sprint:** 12 (Hướng dẫn đổi trả & Phân luồng khiếu nại nghiêm trọng)  

---

## PHẦN 1: BẢNG KIỂM TRA INCREMENT THEO DEFINITION OF DONE (DoD)

Căn cứ theo Definition of Done đã quy định (đạt AC, tích hợp trên môi trường thử nghiệm, sạch lỗi mức High, hoàn tất bài kiểm tra quyền riêng tư), nhóm rà soát minh bạch 5 PBI:

| PBI | Trạng thái công bố | Căn cứ cụ thể theo DoD |
| :--- | :--- | :--- |
| **PBI-51**: Hướng dẫn đổi hàng lỗi kỹ thuật | **Trình bày là Done** | Chạy mượt 32/32 kịch bản kiểm thử; đã tích hợp trơn tru trên môi trường thử nghiệm; không còn lỗi nghiêm trọng nào. |
| **PBI-52**: Hướng dẫn trả hàng theo nhóm sản phẩm | **Nói rõ chưa Done** | Đang bị chặn vì chính sách đồ điện tử còn 2 phiên bản; còn 114 hội thoại chưa thể kết luận tiêu chí nghiệm thu; chưa hoàn thành kiểm thử chấp nhận. |
| **PBI-53**: Chuyển khiếu nại nghiêm trọng | **Nói rõ chưa Done** | Vẫn còn 3/50 ca phân loại sai; lỗi mức nghiêm trọng cao (High) vẫn đang mở, vi phạm trực tiếp tiêu chí chất lượng của DoD. |
| **PBI-54**: Hiển thị lịch sử cho nhân viên tiếp nhận | **Trình bày là Done** | Đã kiểm thử đạt trên môi trường thử nghiệm; đã hoàn thành kiểm tra quyền riêng tư (Privacy Check); tích hợp tốt sau khi sửa lỗi thiếu dữ liệu ở Ngày 9. |
| **PBI-58**: Xóa dữ liệu cá nhân khỏi nội dung báo cáo | **Nói rõ chưa Done** | Mới đạt 10/12 mẫu, vẫn còn 2 mẫu để lộ số điện thoại; chưa đáp ứng tiêu chuẩn an toàn dữ liệu cá nhân nên dứt khoát không thể gắn mác Done. |

---

## PHẦN 2: CHUẨN BỊ VÀ ĐIỀU PHỐI SPRINT REVIEW (TỐI ĐA 75 PHÚT)

### 1. Các bước chuẩn bị thực tế của Scrum Master

1. **Chốt danh sách tính năng được lên sàn (Dựa vào DoD):**  
   Thống nhất với cả nhóm chỉ mang **PBI-51** và **PBI-54** ra thao tác thực tế. Kiên quyết gạt PBI-52, 53 và 58 ra khỏi phần trình diễn sản phẩm hoàn thiện.
2. **"Nói chuyện riêng" với Product Owner để đính chính thư mời:**  
   PO trước đó ghi trong thư mời là tính năng bảo vệ dữ liệu đã xong. SM ngồi lại với PO để cập nhật lại nội dung này trước khi gửi cho Đại diện bảo vệ dữ liệu, tránh việc người ta vào họp với kỳ vọng sai rồi sinh thất vọng.
3. **Chuẩn bị kịch bản demo sống (Live Demo), dẹp bỏ video quay sẵn:**  
   Bảo vệ tinh thần minh bạch của Scrum: hướng dẫn Dev chuẩn bị sẵn kịch bản và dữ liệu thử nghiệm để chạy trực tiếp luồng PBI-51 và PBI-54 trên môi trường test. Từ chối đề xuất dùng video quay sẵn của PO để tránh che giấu lỗi ngầm.
4. **Sắp xếp agenda theo lịch bận của khách mời:**  
   Đại diện chính sách chỉ ngồi được 30 phút đầu, nên nhóm đẩy phần thảo luận chính sách của PBI-52 lên đầu chương trình, giải quyết dứt điểm các vướng mắc của họ trước khi họ rời đi.
5. **Set up kỹ thuật cho Stakeholder tham gia từ xa:**  
   Đại diện bảo vệ dữ liệu dự online nên SM kiểm tra đường truyền, micro và màn hình chia sẻ trước 15 phút. Chuẩn bị sẵn 2 mẫu báo cáo bị sót số điện thoại ở PBI-58 để show thẳng cho họ xem.
6. **Tổng hợp dữ liệu backlog và định hướng bàn luận:**  
   Hỗ trợ PO chuẩn bị bức tranh tổng thể: Sprint Goal đạt được đến đâu, tình hình phát hành thực tế thế nào và các hướng đi đề xuất để cùng thảo luận với mọi người.

---

### 2. Kịch bản trải nghiệm người dùng (User Journey Demo)
*Dựng từ 2 PBI đã Done: PBI-51 + PBI-54*

* **Tình huống:** Khách hàng Nguyễn Văn A nhắn tin lên hệ thống báo bàn phím vừa mua bị liệt phím (lỗi kỹ thuật).
* **Bước 1 (PBI-51):** Bot AI RikkeiAssist nhận diện đúng đây là lỗi kỹ thuật từ nhà sản xuất, tự động tra cứu chính sách và hướng dẫn khách các bước đóng gói, gửi kèm mã bưu gửi để đổi sản phẩm mới nhanh chóng.
* **Bước 2 (PBI-54):** Khi khách bấm nút "Gặp nhân viên hỗ trợ", toàn bộ lịch sử chat, thông tin thiết bị và mã đổi trả vừa tạo lập tức hiển thị đầy đủ trên màn hình của bạn trực tổng đài, các thông tin nhạy cảm đã được che chắn đúng chuẩn, bạn nhân viên không cần hỏi lại khách từ đầu.

---

### 3. Lịch trình chi tiết buổi Sprint Review (75 phút)

| Thời lượng | Nội dung công việc | Phân vai đóng góp thực tế |
| :--- | :--- | :--- |
| **00:00 – 00:05**<br>*(5 phút)* | **Khởi động & Nêu mục tiêu:**<br>Chào hỏi ngắn gọn, giới thiệu mục tiêu Sprint 12, nêu rõ quy tắc làm việc cởi mở và duyệt nhanh lịch trình 75 phút. | • **Scrum Master:** Giữ nhịp, nhắc nhở quy tắc minh bạch.<br>• **PO:** Nêu Sprint Goal và bức tranh chung của Sprint 12. |
| **00:05 – 00:30**<br>*(25 phút)*<br>*Ưu tiên xử lý sớm* | **Gỡ vướng PBI-52 (Trước khi Đại diện chính sách out):**<br>• Giải thích lý do PBI-52 chưa xong (114 hội thoại kẹt giữa 2 phiên bản chính sách).<br>• Làm cầu nối giữa 2 luồng ý kiến: Chủ cửa hàng muốn AI trả lời đại để đỡ kẹt khách vs. Đại diện chính sách kiên quyết cấm trả lời đồ điện tử khi luật chưa chốt. | • **PO:** Điều phối làm rõ rủi ro kinh doanh giữa hai luồng ý kiến.<br>• **Đại diện chính sách:** Chốt mốc thời gian hoàn tất bản pháp lý cuối cùng.<br>• **Chủ cửa hàng:** Chia sẻ áp lực thực tế ngoài quầy.<br>• **Scrum Master:** Giữ không khí xây dựng, không để đôi bên chốt vội các cam kết cảm tính. |
| **00:30 – 00:50**<br>*(20 phút)* | **Demo sống User Journey (PBI-51 + PBI-54):**<br>• Thao tác trực tiếp trên môi trường thử nghiệm luồng đổi hàng lỗi và hiển thị lịch sử cho nhân viên CSKH.<br>• Lắng nghe cảm nhận thực tế của các bên về độ mượt của luồng. | • **Developers:** Trực tiếp thao tác chạy hệ thống, giải đáp chi tiết kỹ thuật.<br>• **Chủ cửa hàng & CSKH:** Đóng góp ý kiến về tính tiện dụng ngoài đời thực.<br>• **PO:** Ghi nhận các phản hồi có giá trị.<br>• **Scrum Master:** Đảm bảo team bám sát kịch bản, không tiện tay bấm sang tính năng chưa Done. |
| **00:50 – 01:05**<br>*(15 phút)* | **Báo cáo minh bạch PBI-53 & PBI-58:**<br>• Trình bày PBI-53 còn 3/50 ca phân loại sai khiếu nại nghiêm trọng.<br>• Chiếu thẳng 2 file mẫu còn sót số điện thoại của PBI-58 cho Đại diện bảo vệ dữ liệu (đang họp online) xem xét. | • **Developers:** Thẳng thắn chỉ ra nguyên nhân kỹ thuật và 2 mẫu lỗi.<br>• **Đại diện bảo mật (Online):** Đánh giá mức độ ảnh hưởng và chốt điều kiện cần sửa.<br>• **PO:** Xác nhận tạm thời chưa đưa tính năng ra môi trường thật nếu chưa an toàn. |
| **01:05 – 01:15**<br>*(10 phút)* | **Tổng kết phản hồi & Thống nhất hướng đi:**<br>• Sàng lọc lại các ý kiến đóng góp, làm rõ điều kiện trước khi tính chuyện đưa vào Backlog.<br>• Dự kiến các ưu tiên cho chặng đường tiếp theo. | • **PO:** Cập nhật hướng điều chỉnh Product Backlog.<br>• **Cả nhóm & Khách mời:** Thảo luận nhanh về độ ưu tiên.<br>• **Scrum Master:** Tóm lược kết quả, đóng sự kiện đúng hạn 75 phút. |

---

## PHẦN 3: KẾ HOẠCH SPRINT RETROSPECTIVE (TỐI ĐA 60 PHÚT)

### 1. Thành phần tham gia
* **Chỉ gồm nội bộ Scrum Team:** Developers (Dev, Tester Khánh Vy), Product Owner và Scrum Master.  
* *Tuyệt đối không mời Chủ cửa hàng, Đại diện chính sách hay Quản lý bảo mật. Nhóm cần một không gian thực sự an toàn để tự nhìn nhận thiếu sót mà không sợ bị phán xét hay đổ lỗi.*

---

### 2. Bảng phân tích: Đi từ Sự việc (Data) đến Bài học (Insight)

| Data (Chuyện gì đã xảy ra?) | Khía cạnh | Insight (Nhóm hiểu ra điều gì?) |
| :--- | :--- | :--- |
| **Data 1:** Đến tận Ngày 4, Khánh Vy mới có đủ quyền vào môi trường test. Cải tiến cũ **IM-11-02** (cấp quyền từ Ngày 1 và tích hợp khi có PBI đầu tiên) lần thứ hai liên tiếp không đạt được. | **Quy trình & Công cụ** *(Process & Tools)* | Team đang viết cải tiến theo kiểu "ước gì được nấy" trên giấy mà không giao việc cụ thể cho ai, cũng chẳng chuẩn bị trước Sprint Planning. Khi gặp vướng mắc về quyền hạn từ phòng ban khác, mọi người có tâm lý chờ đợi thay vì tìm cách xử lý dứt điểm ngay từ sáng Ngày 1, dẫn đến việc test bị dồn toa về cuối Sprint. |
| **Data 2:** Đến Ngày 5, Dev và các bạn nhân viên CSKH mới nhận ra đang hiểu lệch nhau về cụm từ "khiếu nại nghiêm trọng", khiến PBI-53 bị sai 3/50 ca và còn lỗi mức High. | **Tương tác & Tiêu chí nghiệm thu** *(Interactions & DoD)* | Cả nhóm đã vội vã đưa việc vào làm khi tiêu chí nghiệm thu còn quá chung chung, dùng từ ngữ cảm tính. Trong các buổi làm mịn yêu cầu (Backlog Refinement), Dev thiếu sự trao đổi trực tiếp với nhân viên CSKH tuyến đầu để chốt danh sách các tình huống thực tế cụ thể. |

---

### 3. Kế hoạch cải tiến cụ thể (Chọn 1 việc duy nhất cho Sprint 13)

Thay vì ôm đồm nhiều thứ hay tiếp tục "gia hạn" lời hứa suông từ IM-11-02, nhóm sẽ biến nó thành một quy trình bàn giao môi trường có phân công rõ ràng, kiểm tra được và xử lý dứt điểm ngay từ đầu Sprint.

| Hành động cụ thể | Người theo dõi | Thời điểm kiểm tra | Bằng chứng hoàn thành |
| :--- | :--- | :--- | :--- |
| Thiết lập quy trình chuẩn bị môi trường: Scrum Master tạo ticket yêu cầu cấp quyền trước buổi Sprint Planning 24 giờ; Khánh Vy trực tiếp đăng nhập kiểm tra toàn bộ quyền hạn của đội ngũ kiểm thử ngay trong sáng Ngày 1. | **Khánh Vy** phối hợp cùng **Scrum Master** | **12:00 trưa Ngày 1 của Sprint 13** | Tài khoản của toàn bộ thành viên test đăng nhập thành công vào môi trường thử nghiệm và được xác nhận hoạt động bình thường trong buổi Daily Scrum Ngày 2. |