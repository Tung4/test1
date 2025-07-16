New structure:
- HTML: 20 câu
- CSS: 20 câu
- JavaScript: 50 câu
- React: 40 câu
- Performance: 10 câu
- Security: 10 câu
- Tooling & Best Practices: 10 câu
Total: 20+20+50+40+10+10+10 = 160 câu.
But note: the previous list had 100 questions. We need to expand to 160.
We'll:
1. Keep the existing questions and reassign some to the new categories (e.g., some security and performance were in the old list, now we have dedicated categories).
2. Add new questions to meet the counts.
Let's break down:
### HTML (20 câu)
We had 10, so we need 10 more.
### CSS (20 câu)
We had 20 in the previous list? Actually, we had 20 in the previous list (from 11 to 30). So we are good.
### JavaScript (50 câu)
We had 30 (from 31 to 60). We need 20 more.
### React (40 câu)
We had 20 (from 61 to 80). We need 20 more.
### Performance (10 câu)
We had a few in the old list (like lazy loading, bundle size, etc.). We'll move them to this category and add more.
### Security (10 câu)
We had 2 (CORS, XSS, CSRF). We'll move them and add more.
### Tooling & Best Practices (10 câu)
We had some in the old list (like ESLint, tree shaking, etc.). We'll move and add.
We'll reorganize and add new questions accordingly.
Let's start:
---
## HTML (20 câu) - Existing 10 + 10 new
### Existing 10:
1. HTML5 Semantic Elements là gì? Cho ví dụ.
2. Sự khác biệt giữa `id` và `class`?
3. `data-*` attribute dùng để làm gì?
4. Meta tag `viewport` quan trọng thế nào?
5. Khi nào dùng `<canvas>` vs `<svg>`?
6. `defer` và `async` trong thẻ `<script>` khác nhau ra sao?
7. CORS là gì?
8. HTML Form: GET vs POST?
9. Local Storage vs Session Storage?
10. Cách tối ưu hình ảnh trong HTML?
### New 10:
11. **Mô tả các thẻ HTML dùng để tạo bảng.**
    → *Trả lời:* `<table>`, `<tr>` (table row), `<th>` (table header), `<td>` (table data), `<thead>`, `<tbody>`, `<tfoot>`, `<caption>`.
12. **`<div>` và `<span>` khác nhau thế nào?**
    → *Trả lời:* `<div>` là block-level, dùng để nhóm các phần tử block. `<span>` là inline, dùng để nhóm nội dung inline.
13. **`<meta>` tags thường dùng cho SEO?**
    → *Trả lời:* 
    ```html
    <meta name="description" content="...">
    <meta name="keywords" content="...">
    <meta name="author" content="...">
    <meta property="og:title" content="..."> <!-- Open Graph for social media -->
    ```
14. **`<iframe>` dùng để làm gì? Nhược điểm?**
    → *Trả lời:* Nhúng trang web khác vào. Nhược điểm: bảo mật (XSS, clickjacking), ảnh hưởng SEO, tải chậm.
15. **`<picture>` element dùng khi nào?**
    → *Trả lời:* Khi muốn hiển thị hình ảnh khác nhau tùy vào điều kiện (ví dụ: màn hình retina, độ rộng khác nhau). Kết hợp với `<source>` và `<img>`.
16. **`<datalist>` là gì?**
    → *Trả lời:* Cung cấp danh sách gợi ý cho input. Ví dụ:
    ```html
    <input list="browsers">
    <datalist id="browsers">
      <option value="Chrome">
      <option value="Firefox">
    </datalist>
    ```
17. **`<base>` tag có tác dụng gì?**
    → *Trả lời:* Xác định base URL cho tất cả relative URLs trong trang. Ví dụ: `<base href="https://example.com/">`.
