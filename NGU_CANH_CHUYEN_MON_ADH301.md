# NGỮ CẢNH CHUYÊN MÔN HỌC PHẦN UX/UI DESIGN (ADH301)
# & PHÂN TÍCH CHUYÊN SÂU ĐỀ TÀI "STUDYMATE APPLICATION"
**Trường Đại học Công nghệ Thông tin và Truyền thông Việt - Hàn (VKU)**  
**Lớp: 23IT.B | Giảng viên phụ trách tài liệu: ThS. Trần Lê Quỳnh (TranLQ)**  
**Nhóm tác giả 5 thành viên: Lê Văn Cảm · Nguyễn Văn Quốc Triệu · Nguyễn Danh Linh · Nguyễn Đình Hoàng Nguyên · Nguyễn Đức Minh Nghĩa**

---

## PHẦN I: KHUNG CHUYÊN MÔN HỌC PHẦN ADH301 TẠI VKU

Học phần **Thiết kế Giao diện và Trải nghiệm Người dùng (UX/UI Design – ADH301)** trong Học kỳ 7 tại VKU là môn học chuẩn hóa quy trình phát triển sản phẩm kỹ thuật số kết hợp giữa **Khoa học Nhận thức Người dùng (HCI)** và **Kỹ nghệ Phần mềm Hiện đại (Software Engineering)**.

