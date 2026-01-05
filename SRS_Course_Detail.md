# Software Requirements Specification (SRS)
## Trang Chi Tiết Khóa Học - Rikkei Education

---

## 1. Giới thiệu

### 1.1 Mục đích
Tạo trang chi tiết khóa học hiển thị đầy đủ thông tin về một khóa học cụ thể, bao gồm nội dung học, giảng viên, giá cả, đánh giá và các thông tin liên quan để giúp học viên đưa ra quyết định đăng ký.

### 1.2 Đối tượng sử dụng
- Học viên tiềm năng muốn tìm hiểu chi tiết về khóa học trước khi đăng ký
- Học viên đã đăng ký muốn xem lại thông tin khóa học
- Người muốn so sánh các khóa học khác nhau

### 1.3 Giới hạn
- Website chỉ sử dụng HTML và CSS thuần túy, không sử dụng JavaScript
- Không có chức năng đăng ký thực tế (chỉ giao diện)
- Video preview và curriculum sections không có chức năng mở rộng/thu gọn động
- Nút "Thêm vào giỏ hàng" chỉ là giao diện
- Form đánh giá và bình luận không có chức năng thực tế

### 1.4 Phạm vi dự án
Trang chi tiết khóa học bao gồm đầy đủ các thông tin: header, breadcrumb, course header, pricing card, learning outcomes, mô tả, curriculum, yêu cầu, đối tượng, giảng viên, đánh giá, sidebar và footer.

---

## 2. Mô tả hệ thống

### 2.1 Cấu trúc trang chi tiết khóa học

#### 2.1.1 Header (Thanh điều hướng)
- Logo Rikkei Education (link về trang chủ)
- Menu điều hướng với anchor links về trang chủ
- Nút Đăng nhập và Đăng ký

#### 2.1.2 Breadcrumb Navigation
- Đường dẫn: Trang chủ > Khóa học > [Tên khóa học]
- Giúp người dùng biết vị trí hiện tại
- Links để quay lại trang trước

#### 2.1.3 Course Header (Banner tối)
**Phần trái:**
- Badge group: "Bán chạy nhất" + "Lập trình"
- Tiêu đề khóa học: "Lập Trình Web Từ Cơ Bản Đến Nâng Cao"
- Subtitle: Mô tả ngắn về khóa học
- Meta information:
  - Đánh giá: 4.9⭐ (2,345 đánh giá)
  - Số học viên: 12,567
  - Ngày cập nhật: Tháng 12/2025
  - Ngôn ngữ: Tiếng Việt
- Thông tin giảng viên mini (avatar + tên)

**Phần phải:**
- Preview card (sticky khi scroll)

#### 2.1.4 Course Preview Card (Sticky Sidebar)
**Hình ảnh:**
- Thumbnail khóa học
- Play overlay với icon và text "Xem giới thiệu"

**Pricing Section:**
- Giá hiện tại: 1,999,000đ
- Giá cũ: 2,999,000đ (gạch ngang)
- Badge giảm giá: "Giảm 33%"
- Thông báo thời gian: "Ưu đãi kết thúc sau 2 ngày"

**Call-to-Action:**
- Nút "Đăng ký ngay" (primary)
- Nút "Thêm vào giỏ hàng" (outline)

**Khóa học bao gồm:**
- 40 giờ video học
- 25 bài tập thực hành
- Truy cập trên mọi thiết bị
- Truy cập trọn đời
- Chứng chỉ hoàn thành
- Hỗ trợ 24/7

**Guarantee:**
- "Hoàn tiền 100% trong 30 ngày"

#### 2.1.5 Main Content Area

**A. Bạn sẽ học được gì**
- 8 learning outcomes với checkmark icons
- Layout 2 cột trên desktop
- Nội dung:
  - Nắm vững HTML5 và CSS3
  - Lập trình JavaScript
  - Sử dụng React.js
  - Thiết kế responsive
  - Làm việc với API
  - Triển khai website
  - Xây dựng 5+ dự án
  - Best practices

**B. Mô tả khóa học**
- Giới thiệu tổng quan
- Đoạn chào mừng
- Lý do nên chọn khóa học (5 điểm)
- Kết quả sau khóa học (4 điểm)
- Call-to-action cuối

