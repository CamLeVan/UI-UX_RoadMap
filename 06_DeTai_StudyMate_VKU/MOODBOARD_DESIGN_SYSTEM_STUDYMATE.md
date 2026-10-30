# BẢN ĐẶC TẢ MOODBOARD & HỆ THỐNG THIẾT KẾ (DESIGN SYSTEM)
## DỰ ÁN: STUDYMATE APPLICATION — NHÓM 5 (LỚP 23IT.B)
**Học phần:** Thiết kế Giao diện và Trải nghiệm Người dùng (UX/UI Design – ADH301)  
**Trường Đại học Công nghệ Thông tin và Truyền thông Việt - Hàn (VKU)**  
**Giảng viên phụ trách:** ThS. Trần Lê Quỳnh  

---

## 1. KHÁI NIỆM & ĐỊNH HƯỚNG CẢM XÚC MOODBOARD (EMOTIONAL DESIGN)

Moodboard của **StudyMate** được xây dựng nhằm truyền tải 4 giá trị cảm xúc cốt lõi cho sinh viên VKU:
1. **Focus & Clarity (Tập trung & Tinh gọn):** Giao diện phẳng tối giản (Clean Modern Flat Design), không chi tiết thừa, triệt tiêu sự phân tâm.
2. **Academic & Trusted (Học thuật & Đáng tin cậy):** Lấy cảm hứng từ màu xanh nhận diện thương hiệu VKU kết hợp với chất liệu số hiện đại.
3. **Energetic & Motivating (Năng động & Thúc đẩy):** Điểm xuyết gam màu cam/vàng hổ phách tạo năng lượng hoàn thành deadline và học tập nhóm hăng say.
4. **Accessible & Ergonomic (Dễ tiếp cận & Công thái học):** Độ tương phản cao chuẩn WCAG 2.1 AA/AAA, tối ưu hóa vùng chạm di động cho ngón cái.

---

