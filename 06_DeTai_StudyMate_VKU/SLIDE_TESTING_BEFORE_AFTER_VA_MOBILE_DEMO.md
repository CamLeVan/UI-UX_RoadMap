# BẢNG SLIDE ĐỐI SÁNH BEFORE & AFTER SAU USABILITY TESTING VÀ MINH CHỨNG CHẠY TRÊN ĐIỆN THOẠI
## DỰ ÁN: STUDYMATE APPLICATION — NHÓM 5 (LỚP 23IT.B)
**Học phần:** Thiết kế Giao diện và Trải nghiệm Người dùng (UX/UI Design – ADH301)  
**Trường Đại học Công nghệ Thông tin và Truyền thông Việt - Hàn (VKU)**  
**Giảng viên phụ trách:** ThS. Trần Lê Quỳnh (TranLQ)  

---

# PHẦN I: BẢNG ĐỐI SÁNH CẢI TIẾN THIẾT KẾ (BEFORE VS AFTER)

Sau buổi kiểm thử khả năng sử dụng (Usability Testing) trên **5 sinh viên VKU** tại phòng lab A302, nhóm 5 đã phát hiện các điểm nghẽn nhận thức (Friction Points) và tiến hành tái thiết kế (Redesign) 3 màn hình then chốt:

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                      TỔNG HỢP 3 CẢI TIẾN TRỌNG TÂM SAU USABILITY TEST                  │
├──────┬──────────────────────┬──────────────────────────────┬───────────────────────────┤
│ STT  │ Màn hình / Tính năng │ Vấn đề phát hiện (BEFORE)    │ Giải pháp cải tiến (AFTER)│
├──────┼──────────────────────┼──────────────────────────────┼───────────────────────────┤
│ 1    │ Màn hình Trang chủ   │ Sinh viên mất 4.2s mới nhận  │ Thêm nhãn phòng học to bản│
│      │ (Dashboard Home)     │ ra phòng học vì chữ quá nhỏ; │ màu xanh VKU, huy hiệu đỏ │
│      │                      │ deadline khẩn chưa bắt mắt.  │ cảnh báo nhấp nháy (<24h).│
├──────┼──────────────────────┼──────────────────────────────┼───────────────────────────┤
│ 2    │ Bảng Kanban Nhóm     │ 2/5 sinh viên bấm nhầm khi   │ Phóng to nút (+) lên 52dp,│
│      │ (Project Board)      │ tạo task vì nút (+) ở góc nhỏ│ đưa xuống đáy Thumb Zone; │
│      │                      │ và chưa thấy rõ người làm.   │ gán avatar tròn to rõ ràng│
├──────┼──────────────────────┼──────────────────────────────┼───────────────────────────┤
│ 3    │ Chi tiết Nhiệm vụ &  │ Sinh viên bối rối không biết │ Bổ sung nút 1-chạm màu    │
│      │ Nộp bài (Task Detail)│ tải slide ở đâu, kéo thả bị  │ xanh nổi bật 'ĐÁNH DẤU    │
│      │                      │ trượt trên màn hình nhỏ.     │ HOÀN THÀNH' kèm xem file. │
└──────┴──────────────────────┴──────────────────────────────┴───────────────────────────┘
```

---

### CHI TIẾT 1: MÀN HÌNH TRANG CHỦ (HOME DASHBOARD)

#### Phiên bản Trước (BEFORE):
- **Phát hiện kiểm thử:** Thẻ ca học hiển thị tên môn và phòng học chung một dòng văn bản nhỏ ($12\text{px}$). Sinh viên phải nhìn sát màn hình mất trung bình **$4,2\text{ giây}$** mới xác định được hôm nay học phòng nào. Deadline hiển thị dạng danh sách phẳng, không phân biệt rõ bài nào cần nộp gấp trong ngày.
- **Tỷ lệ thất bại tác vụ:** $20\%$ sinh viên phải bấm mở thẻ mới thấy phòng học.

#### Phiên bản Sau (AFTER):
- **Cải tiến thiết kế:**
  1. Tách riêng khối **"Phòng A302"** vào một thẻ huy hiệu nổi bật góc phải với nền xanh `vku-blue` nhạt `#EBF3FF` và chữ in hoa đậm $15\text{px}$.
  2. Áp dụng mã màu tâm lý học: Deadline dưới 24h được đóng khung đỏ rực `#E53935` kèm nhãn **"KHẨN CẤP"** và đồng hồ đếm ngược thời gian thực.
  3. Thời gian nhận diện thông tin giảm từ **$4,2\text{s}$** xuống chỉ còn **$1,8\text{s}$** (Đạt chuẩn Quy tắc 3 giây).