Môn học được vận hành dựa trên 3 trụ cột phương pháp luận quốc tế:
1. **Design Thinking (Stanford d.school / IDEO):** Khung quy trình 5 bước: *Empathize $\rightarrow$ Define $\rightarrow$ Ideate $\rightarrow$ Prototype $\rightarrow$ Test*.
2. **Interaction Design & HCI Foundation (Preece, Rogers, Sharp - 5th Edition):** Thiết kế mô hình khái niệm (Conceptual Model), 10 nguyên lý Heuristics của Jakob Nielsen, Định luật Fitts (Fitts' Law) và Tiêu chuẩn tiếp cận toàn diện (Accessibility - WCAG 2.1).
3. **Google UX Design Certificate & Design Sprint:** Chuẩn hóa quy trình thành một UX Case Study hoàn chỉnh, yêu cầu khảo sát thị trường trên diện rộng và đóng gói hồ sơ nghề nghiệp.

---

## PHẦN II: PHÂN TÍCH NGỮ CẢNH CHUYÊN SÂU ĐỀ TÀI "STUDYMATE APPLICATION"

Đề tài chính thức được nhóm 5 lựa chọn và phát triển là:
> **STUDYMATE APPLICATION — Quản lý học tập tín chỉ & Cộng tác bài tập nhóm thông minh cho sinh viên Trường ĐH Công nghệ Thông tin & Truyền thông Việt - Hàn (VKU)**

Dưới đây là bản phân tích toàn diện ngữ cảnh chuyên môn dựa trên hồ sơ đồ án 31 trang của nhóm tại [01 · TITLE STUDYMATE APPLICATION...pdf](file:///d:/VKU_learning/HK7/UX_UI/06_DeTai_StudyMate_VKU/01%20%C2%B7%20TITLE%20STUDYMATE%20APPLICATION%20Qu%E1%BA%A3n%20l%C3%BD%20h%E1%BB%8Dc%20t%E1%BA%ADp%20t%C3%ADn%20ch%E1%BB%89%20%26%20C%E1%BB%99ng%20t%C3%A1c%20b%C3%A0i%20t%E1%BA%ADp%20nh%C3%B3m%20th%C3%B4ng%20minh%20cho%20sinh%20vi%C3%AAn%20Tr%C6%B0%E1%BB%9Dng%20%C4%90H%20C%C3%B4ng%20ngh%E1%BB%87%20Th%C3%B4ng%20tin%20%26%20Truy%E1%BB%81n%20th%C3%B4ng%20Vi%E1%BB%87t%20-%20H%C3%A0n%20%28VKU%29%20Th%C3%A0nh%20vi%C3%AAn%20L%C3%AA%20V%C4%83n%20C%E1%BA%A3m%20%C2%B7%20Nguy.pdf):

```
                        HỆ THỐNG STUDYMATE TRONG MÔI TRƯỜNG VKU
                                           │
         ┌─────────────────────────────────┼─────────────────────────────────┐
         ▼                                 ▼                                 ▼
┌──────────────────┐             ┌──────────────────┐             ┌──────────────────┐
│ LỊCH HỌC TÍN CHỈ │             │   KANBAN NHÓM    │             │   KHO TÀI LIỆU   │
│ • Đồng bộ SSO    │             │ • 3 Cột linh hoạt│             │ • Gắn theo Môn   │
│ • Phòng & Ca học │             │ • Deadline con   │             │ • Gắn vào Task   │
│ • Đếm ngược thi  │             │ • Báo cáo tự động│             │ • Xem trước File │
└────────┬─────────┘             └────────┬─────────┘             └────────┬─────────┘
         │                                │                                │
         └────────────────────────────────┼────────────────────────────────┘
                                           │
                                           ▼
         ┌───────────────────────────────────────────────────────────────────┐
         │                    MỤC TIÊU TRẢI NGHIỆM (UX GOAL)                 │
         │  "Nhận biết lịch & việc trong 3 giây · Phân chia minh bạch 100%   │
         │   Giảm thời gian tìm kiếm từ 30 phút xuống dưới 1 phút trên ngày"  │
         └───────────────────────────────────────────────────────────────────┘
```

---

### 1. Bối cảnh Thực tế & Vấn đề Cốt lõi (The Problem Context)
Sinh viên VKU cũng như sinh viên đại học theo học chế tín chỉ tại Việt Nam đang gặp khủng hoảng về **phân mảnh thông tin học tập (Information Fragmentation)**:
- **Phân tán đa kênh:** Lịch học nằm trên Cổng thông tin sinh viên (Portal); Thông báo thi nằm trên Website trường; Thảo luận nhóm diễn ra trên Zalo / Messenger; Tài liệu nộp nằm rải rác trên Google Drive, Classroom.
- **Hệ quả thực tế:**
  - Tin nhắn bài tập và tài liệu bị trôi mất sau hàng trăm tin nhắn tán gẫu.
  - Phân công nhiệm vụ bài tập nhóm mập mờ qua chat, không có hạn chót từng chặng (sub-deadlines), dẫn đến tình trạng đùn đẩy, ỷ lại (Free-rider problem).
  - Sinh viên mất từ **25 đến 30 phút mỗi ngày** chỉ để mở nhiều ứng dụng đối chiếu xem hôm nay học môn gì, phòng nào, bài tập nào sắp đến hạn nộp.

### 2. Sự Phù hợp với Mục tiêu Toàn cầu (UN SDG Alignment)
StudyMate giải quyết trực tiếp **SDG 4: Quality Education (Giáo dục có chất lượng)** và **Mục tiêu 4.4 (Kỹ năng kỹ thuật số & Việc làm)**:
- Hỗ trợ người học nâng cao năng lực tự chủ, kỹ năng quản lý thời gian và kỹ năng làm việc nhóm chuyên nghiệp.
- Thúc đẩy chuyển đổi số thực chất trong môi trường đại học công nghệ cao như VKU.

### 3. Dữ liệu Nghiên cứu Thực nghiệm (User Research Findings)
Nhóm đã triển khai phương pháp nghiên cứu hỗn hợp (Mixed-method Research) đạt độ tin cậy khoa học cao:
- **Quy mô khảo sát:** **65 sinh viên** hoàn thành phiếu khảo sát định lượng + **10 sinh viên** phỏng vấn sâu qua 9 câu hỏi chuẩn mực.
- **6 Điểm đau cốt lõi (Pain Points) được lượng hóa:**
  1. *Deadline phân tán (85%):* Kiểm tra 3–5 app khiến bài tập nhỏ thường xuyên bị bỏ sót.
  2. *Phân công mập mờ (77%):* Giao việc qua chat thiếu rõ ràng, không có deadline từng chặng.
  3. *Thất lạc tài liệu (70%):* Slide bài giảng, link Drive trôi mất trong group chat.
  4. *Quá tải nhận thức (68%):* Nhiều môn dồn dập, bối rối không biết việc nào khẩn cấp cần làm trước.
  5. *Ỷ lại trong nhóm (62%):* Thiếu bảng theo dõi minh bạch, người làm nhiều người làm ít.
  6. *Ứng dụng hiện tại cồng kềnh (58%):* Notion hay Asana quá phức tạp, mất nhiều thời gian cấu hình trên mobile.

---

### 4. Phân tích 3 Tệp Chân dung Người dùng Đại diện (3 Personas)

Nhóm đã xây dựng 3 chân dung người dùng bao phủ trọn vẹn vòng đời sinh viên đại học:

#### Persona 1: Nguyễn Minh Anh (20 tuổi – Trưởng nhóm đồ án, SV Năm 2 VKU)
- **Đặc trưng:** Là nhóm trưởng của 3 môn học cùng lúc. Chịu trách nhiệm phân chia công việc, đôn đốc và tổng hợp nộp bài.
- **Trích dẫn tiêu biểu:** *"Làm nhóm trưởng mệt nhất là phải đi nhắn tin riêng nhắc từng bạn nộp bài qua Zalo."*
- **Problem Statement:**  
  $$\text{Minh Anh là Trưởng nhóm đồ án bận rộn} \rightarrow \text{cần giải pháp tập trung để phân chia việc minh bạch} \rightarrow \text{vì giao việc qua chat khiến nhắc nhở mất thời gian và dễ trễ hạn.}$$
- **Giải pháp cho Minh Anh:** Bảng Kanban 3 cột rút gọn gắn avatar thành viên; Đặt deadline con từng chặng trước hạn chính 2 ngày; Hệ thống nhắc việc tự động gửi thông báo đến thành viên chậm trễ.

#### Persona 2: Trần Quốc Huy (19 tuổi – Tân sinh viên Năm 1 VKU)
- **Đặc trưng:** Chưa quen phương pháp tự học tín chỉ, rụt rè trong giao tiếp nhóm, dễ bị phân tâm bởi mạng xã hội.
- **Trích dẫn tiêu biểu:** *"Lên đại học lịch học lung tung quá, em hay bị nhầm phòng học và quên bài tập nhỏ."*
- **Problem Statement:**  
  $$\text{Quốc Huy là Tân sinh viên năm nhất bỡ ngỡ} \rightarrow \text{cần công cụ nhắc lịch thông minh và thẻ việc rõ ràng} \rightarrow \text{vì môi trường tín chỉ khiến bạn quá tải, thụ động và dễ sót bài.}$$
- **Giải pháp cho Quốc Huy:** Widget lịch học thông minh hiện ca học và phòng học thời gian thực; Huy hiệu đếm ngược màu cảnh báo (Đỏ: $<24h$, Vàng: $<3$ ngày); Nút xác nhận 1-chạm nộp bài và báo nhóm.

#### Persona 3: Lê Thu Trang (21 tuổi – Sinh viên Năm cuối vừa học vừa thực tập)
- **Đặc trưng:** Ban ngày đi làm tại doanh nghiệp, tối làm đồ án tốt nghiệp; di chuyển nhiều, chủ yếu sử dụng điện thoại di động trong giờ nghỉ trưa.
- **Trích dẫn tiêu biểu:** *"Mình không có nhiều thời gian mở máy tính, cần xem file và tiến độ nhóm nhanh trên điện thoại."*
- **Problem Statement:**  
  $$\text{Thu Trang là Sinh viên năm cuối bận rộn} \rightarrow \text{cần lưu trữ tập trung và truy cập bài tập nhanh từ di động} \rightarrow \text{vì tệp học tập phân tán khiến duyệt bài tốn quá nhiều thời gian.}$$
- **Giải pháp cho Thu Trang:** Thư viện cây tài liệu gắn theo Môn học và Nhiệm vụ; Trình xem trước (Preview) trực tiếp file PDF, Slide và link Figma; Bộ lọc việc ưu tiên cao cần duyệt ngay trên mobile.

---

### 5. Ma trận Phân tích 20 Đối thủ Cạnh tranh & Cơ hội Thiết kế (USP)

Nhóm đã xuất sắc phân chia 20 ứng dụng khảo sát thành 4 phân khúc thị trường để tìm ra khoảng trống cạnh tranh (Market Gap):

| Phân khúc | Đại diện Khảo sát | Điểm mạnh | Điểm yếu | Khoảng trống cho StudyMate |
|:---|:---|:---|:---|:---|
| **1. LMS Học tập** | Canvas, Google Classroom, Moodle, Blackboard, Microsoft Teams | Quản lý điểm số, lịch thi, nộp bài chính thống. | Không có công cụ cộng tác nhóm nội bộ, không có Kanban. | **Tích hợp Kanban nhóm trực tiếp vào từng môn học.** |
| **2. Lịch & Quản lý Task** | Google Calendar, TickTick, Todoist, Any.do, Apple Reminders | Nhắc giờ chuẩn xác, widget màn hình chính tốt. | Tách rời tài liệu môn học, không hỗ trợ làm việc nhóm theo đồ án. | **Kết nối Lịch học với Deadline và kho tài liệu liên quan.** |
| **3. Ghi chú & Tài liệu** | Notion, OneNote, Evernote, Google Drive, Obsidian | Khả năng tùy biến mạnh mẽ, lưu trữ đa dạng. | Giao diện mobile quá cồng kềnh, mất nhiều thời gian cấu hình. | **Tối giản hóa: Mở app là dùng ngay, tối ưu 100% cho mobile.** |
| **4. Quản trị Nhóm** | Trello, Asana, Slack, Jira, Monday.com | Bảng Kanban trực quan, phân quyền thành viên tốt. | Quá chuyên nghiệp cho doanh nghiệp, không gắn với thời khóa biểu trường. | **Kanban học tập 3 cột tinh gọn gắn liền mã môn học và ca học.** |

> **CƠ HỘI THIẾT KẾ CHO STUDYMATE (DESIGN OPPORTUNITY / USP):**  
> StudyMate định vị là giải pháp **"All-in-one" tinh gọn tối ưu cho di động**: Tích hợp Thời khóa biểu tín chỉ + Đếm ngược Deadline cá nhân + Bảng Kanban nhóm 3 cột + Thư viện tài liệu theo môn học.

---

### 6. Mô hình Khái niệm (Conceptual Model) & Kiến trúc Thông tin (Sitemap)

- **Các ẩn dụ giao diện (Interface Metaphors):**
  - *Calendar* $\rightarrow$ Thời khóa biểu lớp học tín chỉ.
  - *Kanban Board* $\rightarrow$ Bảng dán giấy ghi chú nhóm trên lớp học.
  - *Backpack (Cặp sách)* $\rightarrow$ Kho tài liệu và đề cương môn học.
  - *Clock / Bell* $\rightarrow$ Đồng hồ đếm ngược giờ thi và hạn nộp bài.
- **Tương tác vật lý (Interaction Styles):**
  - Chạm 1 lần (Tap): Xem chi tiết ca học, bấm nút nộp bài.
  - Vuốt (Swipe): Chuyển tab giữa các ngày trong tuần và các cột Kanban.
  - Kéo thả (Drag & Drop): Di chuyển thẻ công việc từ *Đang làm* sang *Đã xong*.
- **Kiến trúc thông tin (Sitemap 4 nhánh chính):**
  1. *Trang chủ (Home):* Lịch học hôm nay, Deadline khẩn ($<24h$), Phím tắt nhóm đồ án, Tiến độ tuần.
  2. *Lịch học (Schedule):* Lịch tuần/tháng, Phòng học, Tiết học, Lịch thi, Chuông báo.
  3. *Nhóm học (Groups):* Bảng Kanban 3 cột, Giao việc & Deadline con, Quản lý thành viên.
  4. *Tài liệu (Library):* Cây thư mục môn học, Tệp đính kèm theo nhiệm vụ, Xem trước PDF/Slide trực tiếp.

---

### 7. Nguyên mẫu Khung dây (Wireframes) & Kịch bản Kiểm thử

Nhóm đã hiện thực hóa 9 Digital Wireframes bao gồm:
1. *Màn hình Chào mừng (Welcome)*
2. *Xác thực tài khoản qua cổng SSO sinh viên (@vku.udn.vn)*
3. *Màn hình Trang chủ Dashboard*
4. *Lịch học tuần (Schedule)*
5. *Danh sách Deadline phân loại theo mức độ khẩn cấp*
6. *Chi tiết Môn học & Đề cương*
7. *Không gian Kanban nhóm (Đồ án UX/UI - Lớp 23IT.B)*
8. *Thêm nhiệm vụ & Phân công người phụ trách*
9. *Chi tiết nhiệm vụ & Đánh dấu hoàn thành*

Kịch bản kiểm thử tính khả dụng (Usability Test Script) được xây dựng dựa trên hành trình đóng vai của Minh Anh: Tạo nhóm đồ án môn UX/UI, phân công 3 nhiệm vụ cho thành viên, đính kèm file đề cương và kéo thẻ việc sang hoàn thành.
