# Review & Completion Guide — Prompt Thiết kế Landing Page TLTS

## Đánh giá tổng quan

Prompt hiện tại đã ở mức rất tốt để sử dụng với:
- AI tạo giao diện: v0, Lovable, Bolt, Claude, ChatGPT
- Designer UI/UX
- Frontend Developer
- Team nội bộ triển khai landing page

Điểm mạnh:
- Brand guideline rõ ràng
- Quy định spacing/layout cụ thể
- UX flow hợp lý
- Có đầy đủ responsive + accessibility + performance
- Định nghĩa rõ từng section
- Có logic conditional render cho section thiếu dữ liệu

Mức độ hoàn thiện hiện tại: ~90–95%

---

# Các nội dung cần bổ sung trước khi dùng

## 1. Social Proof (Hero + Section 3)

### Hero social proof
Gợi ý:

- “Đã triển khai tại 15+ đơn vị · 500+ hồ sơ được xử lý”
- “99% hồ sơ được theo dõi tập trung trên hệ thống”
- “Rút ngắn 60% thời gian xử lý hồ sơ thanh lý”

### Social Proof Bar
Gợi ý:

- “15+ đơn vị · 500+ hồ sơ · 99% chính xác”
- “Toàn bộ dữ liệu thanh lý được đồng bộ SAP”

---

## 2. Screenshot cần chuẩn bị

Danh sách tối thiểu:

1. Dashboard tổng quan
2. Màn hình tạo đề xuất thanh lý
3. Màn hình thẩm định kỹ thuật
4. Màn hình thẩm định tài chính
5. Màn hình báo cáo
6. Timeline xử lý hồ sơ
7. Popup/chi tiết hồ sơ

Khuyến nghị:
- Chụp màn hình 1440px trở lên
- Ẩn dữ liệu nhạy cảm
- Dùng dữ liệu demo sạch
- Đồng bộ UI theme

---

## 3. Testimonials nội bộ

Nên chuẩn bị ít nhất 2–3 quote thật.

Ví dụ format:

> “Hệ thống giúp đơn vị chúng tôi giảm đáng kể thời gian xử lý hồ sơ và dễ dàng theo dõi trạng thái từng bước.”
>
> Nguyễn Văn A — Trưởng phòng Quản lý Tài sản

> “Việc đồng bộ SAP giúp giảm sai lệch dữ liệu và tăng tính minh bạch trong công tác thanh lý.”
>
> Trần Văn B — Phòng Tài chính

---

## 4. FAQ còn thiếu

### FAQ về cấp quyền

Q: Làm thế nào để được cấp quyền sử dụng hệ thống?

A: Cán bộ liên hệ quản trị viên đơn vị hoặc gửi yêu cầu tới bộ phận CNTT VTNet để được cấp tài khoản và phân quyền phù hợp.

### FAQ về bảo mật

Q: Dữ liệu trên hệ thống có được backup và bảo mật không?

A: Có. Dữ liệu được lưu trữ tập trung, backup định kỳ và phân quyền truy cập theo vai trò nhằm đảm bảo an toàn thông tin.

---

## 5. Section triển khai

Gợi ý nội dung:

### Phạm vi triển khai
- VTNet các khu vực
- Trung tâm Kỹ thuật
- Phòng Quản lý Tài sản
- Khối Tài chính

### SLA hỗ trợ
- Phản hồi trong 4 giờ làm việc
- Xử lý sự cố nghiêm trọng trong ngày
- Hỗ trợ qua hotline 1789 Nhánh 2

---

# Khuyến nghị kỹ thuật bổ sung

## 1. Ưu tiên stack đề xuất

### Khuyến nghị tốt nhất
React + Tailwind CSS + Framer Motion

Lý do:
- Nhanh
- Responsive tốt
- Dễ maintain
- Phù hợp AI-generated UI
- Dễ triển khai GitHub Pages/Vercel

---

## 2. Nên thêm Dark Section Contrast

Để landing page bớt phẳng:

- Hero: nền sáng
- Benefits: trắng
- Timeline: gray background
- Testimonials: dark background
- Final CTA: đỏ full-width

Hiện tại prompt đã khá đúng hướng.

---

## 3. Khuyến nghị animation

Nên giới hạn animation ở mức:
- Fade
- Slide nhẹ
- Hover scale nhỏ

Không dùng:
- Parallax nặng
- Particle background
- 3D animation
- Auto carousel khó kiểm soát

---

# Khuyến nghị UX/UI nâng cao

## 1. Sticky CTA Bar

Nên thêm:
- Nút “Truy cập hệ thống”
- Trạng thái online support
- Collapse animation

---

## 2. Hero Section

Nên thêm:
- Grid background cực nhẹ
- Red accent glow rất nhẹ phía sau screenshot
- Browser mockup thật

---

## 3. Benefit Cards

Hover nên gồm:
- Border đổi đỏ
- Accent bar animate width
- Shadow mềm

---

# Prompt bổ sung cho AI code generator

Có thể append thêm đoạn dưới vào cuối prompt nếu dùng Claude/v0/Lovable:

---

## YÊU CẦU OUTPUT

- Xuất toàn bộ landing page hoàn chỉnh
- Code production-ready
- Responsive đầy đủ
- Không dùng dữ liệu giả ngoài placeholder được chỉ định
- Tách component rõ ràng
- Semantic HTML chuẩn
- Tailwind CSS clean
- Không hardcode spacing sai hệ 8px
- Có animation nhẹ bằng Framer Motion
- Có sticky navbar + sticky CTA
- Có smooth scroll
- Có mobile menu
- Có lazy loading image
- Có dark/light contrast rõ ràng
- Tối ưu Lighthouse Performance >= 85
- Toàn bộ text hiển thị bằng tiếng Việt

Nếu thiếu hình ảnh thật:
- Tự động render placeholder block với label mô tả
- Không để broken image

---

# Gợi ý workflow triển khai nhanh

## Cách hiệu quả nhất hiện nay

### Bước 1
Paste prompt vào:
- Lovable
- v0
- Claude

### Bước 2
Sinh UI version đầu tiên

### Bước 3
Đưa sang:
- Cursor
- VSCode
- Windsurf

để refine component.

### Bước 4
Deploy:
- GitHub Pages
- Vercel
- Netlify

---

# Kết luận

Prompt hiện tại đã đủ mạnh để:
- Sinh landing page enterprise-grade
- Dùng trực tiếp cho AI code generator
- Bàn giao cho designer/frontend
- Chuẩn hóa UI theo brand Viettel Networks

Việc còn lại chủ yếu là:
1. Điền dữ liệu thật
2. Chuẩn bị screenshot
3. Bổ sung testimonials
4. Kiểm thử responsive/mobile
5. Deploy nội bộ