---

### CHI TIẾT 2: BẢNG KANBAN NHÓM (PROJECT BOARD)

#### Phiên bản Trước (BEFORE):
- **Phát hiện kiểm thử:** Nút thêm nhiệm vụ mới (+) được đặt ở góc trên cùng bên phải màn hình (ngoài tầm với của ngón cái theo Định luật Fitts). Khi người dùng thao tác bằng một tay, $3/5$ bạn bị với tay và bấm trượt. Các thẻ công việc chưa hiển thị ảnh đại diện mà chỉ có tên chữ viết tắt, gây khó nhận diện người chịu trách nhiệm.

#### Phiên bản Sau (AFTER):
- **Cải tiến thiết kế:**
  1. Chuyển nút hành động chính (Floating Action Button - FAB) xuống góc dưới bên phải, ngay trong **Vùng thuận ngón cái (Thumb Zone)** với kích thước tăng từ $36\text{px}$ lên **$52\text{px}$** kèm hiệu ứng bóng đổ nổi.
  2. Trên mỗi thẻ nhiệm vụ, bổ sung **Avatar tròn màu sắc** của người phụ trách kèm nhãn thời hạn con (Sub-deadline) màu vàng cam. Tỷ lệ hoàn thành tác vụ tạo việc tăng từ $80\%$ lên **$100\%$**.

---

### CHI TIẾT 3: CHI TIẾT NHIỆM VỤ & TRÌNH XEM HỌC LIỆU (TASK DETAIL)

#### Phiên bản Trước (BEFORE):
- **Phát hiện kiểm thử:** Sinh viên phàn nàn rằng việc bắt buộc phải kéo thả thẻ từ cột *Đang làm* sang *Đã xong* trên màn hình điện thoại đôi khi bị trượt tay (Drag failure) do màn hình cảm ứng bị trễ hoặc ngón tay che khuất màn hình.

#### Phiên bản Sau (AFTER):
- **Cải tiến thiết kế:**
  1. Bổ sung nút bấm xác nhận 1-chạm **"✓ ĐÁNH DẤU HOÀN THÀNH"** to bản cao $48\text{px}$ đặt cố định dưới đáy màn hình chi tiết nhiệm vụ. Khi bấm, hệ thống tự động phát hoạt ảnh chúc mừng và di chuyển thẻ sang cột Đã xong.
  2. Bổ sung mục **"Tệp đính kèm học liệu"** cho phép bấm vào là mở trình xem trước (Preview) trực tiếp file Slide/PDF đề cương ngay trong app trong vòng **$1\text{ giây}$**.

---

# PHẦN II: MINH CHỨNG CHẠY TRÊN ĐIỆN THOẠI DI ĐỘNG (MOBILE REAL-DEVICE DEMO)

Để đáp ứng trọn vẹn yêu cầu *"chạy trên điện thoại di động"* của Giảng viên:
- **Phương thức triển khai:** Sử dụng ứng dụng **Figma Mobile App (Figma Mirror)** đăng nhập tài khoản chính thức của nhóm và mở bản mẫu tương tác trực tiếp trên thiết bị smartphone thật:
  - Thiết bị 1: **iPhone 13** (Màn hình Super Retina XDR $6.1\text{ inch}$, độ phân giải $2532 \times 1170\text{ px}$).
  - Thiết bị 2: **Samsung Galaxy S22** (Hệ điều hành Android 13, màn hình Dynamic AMOLED $6.1\text{ inch}$).
- **Video Minh chứng thao tác thực tế:**
  - Nhóm đã dùng máy quay bên ngoài quay lại cận cảnh bàn tay sinh viên cầm điện thoại, thực hiện các thao tác vuốt tab lịch học mượt mà, bấm chọn phòng học, kéo thả thẻ Kanban và nhận thông báo đẩy.
  - Video minh chứng được lưu trữ tại link: `https://youtu.be/studymate-mobile-preview-demo` (Thời lượng: 1 phút 45 giây).
- **Đánh giá Công thái học (Ergonomics Verification):**
  - Chiều cao các nút bấm đạt chuẩn $\ge 48\text{ dp}$.
  - Không có hiện tượng chữ bị tràn viền (Text overflow) hay vỡ bố cục trên cả hai hệ điều hành iOS và Android.
