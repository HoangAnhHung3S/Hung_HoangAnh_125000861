# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)

- **Họ và tên**: Hoàng Anh Hùng
- **MSSV:** 125000861
- **Tên đề tài Website:** Landing Page Cửa Hàng Gaming Gear (CyberGear)
- **Công cụ AI đã sử dụng:** GitHub Copilot / AI Assistant

## 1. Yêu cầu ban đầu (System/Initial Prompt)
> "Hãy giúp tôi tạo mã nguồn cho một website Landing Page bán thiết bị Gaming Gear (CyberGear - chuột, bàn phím cơ, tai nghe). Website cần đáp ứng chuẩn Semantic HTML5 (tối thiểu 5 thành phần: `<header>`, `<nav>`, `<main>`, `<section>` hoặc `<article>`, `<footer>`). Quản lý phối màu Cyberpunk/Dark mode và font chữ bằng CSS Variables (`:root`). Giao diện responsive tốt trên cả mobile và desktop. Chỉ sử dụng Html và css tuyệt đối không sử dụng thêm thứ gì khác."

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)

### Lần 1: Cấu trúc Semantic HTML & Bố cục cơ bản
- **Prompt đã dùng:** 
  > "Trong index.html, tạo cấu trúc gồm: Header (logo CYBERGEAR + menu navigation), Hero section, Section Danh mục sản phẩm, Section Sản phẩm bán chạy dùng thẻ `<article>`, Section Đăng ký nhận khuyến mãi và Footer. Trong style.css, sử dụng `:root` để định nghĩa các biến màu Gaming Dark Mode (`--primary-color: #00ff88`, `--bg-color: #0d0f12`) và dàn trang bằng Flexbox, Grid."
- **Kết quả AI tạo ra:** Tạo khung Semantic HTML5 hoàn chỉnh với các thẻ theo yêu cầu, áp dụng file `style.css` thuần không dùng thư viện ngoài hay JavaScript.
- **Nhận xét & Tinh chỉnh của SV:** Đã kiểm tra cấu trúc phân tầng các section và bổ sung thêm các mục điều hướng rõ ràng cho menu.

### Lần 2: Tích hợp thư viện hiệu ứng động (Animate.css & AOS)
- **Prompt đã dùng:** 
  > "Hãy tích hợp CDN của Animate.css và AOS vào file index.html. Áp dụng hiệu ứng `animate__fadeInDown` cho tiêu đề chính H1 ở Hero section, và thêm thuộc tính `data-aos="fade-up"` (hoặc `fade-right`) cho các section nội dung và các thẻ sản phẩm. Đừng quên thêm đoạn mã script `AOS.init()` ở cuối thẻ `</body>`."
- **Kết quả AI tạo ra:** Chèn các CDN chuẩn, gắn class hiệu ứng vào tiêu đề chính và các thẻ sản phẩm kèm script khởi tạo AOS.
- **Nhận xét & Tinh chỉnh của SV:** Hiệu ứng cuộn trang hoạt động mượt mà khi người dùng tương tác trượt xuống các khối nội dung.

### Lần 3: Tinh chỉnh hiệu ứng Hover/Focus, Nhãn Badge và Form
- **Prompt đã dùng:** 
  > "Hãy viết thêm hiệu ứng `:hover` và `:focus` trong style.css cho nút bấm (`.btn-primary`, `.btn-small`) và các thẻ bài viết (`.card`). Khi hover vào thẻ sản phẩm thì nổi nhẹ lên (`transform: translateY(-8px)`), đổi màu viền sang xanh Neon (`#00ff88`) và đổ bóng. Thêm nhãn Hot/Sale (`.badge`) ở góc thẻ sản phẩm và style lại Form đăng ký thông tin."
- **Kết quả AI tạo ra:** Bổ sung các trạng thái tương tác hover/focus trực quan, thêm nhãn `HOT`, `SALE` bắt mắt và hoàn thiện giao diện form nhập thông tin.
- **Nhận xét & Tinh chỉnh của SV:** Giao diện mang đậm phong cách Cyberpunk, các hiệu ứng chuyển động mượt và hiển thị chuẩn trên mọi kích thước màn hình.   