18. **`<progress>` vs `<meter>`?**
    → *Trả lời:* 
    - `<progress>`: Hiển thị tiến độ hoàn thành của một tác vụ.
    - `<meter>`: Hiển thị giá trị trong một phạm vi (ví dụ: đĩa cứng đầy).
19. **Web Components là gì?**
    → *Trả lời:* Bộ công nghệ tạo component tùy chỉnh, đóng gói (Custom Elements, Shadow DOM, HTML Templates).
20. **ARIA roles là gì? Tại sao quan trọng?**
    → *Trả lời:* Accessible Rich Internet Applications: bổ sung thông tin cho screen reader (ví dụ: `role="button"`). Quan trọng cho web accessibility.
---
## CSS (20 câu) - Existing 20
We already had 20, so we keep them (questions 11 to 30 from the previous list).
---
## JavaScript (50 câu) - Existing 30 + 20 new
### Existing 30 (from the previous list, questions 31 to 60)
### New 20:
51. **`Symbol` trong ES6 dùng để làm gì?**
    → *Trả lời:* Tạo giá trị duy nhất, thường dùng làm key cho object property (tránh xung đột).
52. **Generator function là gì?**
    → *Trả lời:* Hàm có thể tạm dừng và tiếp tục chạy, dùng `function*` và `yield`. Ví dụ:
    ```javascript
    function* gen() {
      yield 1;
      yield 2;
    }
    ```
53. **`new` keyword hoạt động thế nào?**
    → *Trả lời:* Tạo object mới, gán `this` cho object đó, chạy constructor function, trả về object.
54. **`Array.from()` dùng để làm gì?**
    → *Trả lời:* Tạo mảng mới từ array-like hoặc iterable object. Ví dụ: `Array.from('foo')` → `['f','o','o']`.
55. **`Object.freeze()` vs `Object.seal()`?**
    → *Trả lời:* 
    - `Object.freeze()`: không thể thay đổi giá trị, không thêm/xóa property.
    - `Object.seal()`: có thể thay đổi giá trị, nhưng không thêm/xóa property.
56. **`for...in` vs `for...of`?**
    → *Trả lời:* 
    - `for...in`: lặp qua enumerable properties (kể cả kế thừa), dùng cho object.
    - `for...of`: lặp qua iterable objects (array, string, Map, Set).
57. **`Set` và `Map`?**
    → *Trả lời:* 
    - `Set`: tập hợp giá trị duy nhất.
    - `Map`: tập hợp key-value, key có thể bất kỳ kiểu gì.
58. **`WeakMap` và `WeakSet`?**
    → *Trả lời:* Tương tự `Map` và `Set` nhưng không giữ reference mạnh đến object (giúp tránh rò rỉ bộ nhớ).
59. **`Proxy` object?**
    → *Trả lời:* Cho phép tạo proxy cho object, can thiệp các hành vi (đọc, ghi, ...). Dùng cho validation, logging.
60. **`Array.reduceRight()`?**
    → *Trả lời:* Tương tự `reduce` nhưng duyệt từ phải sang trái.
61. **`__proto__` vs `prototype`?**
    → *Trả lời:* 
    - `prototype`: property của constructor function, chứa các phương thức cho các instance.
    - `__proto__`: property của instance, trỏ đến `prototype` của constructor.
62. **`import` và `export` có những cách nào?**
    → *Trả lời:* 
    ```javascript
    // Named export/import
    export const foo = ...;
    import { foo } from ...;
    // Default export/import
    export default ...;
    import bar from ...;
    // Namespace import
    import * as module from ...;
    ```
63. **`try...catch` có bắt được lỗi trong asynchronous code không?**
    → *Trả lời:* Không, trừ khi dùng `async/await` hoặc `.catch()` cho promise.
64. **`Object.assign()` vs spread operator?**
    → *Trả lời:* Cả hai đều dùng để sao chép object. Spread syntax (ES2018) ngắn gọn hơn, nhưng `Object.assign()` có thể gán vào object target.