**C. Nội dung khóa học (Curriculum)**
- Thống kê: 8 phần • 67 bài học • 40 giờ học
- 8 sections với cấu trúc:
  - Section header: Icon dropdown + Tên phần + Số bài & thời lượng
  - Section 1 được expand với 6 lectures chi tiết:
    - Icon (▶️ video hoặc 📝 bài tập)
    - Tên bài học
    - Thời lượng
  - Sections 2-8 chỉ hiển thị header

**Danh sách 8 phần:**
1. Giới thiệu và Cơ bản HTML (8 bài • 3 giờ)
2. CSS Cơ Bản và Nâng Cao (10 bài • 5 giờ)
3. Responsive Design (7 bài • 4 giờ)
4. JavaScript Cơ Bản (12 bài • 6 giờ)
5. JavaScript Nâng Cao (10 bài • 5.5 giờ)
6. React.js Fundamentals (12 bài • 7 giờ)
7. Làm việc với API (6 bài • 4 giờ)
8. Dự Án Cuối Khóa và Triển Khai (8 bài • 5.5 giờ)

**D. Yêu cầu**
- Máy tính có kết nối internet
- Không cần kiến thức lập trình trước đó
- Tinh thần học hỏi và sẵn sàng thực hành
- Cam kết dành ít nhất 5-10 giờ/tuần để học

**E. Khóa học dành cho ai**
- Người mới bắt đầu muốn học lập trình web
- Sinh viên ngành CNTT muốn nâng cao kỹ năng
- Người muốn chuyển nghề sang lập trình
- Freelancer muốn mở rộng dịch vụ
- Designer muốn học code để tự implement design

**F. Giảng viên**
- Avatar (150x150px)
- Tên: Nguyễn Văn A
- Chức danh: Senior Full-stack Developer
- Thống kê:
  - 4.9⭐ Đánh giá
  - 45,678 Học viên
  - 15 Khóa học
- Tiểu sử (3 đoạn):
  - Kinh nghiệm 10+ năm
  - Đào tạo 45,000+ học viên
  - Chuyên môn: JavaScript, React.js, Node.js, MongoDB, AWS, Docker

**G. Đánh giá từ học viên**

*Rating Overview:*
- Điểm trung bình: 4.9/5
- Số lượng: 2,345 đánh giá
- Hiển thị 5 sao

*Rating Breakdown:*
- 5 sao: 85% (progress bar)
- 4 sao: 12%
- 3 sao: 2%
- 2 sao: 1%
- 1 sao: 0%

*Reviews List (3 reviews):*
1. **Trần Thị B** - 5⭐ - 2 tuần trước
   - Nội dung: Khóa học chi tiết, giảng viên rõ ràng, đáng tiền
   - Helpful: 👍 Có (234)

2. **Lê Văn C** - 5⭐ - 1 tháng trước
   - Nội dung: Chuyển nghề thành công, apply được Junior Developer
   - Helpful: 👍 Có (189)

3. **Phạm Thị D** - 5⭐ - 1 tháng trước
   - Nội dung: Support tốt, làm được 3 dự án, đang freelance
   - Helpful: 👍 Có (156)

- Nút "Xem thêm đánh giá"

#### 2.1.6 Sidebar

**A. Khóa học liên quan**
3 khóa học với:
- Thumbnail (100x60px)
- Tên khóa học
- Rating (⭐ 4.8)
- Giá (1,699,000đ)

Danh sách:
1. UI/UX Design Chuyên Nghiệp - 4.8⭐ - 1,699,000đ
2. Phát Triển Ứng Dụng Di Động - 4.7⭐ - 2,299,000đ
3. Machine Learning Cơ Bản - 4.9⭐ - 2,799,000đ