## 2. BẢNG MÀU NHẬN DIỆN THƯƠNG HIỆU (COLOR PALETTE & TOKENS)

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                        BẢNG MÃ MÀU THIẾT KẾ STUDYMATE (HEX & RGB)                      │
├────────────────────┬───────────┬───────────────────┬───────────────────────────────────┤
│ Phân loại màu      │ Tên Token │ Mã Màu (HEX)      │ Vai trò & Ý nghĩa giao diện       │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Primary (Chính)**│ `vku-blue`│ `#0052CC`         │ Màu xanh thương hiệu VKU. Dùng cho│
│                    │           │ RGB(0, 82, 204)   │ Header, CTA chính, Tab đang chọn. │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Secondary (Phụ)**│ `amber`   │ `#FF9900`         │ Màu cam/vàng bổ trợ VKU. Dùng cho │
│                    │           │ RGB(255, 153, 0)  │ Huy hiệu điểm số, thẻ deadline tuần│
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Semantic - Đỏ**  │ `danger`  │ `#E53935`         │ Cảnh báo deadline khẩn (<24h), lỗi│
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Semantic - Xanh**│ `success` │ `#2E7D32`         │ Thẻ đã hoàn thành (Done), an toàn │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Semantic - Vàng**│ `warning` │ `#F9A825`         │ Deadline sắp đến hạn (1-3 ngày)   │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Neutral - Nền**  │ `bg-page` │ `#F8FAFC`         │ Nền trang mềm dịu chống mỏi mắt   │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Neutral - Thẻ**  │ `bg-card` │ `#FFFFFF`         │ Nền các khối thẻ Card, Container  │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Neutral - Chữ**  │ `text-main`│ `#1E293B`        │ Màu chữ chính, độ tương phản 12:1 │
├────────────────────┼───────────┼───────────────────┼───────────────────────────────────┤
│ **Neutral - Mờ**   │ `text-sub`│ `#64748B`         │ Màu chú thích, ngày giờ, nhãn phụ │
└────────────────────┴───────────┴───────────────────┴───────────────────────────────────┘
```

---

## 3. QUY CHUẨN KIỂU CHỮ (TYPOGRAPHY HIERARCHY)

Dự án sử dụng bộ font **Inter** (Google Font mã nguồn mở) tối ưu hóa độ sắc nét cho màn hình cảm ứng di động:

| Cấp bậc (Level) | Cỡ chữ (Size) | Độ đậm (Weight) | Chiều cao dòng (Line-height) | Trường hợp sử dụng trên màn hình |
|:---|:---:|:---:|:---:|:---|
| **Display 1** | `28px` | Bold (700) | `36px` | Tiêu đề lớn màn hình Chào mừng (Welcome) |
| **Heading 1** | `22px` | SemiBold (600) | `28px` | Tiêu đề màn hình chính (Dashboard, Lịch học) |
| **Heading 2** | `18px` | SemiBold (600) | `24px` | Tên môn học, Tên cột Kanban (To Do / Doing) |
| **Subheading** | `15px` | Medium (500) | `20px` | Tên thẻ công việc, Tên người phụ trách |
| **Body Text** | `14px` | Regular (400) | `20px` | Nội dung mô tả nhiệm vụ, văn bản thông báo |
| **Caption / Tag** | `12px` | Medium (500) | `16px` | Nhãn deadline, thời gian ca học, phòng A302 |
| **Micro Text** | `10px` | SemiBold (600) | `12px` | Huy hiệu số thông báo đỏ trên icon |

---

## 4. HỆ THỐNG BIỂU TƯỢNG & ĐỒ HỌA CẢM HỨNG (ICONOGRAPHY & VISUAL MOTIFS)

- **Bộ Icon chuẩn:** Sử dụng **Phosphor Icons** / **Lucide Icons** nét mảnh $1.5\text{px}$, bo góc nhẹ nhàng:
  - 📅 **Calendar:** Biểu tượng lịch học phân ca rõ ràng.
  - 📋 **Kanban Columns:** Biểu tượng 3 cột luồng công việc nhóm.
  - 🔔 **Bell Notification:** Chuông nhắc deadline kèm chấm đỏ động.
  - 📎 **Paperclip:** Đính kèm slide bài giảng và tệp đề cương.
  - 👤 **Avatar Circle:** Huy hiệu người phụ trách công việc nhóm.
- **Phong cách Bo góc (Border Radius):**
  - Thẻ Card & Container: `rounded-2xl` ($16\text{px}$) tạo cảm giác thân thiện, mềm mại.
  - Nút bấm (Buttons): `rounded-xl` ($12\text{px}$) tạo điểm bấm rõ ràng.
  - Huy hiệu (Badges): `rounded-full` ($9999\text{px}$) kiểu viên thuốc (Pill shape).
- **Hiệu ứng Đổ bóng (Elevation & Shadows):**
  - Card Shadow: `0px 4px 20px rgba(0, 82, 204, 0.06)` – Đổ bóng xanh nhẹ tạo độ nổi tinh tế mà không bị thô cứng.

---

## 5. HỆ THỐNG THÀNH PHẦN GIAO DIỆN MẪU (UI COMPONENTS KIT)

1. **Buttons (Nút bấm):**
   - *Primary CTA:* Nền xanh `#0052CC`, chữ trắng, bo góc 12px, chiều cao đạt chuẩn $48\text{px}$ cho ngón cái.
   - *Secondary:* Viền xanh `1.5px`, nền trắng, chữ xanh `#0052CC`.
   - *Danger / Warning:* Nền đỏ nhạt `#FEE2E2`, chữ đỏ đậm `#DC2626`.
2. **Task Cards (Thẻ công việc Kanban):**
   - Nền trắng `#FFFFFF`, viền mờ `#E2E8F0`, chứa tên việc, thanh tiến độ mini, nhãn deadline và ảnh đại diện thành viên.
3. **Bottom Navigation Bar:**
   - Cố định dưới chân màn hình, chiều cao $64\text{px}$, hiệu ứng đổ bóng mờ, khoảng cách icon tối thiểu $48\text{px}$ chống bấm nhầm.

---

## HƯỚNG DẪN XUẤT RA FILE PDF NỘP CHO GIẢNG VIÊN
Nhóm mở file Figma thiết kế Moodboard, chọn Frame **Moodboard & UI Kit (1920x1080)** và nhấn `Ctrl + Shift + E` (Export as PDF) để nộp vào Cột 2 theo quy định.