65. **`String.raw()`?**
    → *Trả lời:* Dùng để in string nguyên bản (không xử lý escape). Ví dụ: `String.raw`\n` in ra "\\n".
66. **`Intl` object dùng để làm gì?**
    → *Trả lời:* Format số, ngày, tiền tệ theo ngôn ngữ (internationalization). Ví dụ: `Intl.DateTimeFormat`.
67. **`decodeURI()` vs `decodeURIComponent()`?**
    → *Trả lời:* 
    - `decodeURI`: giải mã toàn bộ URI.
    - `decodeURIComponent`: giải mã từng phần của URI (như %20).
68. **`eval()` có nên dùng không? Tại sao?**
    → *Trả lời:* Không, vì bảo mật (chạy mã tùy ý) và hiệu năng.
69. **`with` statement?**
    → *Trả lời:* Thêm object vào scope chain. Không nên dùng vì khó đọc, không tối ưu được, và bị cấm trong strict mode.
70. **`Error` object có các thuộc tính nào?**
    → *Trả lời:* `name`, `message`, `stack` (non-standard).
---
## React (40 câu) - Existing 20 + 20 new
### Existing 20 (from the previous list, questions 61 to 80)
### New 20:
81. **React Fragments dùng để làm gì?**
    → *Trả lời:* Bao bọc nhiều phần tử mà không cần thêm node DOM, dùng `<Fragment>` hoặc `<>...</>`.
82. **Portals trong React?**
    → *Trả lời:* Render component ra ngoài DOM hierarchy (vd: modal, tooltip). Dùng `ReactDOM.createPortal(child, container)`.
83. **`useReducer` dùng thế nào?**
    → *Trả lời:* Quản lý state phức tạp, tương tự Redux. Nhận reducer function và initial state, trả về state và dispatch function.
84. **React.memo() là gì?**
    → *Trả lời:* Higher Order Component để memoize functional component, chỉ re-render khi props thay đổi.
85. **Lợi ích của việc dùng key prop?**
    → *Trả lời:* Giúp React xác định item nào thay đổi, thêm, xóa → hiệu năng tốt hơn.
86. **React.StrictMode là gì?**
    → *Trả lời:* Phát hiện các vấn đề tiềm ẩn (vd: unsafe lifecycle, legacy API) trong ứng dụng. Chỉ chạy ở development.
87. **`useLayoutEffect` vs `useEffect`?**
    → *Trả lời:* 
    - `useEffect`: chạy sau khi render và paint (không block UI).
    - `useLayoutEffect`: chạy sau khi render nhưng trước khi paint (dùng khi cần tính toán layout).
88. **Cách bắt lỗi trong React component?**
    → *Trả lời:* Dùng Error Boundary (class component với `componentDidCatch`).
89. **React Suspense?**
    → *Trả lời:* Hiển thị fallback UI trong khi chờ dữ liệu hoặc component tải. Dùng với `React.lazy`.
90. **Code splitting trong React?**
    → *Trả lời:* Chia nhỏ bundle, tải component khi cần. Dùng `React.lazy` và `Suspense`.
91. **Server Components trong React?**
    → *Trả lời:* Component chạy trên server, giảm bundle client. Đang thử nghiệm.
92. **React Hook Form vs Formik?**
    → *Trả lời:* Thư viện quản lý form. React Hook Form tập trung hiệu năng (uncontrolled), Formik dùng controlled.
93. **`useImperativeHandle`?**
    → *Trả lời:* Tùy chỉnh instance value khi dùng `ref` (thường kết hợp với `forwardRef`).
94. **React Context có nhược điểm gì?**
    → *Trả lời:* Khó tối ưu (khi context value thay đổi, mọi component dùng context đều re-render). Nên dùng cho dữ liệu ít thay đổi.
95. **Khi nào dùng Redux thay vì Context?**
    → *Trả lời:* Khi ứng dụng phức tạp, cần middleware (logger, thunk), dev tools, hoặc xử lý state lớn.
96. **Redux Toolkit là gì?**
    → *Trả lời:* Bộ công cụ chính thức để viết Redux đơn giản hơn (tạo store, slice, tự động xử lý immutable).
97. **Redux Thunk vs Redux Saga?**
    → *Trả lời:* 
    - Thunk: dùng cho logic async đơn giản (hàm trả về hàm).
    - Saga: dùng generator function, xử lý side effect phức tạp.
98. **`connect()` trong React-Redux?**
    → *Trả lời:* HOC để kết nối component với Redux store (mapStateToProps, mapDispatchToProps).
99. **Cấu trúc thư mục React project?**
    → *Trả lời:* Có nhiều cách: 
    - Theo chức năng (feature-based): mỗi feature có component, service, style riêng.
    - Theo kiểu file: components/, containers/, services/, ...
100. **Testing React component?**
     → *Trả lời:* Dùng Jest (test runner) và React Testing Library (test behavior) hoặc Enzyme (test implementation).
---
## Performance (10 câu)
We'll take some from the old list and add new ones.
1. **Lazy loading là gì? (moved from HTML)**
    → *Trả lời:* Tải tài nguyên (ảnh, component) khi cần. React: `React.lazy()`, ảnh: `loading="lazy"`.
2. **Bundle size tối ưu thế nào? (moved from old list)**
    → *Trả lời:* Code splitting, tree shaking, minify, gzip, dùng thư viện nhẹ.
3. **Critical Rendering Path là gì? (moved from old list)**
    → *Trả lời:* Quá trình trình duyệt chuyển HTML/CSS/JS thành pixels trên màn hình. Tối ưu bằng minimize render-blocking resources.
4. **Debounce và Throttle? (moved from JavaScript)**
    → *Trả lời:*  
    - Debounce: Gọi hàm sau khi dừng event X ms (ví dụ: search input).  
    - Throttle: Gọi hàm mỗi X ms (ví dụ: scroll).
5. **Virtual DOM giúp cải thiện hiệu năng?**
    → *Trả lời:* So sánh Virtual DOM trước/sau, chỉ cập nhật phần thay đổi lên DOM thật → giảm số lần update DOM.
6. **`useMemo` và `useCallback`?**
    → *Trả lời:* 
    - `useMemo`: memoize giá trị tính toán.
    - `useCallback`: memoize function.
    → Tránh tính toán lại hoặc tạo function mới khi không cần.
7. **Window.onload vs document.DOMContentLoaded?**
    → *Trả lời:* 
    - `DOMContentLoaded`: khi DOM sẵn sàng (chưa có ảnh).
    - `window.onload`: khi tất cả tài nguyên (ảnh, CSS) tải xong.
8. **Tại sao tránh inline style trong React?**
    → *Trả lời:* Tạo object style mới mỗi lần render → component con re-render không cần thiết.
9. **Tối ưu ảnh? (moved from old list)**
    → *Trả lời:* Nén ảnh (TinyPNG), dùng WebP/AVIF, responsive images (`srcset`), lazy loading.
10. **Web Workers? (moved from old list)**
     → *Trả lời:* Chạy script trên luồng nền → tránh block main thread.
---
## Security (10 câu)
1. **CORS là gì? (moved from HTML)**
    → *Trả lời:* Cơ chế bảo mật trình duyệt ngăn truy cập tài nguyên từ domain khác. Server phải gửi header `Access-Control-Allow-Origin`.
2. **XSS là gì? Phòng chống? (moved from old list)**
    → *Trả lời:* Tấn công chèn mã độc. Cách chống: Escape user input, dùng `Content-Security-Policy`.
3. **CSRF là gì? Phòng chống? (moved from old list)**
    → *Trả lời:* Tấn công giả mạo request. Cách chống: Dùng CSRF token, cookie `SameSite=Strict`.
4. **`HttpOnly` cookie? (moved from old list)**
    → *Trả lời:* Chặn JavaScript truy cập cookie → chống XSS.
5. **Content Security Policy (CSP)?**
    → *Trả lời:* Header quy định nguồn tài nguyên được phép tải (script, image, ...), chống XSS.
6. **SQL Injection?**
    → *Trả lời:* Tấn công chèn mã SQL vào input. Frontend không xử lý, phải do backend (dùng parameterized queries).
7. **Clickjacking?**
    → *Trả lời:* Tấn công dùng iframe che phủ nút thật. Chống: dùng header `X-Frame-Options: DENY` hoặc `Content-Security-Policy: frame-ancestors 'none'`.
8. **HTTPS tại sao quan trọng?**
    → *Trả lời:* Mã hóa dữ liệu giữa client và server, chống nghe lén, bảo vệ thông tin nhạy cảm.
9. **JWT (JSON Web Token) lưu ở đâu an toàn?**
    → *Trả lời:* HttpOnly cookie (chống XSS), không lưu localStorage/sessionStorage.
10. **Mã hóa mật khẩu ở frontend?**
     → *Trả lời:* Không nên. Mật khẩu phải được mã hóa ở backend (dùng bcrypt, ...). Frontend có thể hash nhưng không thay thế backend.
---
## Tooling & Best Practices (10 câu)
1. **ESLint là gì?**
    → *Trả lời:* Công cụ kiểm tra code JavaScript, bắt lỗi, đảm bảo coding convention.
2. **Tree Shaking? (moved from old list)**
    → *Trả lời:* Kỹ thuật loại code không dùng khi build (vd: Webpack).
3. **Webpack vs Vite?**
    → *Trả lời:* 
    - Webpack: bundler phổ biến, mạnh mẽ.
    - Vite: build tool nhanh, dùng ES modules native, phát triển bởi Vue creator.
4. **Git hook là gì?**
    → *Trả lời:* Kịch bản chạy trước/sau các sự kiện Git (vd: pre-commit chạy linter).
5. **CI/CD là gì?**
    → *Trả lời:* Continuous Integration/Continuous Deployment: tự động build, test, deploy khi push code.
6. **Unit test vs Integration test?**
    → *Trả lời:* 
    - Unit test: test từng hàm/component riêng lẻ.
    - Integration test: test tương tác giữa các thành phần.
7. **Feature Flags?**
    → *Trả lời:* Kỹ thuật bật/tắt tính năng mà không cần deploy mới. Dùng để thử nghiệm, rollback nhanh.
8. **Chrome DevTools dùng để debug lỗi gì?**
    → *Trả lời:* Lỗi JS (Sources), mạng (Network), hiệu năng (Performance), bộ nhớ (Memory).
9. **Prettier?**
    → *Trả lời:* Công cụ format code tự động, thường kết hợp với ESLint.
10. **Semantic Versioning (SemVer)?**
     → *Trả lời:* Quy ước đặt version: MAJOR.MINOR.PATCH. 
        - PATCH: sửa lỗi.
        - MINOR: thêm tính năng (không phá vỡ API cũ).
        - MAJOR: thay đổi lớn, phá vỡ API cũ.
---
---
### **Performance (10 câu bổ sung)**
1. **Tại sao nên sử dụng CDN?**  
   → CDN (Content Delivery Network) giúp phân phối tài nguyên tĩnh (ảnh, CSS, JS) từ server gần người dùng → giảm latency, tăng tốc độ tải.
2. **Preload, Prefetch, Preconnect?**  
   → 
   - `preload`: Tải sớm tài nguyên quan trọng (font, CSS critical).  
   - `prefetch`: Tải trước tài nguyên cho trang tiếp theo.  
   - `preconnect`: Thiết lập kết nối sớm đến domain bên ngoài.
3. **HTTP/2 Server Push là gì?**  
   → Server chủ động gửi tài nguyên tới browser trước khi browser yêu cầu → giảm round trips.
4. **Critical CSS là gì?**  
   → CSS cần thiết cho nội dung hiển thị đầu tiên (above-the-fold). Nên inline để tránh render-blocking.
5. **Tác dụng của `will-change`?**  
   → Báo trước cho browser biết phần tử sẽ thay đổi (transform, opacity) → browser chuẩn bị tối ưu hóa.
6. **Lazy loading cho video?**  
   → Dùng `loading="lazy"` cho thẻ `<video>` hoặc sử dụng Intersection Observer API để tải khi video vào viewport.
7. **Tối ưu Web Fonts?**  
   → 
   - Dùng `font-display: swap` để hiển thị text sớm.  
   - Subset font (chỉ ký tự cần thiết).  
   - Preload font.
8. **Memory Leak trong JS?**  
   → Rò rỉ bộ nhớ khi không giải phóng biến không dùng. Cách phát hiện: Chrome DevTools Memory tab.
9. **Tại sao tránh dùng `@import` trong CSS?**  
   → `@import` gây render-blocking và tăng số request. Thay bằng `<link>` hoặc gom file.
10. **Tối ưu re-render trong React?**  
    → 
    - Sử dụng `React.memo` cho component.  
    - Tránh truyền callback/inline object làm prop (dùng `useCallback`/`useMemo`).  
    - Chia nhỏ component.
---
### **Security (10 câu bổ sung)**
1. **Same-origin Policy (SOP) là gì?**  
   → Chỉ cho phép website truy cập tài nguyên cùng origin (protocol + domain + port). Ngăn truy cập tài nguyên trái phép.
2. **CORS Preflight Request?**  
   → Browser gửi OPTIONS request để kiểm tra server có cho phép method/header không trước khi gửi request thật.
3. **XSS Reflected vs Stored?**  
   → 
   - Reflected: Mã độc nằm trong URL → nạn nhân click link.  
   - Stored: Mã độc lưu vào database (bình luận) → hiển thị cho mọi người.
4. **DOM-based XSS?**  
   → Mã độc thông qua thao tác DOM (vd: `document.write()` với input user) → không gửi đến server.
5. **Security Headers quan trọng?**  
   → 
   - `Content-Security-Policy`: Chống XSS.  
   - `X-Frame-Options`: Chống clickjacking.  
   - `X-Content-Type-Options: nosniff`: Ngăn MIME sniffing.  
   - `Strict-Transport-Security`: Buộc dùng HTTPS.
6. **JWT (JSON Web Token) bảo mật thế nào?**  
   → Ký token bằng secret key (HS256) hoặc private key (RS256). Lưu token trong HttpOnly cookie.
7. **OAuth 2.0 Flow?**  
   → Ủy quyền truy cập tài nguyên mà không chia sẻ mật khẩu. Gồm: Authorization Code Flow (server-side), Implicit Flow (client-side).
8. **Rate Limiting?**  
   → Giới hạn số request từ client → chống brute force. Triển khai ở server.
9. **Subresource Integrity (SRI)?**  
   → Kiểm tra file tải từ CDN không bị sửa đổi. Ví dụ:  
   ```html
   <script src="https://cdn.example.com/lib.js" 
           integrity="sha384-..."></script>
   ```
10. **CORS với Credentials?**  
    → Khi gửi cookie qua CORS, server cần:  
    - Header `Access-Control-Allow-Credentials: true`  
    - `Access-Control-Allow-Origin` phải chỉ định domain (không dùng `*`).
---
Tổng cộng giờ chúng ta đã có:
- Performance: 20 câu (10 ban đầu + 10 bổ sung)
- Security: 20 câu (10 ban đầu + 10 bổ sung)
Hy vọng bộ câu hỏi này giúp bạn tự tin hơn khi phỏng vấn! Nếu cần giải thích sâu hơn câu nào, hãy hỏi nhé.
