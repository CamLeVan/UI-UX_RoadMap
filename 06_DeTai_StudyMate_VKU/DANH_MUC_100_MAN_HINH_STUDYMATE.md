# BẢNG TỔNG MỤC 100 MÀN HÌNH THIẾT KẾ (SCREEN INVENTORY) — ĐỒ ÁN STUDYMATE
## TRÍCH XUẤT CHÍNH XÁC 100% TỪ FILE FIGMA CỦA NHÓM (FIGMA REST API)
**Học phần:** Thiết kế Giao diện và Trải nghiệm Người dùng (UX/UI Design – ADH301)  
**Trường Đại học Công nghệ Thông tin và Truyền thông Việt - Hàn (VKU)**  
**Lớp sinh hoạt:** 23IT.B | **Nhóm 5:** Lê Văn Cảm, Nguyễn Văn Quốc Triệu, Nguyễn Danh Linh, Nguyễn Đình Hoàng Nguyên, Nguyễn Đức Minh Nghĩa  

---

## TỔNG QUAN PHÂN BỔ 100 MÀN HÌNH

Hệ sinh thái StudyMate đã được thiết kế đầy đủ **100 màn hình (chuẩn tỷ lệ iPhone 375x812px)** bao gồm 2 phân hệ phân quyền:
- **Phân hệ Sinh viên (User Role):** 60 màn hình (Từ Screen #1 đến Screen #60).
- **Phân hệ Quản trị viên (Admin Role):** 40 màn hình (Từ Screen #61 đến Screen #100).

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                        CƠ CẤU 100 MÀN HÌNH TRONG FILE FIGMA STUDYMATE                  │
├──────┬──────────────────────────────────────────┬───────────┬──────────────────────────┤
│ Cụm  │ Tên Nhóm Luồng Chức Năng                 │ Số Màn    │ Số Hiệu Màn Hình (ID)    │
├──────┼──────────────────────────────────────────┼───────────┼──────────────────────────┤
│ **1**│ Luồng Chính Sinh viên (Core Flow)        │ 18 màn    │ Screen #1  → Screen #18  │
│ **2**│ Đăng ký & Xác thực Tài khoản             │ 6 màn     │ Screen #19 → Screen #24  │
│ **3**│ Lịch học & Lịch thi Tín chỉ              │ 6 màn     │ Screen #25 → Screen #30  │
│ **4**│ Nhóm & Cộng tác Đồ án                    │ 7 màn     │ Screen #31 → Screen #37  │
│ **5**│ Nhiệm vụ & Deadline Kanban               │ 6 màn     │ Screen #38 → Screen #43  │
│ **6**│ Kho Tài liệu & Tìm kiếm Học liệu         │ 6 màn     │ Screen #44 → Screen #49  │
│ **7**│ Cá nhân, Cài đặt & Tùy biến              │ 7 màn     │ Screen #50 → Screen #56  │
│ **8**│ Trợ giúp & Trạng thái Hệ thống (Empty/Err│ 4 màn     │ Screen #57 → Screen #60  │
├──────┼──────────────────────────────────────────┼───────────┼──────────────────────────┤
│ **9**│ Admin: Đăng nhập, 2FA & Dashboard        │ 6 màn     │ Screen #61 → Screen #66  │
│**10**│ Admin: Quản lý Người dùng & Phân quyền   │ 7 màn     │ Screen #67 → Screen #73  │
│**11**│ Admin: Học vụ, Môn học & Thời khóa biểu  │ 7 màn     │ Screen #74 → Screen #80  │
│**12**│ Admin: Quản lý Lịch thi, Nhóm & Tài liệu │ 7 màn     │ Screen #81 → Screen #87  │
│**13**│ Admin: Thông báo, Phản hồi & Nhật ký     │ 6 màn     │ Screen #88 → Screen #93  │
│**14**│ Admin: Cài đặt Hệ thống, SSO & Sao lưu   │ 7 màn     │ Screen #94 → Screen #100 │
├──────┴──────────────────────────────────────────┴───────────┴──────────────────────────┤
│ **TỔNG CỘNG ĐÃ CÓ TRÊN FIGMA:** **100 / 100 MÀN HÌNH HOÀN TOÀN TRÙNG KHỚP!**           │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## DANH MỤC CHI TIẾT TỪ MÀN HÌNH 1 ĐẾN MÀN HÌNH 100

### PHẦN I: PHÂN HỆ SINH VIÊN (USER ROLE) — 60 MÀN HÌNH

#### Cụm 1: Luồng chính sinh viên (Group 1 - 18 màn hình)
- `Screen #1`: **1 Splash** (id: `2:4`)
- `Screen #2`: **2 Đăng nhập SSO** (id: `2:15`)
- `Screen #3`: **3 Trang chủ** (id: `2:40`)
- `Screen #4`: **4 Lịch học tuần** (id: `2:94`)
- `Screen #5`: **5 Kanban nhóm** (id: `2:155`)
- `Screen #6`: **6 Thêm nhiệm vụ** (id: `2:213`)
- `Screen #7`: **7 Chi tiết nhiệm vụ** (id: `2:250`)
- `Screen #8`: **8 Thư viện tài liệu** (id: `2:289`)
- `Screen #9`: **9 Onboarding** (id: `4:4`)
- `Screen #10`: **10 Danh sách nhóm** (id: `4:22`)
- `Screen #11`: **11 Tham gia nhóm** (id: `4:67`)
- `Screen #12`: **12 Danh sách deadline** (id: `4:91`)
- `Screen #13`: **13 Chi tiết môn học** (id: `4:141`)
- `Screen #14`: **14 Xem trước tệp** (id: `4:194`)
- `Screen #15`: **15 Thành viên nhóm** (id: `4:216`)
- `Screen #16`: **16 Kanban sau hoàn thành** (id: `4:285`)
- `Screen #17`: **17 Thông báo** (id: `4:345`)
- `Screen #18`: **18 Cá nhân** (id: `4:381`)

#### Cụm 2: Đăng ký & Xác thực (6 màn hình)
- `Screen #19`: **19 Đăng ký tài khoản** (id: `29:2140`)
- `Screen #20`: **20 Quên mật khẩu** (id: `29:2177`)
- `Screen #21`: **21 Nhập mã OTP** (id: `29:2196`)
- `Screen #22`: **22 Đặt lại mật khẩu** (id: `29:2225`)
- `Screen #23`: **23 Bảo mật FaceID & 2 lớp** (id: `29:2256`)
- `Screen #24`: **24 Hoàn tất hồ sơ** (id: `29:2281`)

#### Cụm 3: Lịch học & Lịch thi (6 màn hình)
- `Screen #25`: **25 Lịch học · Xem tháng** (id: `29:2311`)
- `Screen #26`: **26 Chi tiết buổi học** (id: `29:2479`)
- `Screen #27`: **27 Thêm lịch cá nhân** (id: `29:2513`)
- `Screen #28`: **28 Lịch thi** (id: `29:2557`)
- `Screen #29`: **29 Chi tiết lịch thi** (id: `29:2605`)
- `Screen #30`: **30 Nhắc lịch học & thi** (id: `29:2643`)

#### Cụm 4: Nhóm & Cộng tác (7 màn hình)
- `Screen #31`: **31 Tạo nhóm mới** (id: `29:2687`)
- `Screen #32`: **32 Mã mời nhóm** (id: `29:2720`)
- `Screen #33`: **33 Cài đặt nhóm** (id: `29:2745`)
- `Screen #34`: **34 Hoạt động nhóm** (id: `29:2782`)
- `Screen #35`: **35 Chat nhóm** (id: `29:2833`)
- `Screen #36`: **36 Báo cáo tiến độ** (id: `29:2863`)
- `Screen #37`: **37 Xác nhận rời nhóm** (id: `29:2952`)

#### Cụm 5: Nhiệm vụ (6 màn hình)
- `Screen #38`: **38 Chỉnh sửa nhiệm vụ** (id: `29:3003`)
- `Screen #39`: **39 Bình luận nhiệm vụ** (id: `29:3045`)
- `Screen #40`: **40 Nộp bản nháp** (id: `29:3078`)
- `Screen #41`: **41 Xác nhận xóa việc** (id: `29:3107`)
- `Screen #42`: **42 Lọc nhiệm vụ** (id: `29:3144`)
- `Screen #43`: **43 Việc của tôi** (id: `29:3186`)

#### Cụm 6: Tài liệu & Tìm kiếm (6 màn hình)
- `Screen #44`: **44 Danh sách tệp trong thư mục** (id: `29:3239`)
- `Screen #45`: **45 Tải tệp lên** (id: `29:3293`)
- `Screen #46`: **46 Tài liệu đã lưu** (id: `29:3326`)
- `Screen #47`: **47 Kết quả tìm kiếm** (id: `29:3384`)
- `Screen #48`: **48 Tìm kiếm toàn cục** (id: `29:3429`)
- `Screen #49`: **49 Chia sẻ tài liệu** (id: `29:3474`)

#### Cụm 7: Cá nhân & Cài đặt (7 màn hình)
- `Screen #50`: **50 Thông tin cá nhân** (id: `29:3517`)
- `Screen #51`: **51 Chỉnh sửa hồ sơ** (id: `29:3553`)
- `Screen #52`: **52 Môn học đã đăng ký** (id: `29:3587`)
- `Screen #53`: **53 Cài đặt nhắc việc** (id: `29:3637`)
- `Screen #54`: **54 Đổi mật khẩu** (id: `29:3678`)
- `Screen #55`: **55 Ngôn ngữ & giao diện** (id: `29:3713`)
- `Screen #56`: **56 Xác nhận đăng xuất** (id: `29:3756`)

#### Cụm 8: Trợ giúp & Trạng thái hệ thống (4 màn hình)
- `Screen #57`: **57 Trợ giúp & hỗ trợ** (id: `29:3819`)
- `Screen #58`: **58 Gửi phản hồi** (id: `29:3868`)
- `Screen #59`: **59 Mất kết nối mạng (Error/Offline)** (id: `29:3900`)
- `Screen #60`: **60 Trạng thái trống · Chưa có nhóm (Empty State)** (id: `29:3936`)

---

### PHẦN II: PHÂN HỆ QUẢN TRỊ VIÊN (ADMIN ROLE) — 40 MÀN HÌNH

#### Cụm 9: Đăng nhập & Tổng quan (6 màn hình)
- `Screen #61`: **61 Admin · Đăng nhập** (id: `29:8`)
- `Screen #62`: **62 Admin · Xác thực 2 lớp** (id: `29:35`)
- `Screen #63`: **63 Admin · Quên mật khẩu** (id: `29:66`)
- `Screen #64`: **64 Admin · Dashboard** (id: `29:88`)
- `Screen #65`: **65 Admin · Báo cáo thống kê** (id: `29:165`)
- `Screen #66`: **66 Admin · Xuất báo cáo** (id: `29:243`)

#### Cụm 10: Quản lý Người dùng (7 màn hình)
- `Screen #67`: **67 Admin · Danh sách người dùng** (id: `29:288`)
- `Screen #68`: **68 Admin · Chi tiết người dùng** (id: `29:357`)
- `Screen #69`: **69 Admin · Thêm/sửa người dùng** (id: `29:395`)
- `Screen #70`: **70 Admin · Nhập danh sách CSV** (id: `29:436`)
- `Screen #71`: **71 Admin · Phân quyền** (id: `29:485`)
- `Screen #72`: **72 Admin · Xác nhận khóa tài khoản** (id: `29:525`)
- `Screen #73`: **73 Admin · Lọc người dùng** (id: `29:566`)

#### Cụm 11: Học vụ, Môn học & Thời khóa biểu (7 màn hình)
- `Screen #74`: **74 Admin · Danh sách môn học** (id: `29:609`)
- `Screen #75`: **75 Admin · Thêm môn học** (id: `29:669`)
- `Screen #76`: **76 Admin · Chi tiết môn học** (id: `29:707`)
- `Screen #77`: **77 Admin · Gán giảng viên** (id: `29:751`)
- `Screen #78`: **78 Admin · Lớp học phần** (id: `29:789`)
- `Screen #79`: **79 Admin · Thời khóa biểu** (id: `29:849`)
- `Screen #80`: **80 Admin · Thêm/sửa buổi học** (id: `29:900`)

#### Cụm 12: Lịch thi, Nhóm & Tài liệu (7 màn hình)
- `Screen #81`: **81 Admin · Quản lý lịch thi** (id: `29:947`)
- `Screen #82`: **82 Admin · Danh sách nhóm** (id: `29:999`)
- `Screen #83`: **83 Admin · Chi tiết nhóm** (id: `29:1059`)
- `Screen #84`: **84 Admin · Xác nhận giải tán nhóm** (id: `29:1109`)
- `Screen #85`: **85 Admin · Quản lý tài liệu** (id: `29:1153`)
- `Screen #86`: **86 Admin · Kiểm duyệt tài liệu** (id: `29:1210`)
- `Screen #87`: **87 Admin · Dung lượng lưu trữ** (id: `29:1243`)

#### Cụm 13: Thông báo & Phản hồi (6 màn hình)
- `Screen #88`: **88 Admin · Gửi thông báo** (id: `29:1313`)
- `Screen #89`: **89 Admin · Lịch sử thông báo** (id: `29:1366`)
- `Screen #90`: **90 Admin · Mẫu thông báo** (id: `29:1420`)
- `Screen #91`: **91 Admin · Danh sách phản hồi** (id: `29:1457`)
- `Screen #92`: **92 Admin · Chi tiết phản hồi** (id: `29:1514`)
- `Screen #93`: **93 Admin · Nhật ký hoạt động** (id: `29:1547`)

#### Cụm 14: Hệ thống & Tài khoản Quản trị (7 màn hình)
- `Screen #94`: **94 Admin · Cài đặt hệ thống** (id: `29:1603`)
- `Screen #95`: **95 Admin · Đồng bộ SSO** (id: `29:1657`)
- `Screen #96`: **96 Admin · Sao lưu & khôi phục** (id: `29:1695`)
- `Screen #97`: **97 Admin · Quản lý quản trị viên** (id: `29:1738`)
- `Screen #98`: **98 Admin · Hồ sơ quản trị** (id: `29:1779`)
- `Screen #99`: **99 Admin · Đổi mật khẩu** (id: `29:1834`)
- `Screen #100`: **100 Admin · Xác nhận đăng xuất** (id: `29:1871`)