**B. Chia sẻ khóa học**
4 nút chia sẻ:
- Facebook (màu #1877f2)
- Twitter (màu #1da1f2)
- LinkedIn (màu #0a66c2)
- Sao chép link (màu xám)

#### 2.1.7 Footer
- Logo Rikkei Education
- Mô tả ngắn
- Social media links
- 3 cột menu (Khóa học, Về chúng tôi, Hỗ trợ)
- Copyright

---

## 3. Yêu cầu hệ thống

### 3.1 Yêu cầu phần cứng
- Thiết bị có khả năng truy cập internet
- Màn hình tối thiểu 320px (mobile) đến 1920px+ (desktop)

### 3.2 Yêu cầu phần mềm
- Trình duyệt web hiện đại:
  - Google Chrome (90+)
  - Mozilla Firefox (88+)
  - Safari (14+)
  - Microsoft Edge (90+)

### 3.3 Công nghệ sử dụng
- **HTML5**: Cấu trúc semantic
- **CSS3**: Styling và responsive
  - CSS Variables
  - Flexbox và Grid Layout
  - Media Queries
  - CSS Transitions
  - Sticky positioning

### 3.4 Dependencies
- File `style.css` - Base styles từ trang chủ
- File `course-detail.css` - Styles riêng cho trang chi tiết

---

## 4. Thiết kế giao diện

### 4.1 Layout Structure
- **Container**: Max-width 1200px
- **Main Layout**: 2 columns
  - Main content: Flex 1
  - Sidebar: 350px (sticky)

### 4.2 Hệ thống màu sắc
Kế thừa từ trang chủ:
- Primary: #6366f1
- Secondary: #ec4899
- Accent: #f59e0b
- Text Dark: #1f2937
- Text Light: #6b7280
- Background: #ffffff, #f9fafb, #f3f4f6

**Màu bổ sung cho trang chi tiết:**
- Course Header Background: #1f2937 (dark)
- Success Green: #16a34a (checkmarks, guarantee)
- Warning Yellow: #fef3c7 (time remaining background)
- Discount Green: #dcfce7 background, #166534 text

### 4.3 Typography
- Hero Title: 2.5rem (40px)
- Section Heading: 1.75rem (28px)
- Subsection Heading: 1.5rem (24px)
- Body Text: 1rem (16px)
- Small Text: 0.875rem (14px)

### 4.4 Spacing
Sử dụng hệ thống spacing từ base:
- XS: 0.5rem, SM: 1rem, MD: 1.5rem
- LG: 2rem, XL: 3rem, 2XL: 4rem

### 4.5 Components Styling

**Breadcrumb:**
- Background: #f9fafb
- Border bottom: 1px solid #e5e7eb
- Separator: "›"

**Course Header:**
- Background: #1f2937 (dark)
- Text: White
- Padding: 3rem 0

**Preview Card:**
- Background: White
- Border radius: 0.75rem
- Box shadow: XL
- Sticky top: 80px

**Badges:**
- Bestseller: #f59e0b background
- Category: rgba(255,255,255,0.15) background
- Discount: #dcfce7 background, #166534 text

**Buttons:**
- Primary: #6366f1 background
- Outline: Transparent background, #6366f1 border
- Block: width 100%
- Large: 0.875rem 2rem padding

**Content Boxes:**
- Background: White
- Padding: 3rem
- Border radius: 0.75rem
- Box shadow: SM

**Curriculum Sections:**
- Border: 1px solid #e5e7eb
- Header background: #f9fafb
- Hover: #f3f4f6

**Rating Bars:**
- Background: #f3f4f6
- Fill: #f59e0b
- Height: 8px

**Share Buttons:**
- Facebook: #1877f2
- Twitter: #1da1f2
- LinkedIn: #0a66c2
- Copy: #f3f4f6

### 4.6 Responsive Breakpoints

**Desktop (>1024px):**
- 2-column layout (main + sidebar)
- Sticky preview card
- 2-column learning outcomes
- 2-column rating summary

**Tablet (768px - 1024px):**
- Single column layout
- Preview card static (not sticky)
- Single column learning outcomes
- Single column rating summary

**Mobile (<768px):**
- All single column
- Reduced padding
- Smaller font sizes
- Stacked buttons
- Collapsed instructor header

---

## 5. Triển khai

### 5.1 Môi trường phát triển
- **IDE**: Visual Studio Code
- **Extensions**: Live Server, HTML CSS Support, Prettier
- **Browser DevTools**: Chrome DevTools

### 5.2 Cấu trúc files
```
demo/
├── index.html              # Trang chủ
├── course-detail.html      # Trang chi tiết khóa học
├── style.css               # Base styles
├── course-detail.css       # Course detail specific styles
└── SRS_Course_Detail.md    # Tài liệu này
```

### 5.3 Linking Strategy
- `course-detail.html` import cả `style.css` và `course-detail.css`
- Logo và breadcrumb links về `index.html`
- Menu navigation links về các sections trong `index.html` (với #anchors)

### 5.4 Image Sources
- **Course images**: Unsplash với query parameters (w=800&h=450)
- **Instructor avatar**: Unsplash (w=150&h=150)
- **Reviewer avatars**: Unsplash (w=50&h=50)
- **Logo**: Rikkei Education official logo

### 5.5 Môi trường triển khai
- GitHub Pages
- Netlify
- Vercel
- Hoặc bất kỳ static hosting nào

---

## 6. Tính năng

### 6.1 Tính năng chức năng

#### 6.1.1 Navigation
- **Breadcrumb**: Links về trang chủ và danh sách khóa học
- **Header Menu**: Links về các sections trong trang chủ
- **Anchor Links**: Scroll đến instructor section

#### 6.1.2 Information Display
- **Course Overview**: Hiển thị đầy đủ thông tin meta
- **Pricing**: Giá gốc, giá sale, % giảm
- **Curriculum**: 8 sections với tổng số bài và thời lượng
- **Reviews**: Rating overview + breakdown + individual reviews
- **Instructor Profile**: Avatar, bio, stats

#### 6.1.3 Visual Feedback
- **Hover Effects**:
  - Buttons: transform translateY(-2px) + shadow
  - Cards: background color change
  - Links: color change
  - Preview image: play overlay opacity
- **Sticky Positioning**: Preview card sticky khi scroll (desktop)
- **Focus States**: Input-like elements có border highlight

#### 6.1.4 Content Organization
- **Sections**: Rõ ràng với headings và spacing
- **Lists**: Bullet points và checkmarks
- **Grid Layouts**: Learning outcomes, rating breakdown
- **Flex Layouts**: Meta info, buttons, headers

### 6.2 Tính năng phi chức năng

#### 6.2.1 Hiệu năng
- **Load Time**: < 2s (chỉ HTML/CSS)
- **Optimized Images**: Sử dụng query parameters để resize
- **Minimal CSS**: Tái sử dụng base styles
- **No JavaScript**: Không có overhead từ JS

#### 6.2.2 Khả năng sử dụng (Usability)
- **Clear Hierarchy**: Headings rõ ràng
- **Scannable Content**: Sử dụng lists, icons, spacing
- **Prominent CTAs**: Buttons nổi bật
- **Sticky Pricing**: Preview card luôn visible khi scroll
- **Breadcrumb**: Dễ quay lại trang trước

#### 6.2.3 Responsive Design
- **Mobile (320px - 767px)**:
  - Single column layout
  - Stacked elements
  - Full-width buttons
  - Reduced font sizes
  - Collapsed instructor header

- **Tablet (768px - 1023px)**:
  - Single column main layout
  - Preview card không sticky
  - Moderate spacing

- **Desktop (1024px+)**:
  - 2-column layout
  - Sticky preview card
  - Optimal spacing
  - Multi-column grids

#### 6.2.4 Accessibility
- **Semantic HTML**: header, nav, main, section, article
- **Alt Text**: Tất cả images có alt
- **ARIA Labels**: Links có aria-label khi cần
- **Heading Hierarchy**: h1, h2, h3 đúng thứ tự
- **Keyboard Navigation**: Có thể tab qua các elements
- **Color Contrast**: Đảm bảo contrast ratio tốt

#### 6.2.5 SEO
- **Meta Tags**: Title và description specific cho khóa học
- **Structured Content**: Proper heading hierarchy
- **Breadcrumb**: Giúp search engines hiểu structure
- **Semantic HTML**: Tốt cho crawlers
- **Image Alt Text**: Mô tả cho search engines

#### 6.2.6 Maintainability
- **CSS Variables**: Dễ thay đổi colors, spacing
- **Modular CSS**: Tách riêng course-detail.css
- **Consistent Naming**: BEM-like naming convention
- **Comments**: Code có comments khi cần
- **Reusable Classes**: .btn, .content-box, etc.

#### 6.2.7 Compatibility
- **Cross-browser**: Chrome, Firefox, Safari, Edge
- **Cross-device**: Desktop, tablet, mobile
- **Screen Sizes**: 320px đến 1920px+
- **No JavaScript Required**: Hoạt động hoàn toàn với HTML/CSS

### 6.3 Giới hạn tính năng
- **No Dynamic Curriculum**: Sections không expand/collapse được
- **No Video Player**: Play button chỉ là UI
- **No Cart Functionality**: "Thêm vào giỏ" chỉ là button
- **No Enrollment**: "Đăng ký ngay" chỉ là link
- **No Review Submission**: Không có form để submit review
- **No Helpful Voting**: Nút "Hữu ích" không hoạt động
- **Static Content**: Tất cả nội dung hard-coded
- **No User Authentication**: Login/Register buttons chỉ là UI

---

## 7. Tiêu chí nghiệm thu

### 7.1 Tiêu chí chức năng
- ✅ Breadcrumb navigation hoạt động
- ✅ Header links về trang chủ
- ✅ Tất cả sections hiển thị đầy đủ
- ✅ Curriculum hiển thị 8 sections với thông tin đúng
- ✅ Section 1 hiển thị 6 lectures chi tiết
- ✅ Instructor profile hiển thị đầy đủ
- ✅ Reviews hiển thị rating overview + breakdown + 3 reviews
- ✅ Sidebar hiển thị 3 related courses
- ✅ Share buttons hiển thị đầy đủ

### 7.2 Tiêu chí giao diện
- ✅ Course header có background tối với text trắng
- ✅ Preview card có styling đẹp với pricing rõ ràng
- ✅ Learning outcomes layout 2 cột (desktop)
- ✅ Curriculum sections có border và hover effect
- ✅ Rating bars hiển thị đúng tỷ lệ
- ✅ Instructor avatar tròn, hiển thị đẹp
- ✅ Review avatars tròn, kích thước phù hợp
- ✅ Related courses có thumbnail và thông tin đầy đủ
- ✅ Share buttons có màu sắc phù hợp

### 7.3 Tiêu chí responsive
- ✅ Desktop (>1024px): 2-column layout, sticky preview card
- ✅ Tablet (768-1024px): Single column, preview card static
- ✅ Mobile (<768px): All single column, stacked elements
- ✅ Không có horizontal scroll
- ✅ Images responsive, không vỡ layout
- ✅ Text readable trên mọi kích thước màn hình

### 7.4 Tiêu chí tương thích
- ✅ Hoạt động trên Chrome
- ✅ Hoạt động trên Firefox
- ✅ Hoạt động trên Safari
- ✅ Hoạt động trên Edge

### 7.5 Tiêu chí code quality
- ✅ HTML valid (W3C)
- ✅ CSS valid (W3C CSS)
- ✅ Code được format đẹp
- ✅ Sử dụng semantic HTML
- ✅ CSS organized và có comments
- ✅ Không có code dư thừa

### 7.6 Tiêu chí performance
- ✅ Trang load nhanh (< 2s)
- ✅ Images optimized với query parameters
- ✅ CSS minimal và efficient
- ✅ Không có blocking resources

---

## 8. Phụ lục

### 8.1 Thông tin khóa học mẫu

**Tên**: Lập Trình Web Từ Cơ Bản Đến Nâng Cao

**Thông tin cơ bản:**
- Danh mục: Lập trình
- Cấp độ: Cơ bản
- Thời lượng: 40 giờ
- Số bài học: 67 bài
- Số phần: 8 phần
- Ngôn ngữ: Tiếng Việt

**Giá:**
- Giá gốc: 2,999,000đ
- Giá sale: 1,999,000đ
- Giảm: 33%

**Thống kê:**
- Rating: 4.9/5
- Số đánh giá: 2,345
- Số học viên: 12,567
- Cập nhật: Tháng 12/2025

**Giảng viên:**
- Tên: Nguyễn Văn A
- Chức danh: Senior Full-stack Developer
- Kinh nghiệm: 10+ năm
- Tổng học viên: 45,678
- Tổng khóa học: 15
- Rating: 4.9/5

### 8.2 Curriculum chi tiết

**Phần 1: Giới thiệu và Cơ bản HTML** (8 bài • 3 giờ)
1. Giới thiệu khóa học và lộ trình học - 10:30
2. Cài đặt môi trường phát triển - 15:45
3. HTML cơ bản: Tags và Elements - 25:20
4. Làm việc với Text và Links - 20:15
5. Images và Multimedia - 18:30
6. Bài tập: Tạo trang HTML đầu tiên - 30:00

**Phần 2-8**: Chỉ hiển thị header với tổng số bài và thời lượng

### 8.3 Learning Outcomes (8 items)
1. Nắm vững HTML5 và CSS3 để xây dựng giao diện web hiện đại
2. Lập trình JavaScript từ cơ bản đến nâng cao
3. Sử dụng thành thạo React.js để xây dựng ứng dụng web
4. Thiết kế responsive cho mọi thiết bị
5. Làm việc với API và xử lý dữ liệu
6. Triển khai website lên hosting và domain
7. Xây dựng 5+ dự án thực tế để bổ sung portfolio
8. Áp dụng best practices và coding standards

### 8.4 Khóa học bao gồm (6 items)
1. 40 giờ video học
2. 25 bài tập thực hành
3. Truy cập trên mọi thiết bị
4. Truy cập trọn đời
5. Chứng chỉ hoàn thành
6. Hỗ trợ 24/7

### 8.5 Related Courses (3 items)
1. UI/UX Design Chuyên Nghiệp - 4.8⭐ - 1,699,000đ
2. Phát Triển Ứng Dụng Di Động - 4.7⭐ - 2,299,000đ
3. Machine Learning Cơ Bản - 4.9⭐ - 2,799,000đ

### 8.6 Sample Reviews (3 items)

**Review 1:**
- Tên: Trần Thị B
- Rating: 5⭐
- Thời gian: 2 tuần trước
- Nội dung: "Khóa học rất chi tiết và dễ hiểu. Giảng viên giải thích rất rõ ràng, từng bước một. Mình đã hoàn thành khóa học và tự tin làm được nhiều dự án web. Rất đáng tiền!"
- Helpful: 234

**Review 2:**
- Tên: Lê Văn C
- Rating: 5⭐
- Thời gian: 1 tháng trước
- Nội dung: "Mình là người chuyển nghề sang IT, khóa học này giúp mình rất nhiều. Nội dung cập nhật, bài tập thực tế. Sau 3 tháng học, mình đã apply được vị trí Junior Developer. Cảm ơn thầy và Rikkei Education!"
- Helpful: 189

**Review 3:**
- Tên: Phạm Thị D
- Rating: 5⭐
- Thời gian: 1 tháng trước
- Nội dung: "Khóa học tuyệt vời! Giảng viên nhiệt tình, support nhanh. Nội dung từ cơ bản đến nâng cao, phù hợp cho người mới. Mình đã làm được 3 dự án và đang freelance kiếm thêm thu nhập."
- Helpful: 156

### 8.7 Tài nguyên sử dụng
- **Images**: Unsplash (https://unsplash.com/)
- **Logo**: Rikkei Education (https://rikkei.edu.vn/)
- **Icons**: Unicode emoji characters
- **Fonts**: System fonts

### 8.8 Tài liệu tham khảo
- HTML5 Specification: https://html.spec.whatwg.org/
- CSS3 Specification: https://www.w3.org/Style/CSS/
- MDN Web Docs: https://developer.mozilla.org/
- CSS Sticky Positioning: https://developer.mozilla.org/en-US/docs/Web/CSS/position

---

## 9. So sánh với trang chủ

### 9.1 Điểm giống
- Sử dụng chung hệ thống màu sắc
- Sử dụng chung typography
- Sử dụng chung spacing system
- Header và Footer giống nhau
- Responsive breakpoints giống nhau

### 9.2 Điểm khác
- **Layout**: Trang chi tiết có 2-column layout (main + sidebar)
- **Header**: Course header có background tối thay vì màu primary
- **Sticky Elements**: Preview card sticky khi scroll
- **Content Depth**: Nhiều thông tin chi tiết hơn
- **Components**: Có thêm breadcrumb, curriculum, reviews, instructor profile
- **CSS File**: Có file CSS riêng (course-detail.css)

---

**Phiên bản**: 1.0  
**Ngày tạo**: 05/01/2026  
**Người tạo**: Development Team  
**Trạng thái**: Hoàn thành  
**Liên kết**: Trang này là phần mở rộng của Landing Page (xem SRS_Rikkei_Education.md)
