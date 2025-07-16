HTML (10 câu)
HTML5 Semantic Elements là gì? Cho ví dụ.
→ Trả lời: Thẻ mô tả rõ mục đích nội dung (ví dụ: <header>, <article>, <nav>). Giúp SEO tốt hơn và tăng khả năng truy cập.

Sự khác biệt giữa id và class?
→ Trả lời: id là duy nhất (1 phần tử/id), class dùng cho nhóm phần tử. CSS: #id vs .class.

data-* attribute dùng để làm gì?
→ Trả lời: Lưu dữ liệu tùy chỉnh trong DOM (ví dụ: <div data-user-id="123">). Truy cập qua JS: element.dataset.userId.

Meta tag viewport quan trọng thế nào?
→ Trả lời: <meta name="viewport" content="width=device-width, initial-scale=1"> → Responsive design trên mobile.

Khi nào dùng <canvas> vs <svg>?
→ Trả lời: <canvas> cho đồ họa động (game), <svg> cho đồ họa vector (icons, hình đơn giản).

defer và async trong thẻ <script> khác nhau ra sao?
→ Trả lời: Cả hai không chặn DOM. async tải và chạy ngay khi tải xong, defer chạy sau khi DOM sẵn sàng.

CORS là gì?
→ Trả lời: Cơ chế bảo mật trình duyệt ngăn truy cập tài nguyên từ domain khác. Server phải gửi header Access-Control-Allow-Origin.

HTML Form: GET vs POST?
→ Trả lời: GET gửi dữ liệu qua URL (dùng cho tìm kiếm), POST gửi qua body (dùng cho tạo/xóa dữ liệu).

Local Storage vs Session Storage?
→ Trả lời: Local Storage lưu vĩnh viễn, Session Storage mất khi đóng tab.

Cách tối ưu hình ảnh trong HTML?
→ Trả lời: Dùng định dạng WebP, thuộc tính loading="lazy", srcset cho responsive, nén ảnh.

CSS (20 câu)
CSS Box Model là gì?
→ Trả lời: Gồm: content → padding → border → margin. box-sizing: border-box bao gồm padding/border trong width.

Position: relative, absolute, fixed khác nhau thế nào?
→ Trả lời:

relative: Dịch chuyển từ vị trí gốc.

absolute: Tuyệt đối so với phần tử cha gần nhất có position ≠ static.

fixed: Tuyệt đối so với viewport.

Flexbox vs Grid?
→ Trả lời:

Flexbox: 1 chiều (row hoặc column).

Grid: 2 chiều (row + column). Dùng Grid cho layout phức tạp.

BEM là gì? Ví dụ.
→ Trả lời: Quy ước đặt tên class: .block__element--modifier (ví dụ: .menu__item--active).

CSS Specificity tính thế nào?
→ Trả lời: Độ ưu tiên: !important > inline style > #id > .class > element. Tính điểm: (0,0,0,0).

em vs rem?
→ Trả lời: em dựa trên font-size của phần tử cha, rem dựa trên font-size root (<html>).

Media Query viết thế nào?
→ Trả lời:

css
@media (max-width: 768px) { ... } /* Mobile */
CSS Variable là gì?
→ Trả lời: Khai báo: :root { --color: red; }, sử dụng: color: var(--color);.

Cách center một phần tử?
→ Trả lời:

css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
Pseudo-class :nth-child() dùng thế nào?
→ Trả lời: Chọn phần tử con thứ n (ví dụ: :nth-child(2n) chọn phần tử chẵn).

CSS Reset vs Normalize.css?
→ Trả lời: Reset xóa style mặc định, Normalize.css chuẩn hóa style giữa trình duyệt.

z-index hoạt động ra sao?
→ Trả lời: Kiểm soát thứ tự chồng lớp. Chỉ hoạt động với position ≠ static.

CSS Selector A > B vs A B?
→ Trả lời: A > B: con trực tiếp, A B: mọi phần tử B bên trong A.

Transition vs Animation?
→ Trả lời: Transition cho hiệu ứng đơn giản (hover), Animation cho hiệu ứng phức tạp với @keyframes.

Cách ẩn phần tử?
→ Trả lời:

display: none: Xóa khỏi layout.

visibility: hidden: Ẩn nhưng vẫn chiếm chỗ.

opacity: 0: Trong suốt nhưng tương tác được.

Float trong CSS dùng để làm gì?
→ Trả lời: Canh trái/phải phần tử, thường dùng cho bố cục cũ. Hiện đại dùng Flex/Grid.

overflow: hidden có tác dụng gì ngoài ẩn nội dung?
→ Trả lời: Tạo BFC (Block Formatting Context) → ngăn margin collapse.

Sự khác biệt giữa inline và inline-block?
→ Trả lời: inline không đặt width/height, inline-block có thể.

CSS Preprocessor (SASS/LESS) ưu điểm gì?
→ Trả lời: Biến, nested rules, mixins, functions → code ngắn gọn hơn.

Responsive Design vs Adaptive Design?
→ Trả lời: Responsive dùng media query (1 code cho mọi device), Adaptive dùng server detect device để trả layout riêng.

JavaScript (30 câu)
let, const, var khác nhau thế nào?
→ Trả lời:

var: function-scoped, hoisting.

let/const: block-scoped, không hoisting.

const không gán lại được.

Closure là gì? Cho ví dụ.
→ Trả lời: Hàm truy cập biến ngoài phạm vi nó. Ví dụ:

javascript
function outer() {
  let x = 10;
  return function inner() { console.log(x); };
}
this trong JavaScript?
→ Trả lời: Giá trị this phụ thuộc vào ngữ cảnh:

Hàm thường: this = global (window/undefined trong strict mode).

Arrow function: this từ scope ngoài.

Method: this = object gọi hàm.

Promise là gì?
→ Trả lời: Xử lý bất đồng bộ. Có 3 trạng thái: pending, fulfilled, rejected. Dùng .then(), .catch().

Async/Await khác Promise thế nào?
→ Trả lời: Async/await là syntax sugar cho Promise, giúp code đồng bộ hơn. Ví dụ:

javascript
async function fetchData() {
  const data = await fetch(url);
}
Event Bubbling và Capturing?
→ Trả lời:

Bubbling: Sự kiện lan từ trong ra ngoài.

Capturing: Lan từ ngoài vào trong.
Dùng e.stopPropagation() để dừng.

Cách tạo object trong JS?
→ Trả lời:

javascript
// 1. Object literal
const obj = { key: "value" };

// 2. Constructor
function Person(name) { this.name = name; }
map() vs forEach()?
→ Trả lời: map() trả về mảng mới, forEach() không trả về gì.

=== vs ==?
→ Trả lời: === so sánh giá trị và kiểu dữ liệu, == chỉ so giá trị (chuyển đổi kiểu).

Arrow function và regular function?
→ Trả lời: Arrow function không có this, arguments, không dùng làm constructor.

null vs undefined?
→ Trả lời: undefined là biến chưa gán giá trị, null là giá trị rỗng cố ý.

Event Loop là gì?
→ Trả lời: Cơ chế xử lý bất đồng bộ: Call Stack → Callback Queue → Event Loop đẩy vào Stack khi rỗng.

Cách clone object?
→ Trả lời:

javascript
const shallowCopy = { ...obj };
const deepCopy = JSON.parse(JSON.stringify(obj));
call(), apply(), bind() khác nhau?
→ Trả lời:

call(thisArg, arg1, arg2): Gọi hàm với this mới.

apply(thisArg, [args]): Tương tự nhưng nhận mảng.

bind(thisArg): Trả về hàm mới với this bị ràng buộc.

typeof và instanceof?
→ Trả lời: typeof trả kiểu dữ liệu, instanceof kiểm tra object thuộc class nào.

Các phương thức mảng thường dùng?
→ Trả lời: push(), pop(), slice(), splice(), find(), filter(), reduce().

Debounce vs Throttle?
→ Trả lời:

Debounce: Gọi hàm sau khi dừng event X ms (ví dụ: search input).

Throttle: Gọi hàm mỗi X ms (ví dụ: scroll).

localStorage vs sessionStorage vs Cookie?
→ Trả lời:

Cookie: Lưu 4KB, gửi lên server.

localStorage: Lưu 5-10MB, không hết hạn.

sessionStorage: Hết khi đóng tab.

ES6 Modules?
→ Trả lời:

javascript
// Export
export const foo = () => {};

// Import
import { foo } from './module.js';
Template Literals?
→ Trả lời: Dùng backtick `Hello ${name}` để chèn biến và multi-line string.

Rest và Spread operator?
→ Trả lời:

javascript
// Rest: Gom thành mảng
function sum(...args) { }

// Spread: Giải mảng/object
const arr2 = [...arr1];
CORS giải quyết thế nào?
→ Trả lời:

Server trả header Access-Control-Allow-Origin: *.

Dùng proxy hoặc JSONP (cũ).

fetch() vs axios?
→ Trả lời: fetch() có sẵn trong trình duyệt, axios là thư viện hỗ trợ cancel request, timeout.

Strict mode là gì?
→ Trả lời: "use strict": Ngăn lỗi phổ biến (vd: biến chưa khai báo), bật tính năng mới.

setTimeout() và setInterval()?
→ Trả lời: setTimeout() chạy 1 lần, setInterval() lặp lại.

Callback hell là gì?
→ Trả lời: Callback lồng nhau gây khó đọc. Giải quyết bằng Promise/async-await.

IIFE là gì?
→ Trả lời: Immediately Invoked Function Expression:

javascript
(function() { console.log("IIFE"); })();
Object.keys() vs Object.entries()?
→ Trả lời:

Object.keys(obj): Trả mảng keys.

Object.entries(obj): Trả mảng [key, value].

Sự kiện DOMContentLoaded vs load?
→ Trả lời:

DOMContentLoaded: DOM sẵn sàng (chưa load ảnh).

load: Mọi tài nguyên (ảnh, CSS) đã tải xong.

Memoization là gì?
→ Trả lời: Kỹ thuật cache kết quả hàm để tối ưu hiệu năng (dùng cho hàm tốn CPU).

React (20 câu)
Virtual DOM là gì?
→ Trả lời: Bản sao JS của DOM thật. React so sánh Virtual DOM trước/sau khi thay đổi → cập nhật DOM thật tối thiểu.

Sự khác biệt giữa state và props?
→ Trả lời:

Props: Dữ liệu từ cha → con (read-only).

State: Dữ liệu nội bộ component (thay đổi bằng setState/useState).

Component Lifecycle trong class component?
→ Trả lời:

Mounting: constructor → render → componentDidMount.

Updating: shouldComponentUpdate → render → componentDidUpdate.

Unmounting: componentWillUnmount.

Hooks là gì?
→ Trả lời: Cho phép dùng state, lifecycle trong functional component (ví dụ: useState, useEffect).

useEffect dùng thế nào?
→ Trả lời: Xử lý side effect (call API, subscriptions). Có thể mô phỏng componentDidMount, componentDidUpdate, componentWillUnmount.

Conditional rendering trong React?
→ Trả lời: Dùng if, &&, hoặc ternary operator:

jsx
{isLoggedIn && <UserPanel />}
Keys trong list quan trọng thế nào?
→ Trả lời: Giúp React xác định phần tử thay đổi → tối ưu render. Dùng giá trị unique (id).

Sự khác biệt giữa controlled và uncontrolled component?
→ Trả lời:

Controlled: Form data quản lý bởi React state.

Uncontrolled: Form data quản lý bởi DOM (dùng useRef).

Lifting State Up là gì?
→ Trả lời: Di chuyển state lên component cha gần nhất để chia sẻ state giữa các component con.

Context API dùng để làm gì?
→ Trả lời: Truyền dữ liệu xuyên component mà không cần prop drilling (vd: theme, user data).

Cách tối ưu hiệu năng React?
→ Trả lời:

React.memo() cho functional component.

useMemo, useCallback để memoize.

Code splitting.

Redux là gì?
→ Trả lời: Thư viện quản lý state toàn cục. Luồng: Action → Reducer → Store → View.

JSX là gì?
→ Trả lời: Cú pháp giống HTML trong JS, được Babel biên dịch thành React.createElement().

Các cách styling trong React?
→ Trả lời: Inline style, CSS module, Styled Components, Sass.

Server-Side Rendering (SSR) vs Client-Side Rendering (CSR)?
→ Trả lời:

SSR: Render HTML trên server → tốt cho SEO.

CSR: Render trên trình duyệt → tương tác mượt hơn.

Custom Hook là gì?
→ Trả lời: Hàm tái sử dụng logic có sử dụng hooks (tên bắt đầu bằng use).

useRef dùng thế nào?
→ Trả lời: Lưu giá trị tồn tại giữa các lần render, không gây re-render. Thường dùng truy cập DOM.

Error Boundary trong React?
→ Trả lời: Component bắt lỗi trong cây con, hiển thị UI dự phòng. Dùng componentDidCatch.

PropTypes là gì?
→ Trả lời: Kiểm tra kiểu dữ liệu props:

javascript
Component.propTypes = { name: PropTypes.string.isRequired }
React Router dùng thế nào?
→ Trả lời: Quản lý routing:

jsx
<Route path="/about" element={<About />} />
Chung & Best Practices (20 câu)
Web Accessibility (a11y) là gì?
→ Trả lời: Thiết kế web dùng được cho người khuyết tật. Cách: dùng semantic HTML, ARIA attributes, keyboard navigation.

SEO cơ bản cho Frontend?
→ Trả lời: Meta tags, semantic HTML, tối ưu hình ảnh, server-side rendering, tốc độ tải.

CORS hoạt động thế nào?
→ Trả lời: Trình duyệt gửi OPTIONS request để kiểm tra server có cho phép domain hiện tại không.

HTTP/2 ưu điểm gì?
→ Trả lời: Multiplexing (nhiều request trên 1 kết nối), header compression, server push.

Cookie attributes: Secure, HttpOnly, SameSite?
→ Trả lời:

Secure: Chỉ gửi qua HTTPS.

HttpOnly: Chặn JS truy cập.

SameSite: Chống CSRF.

CSRF là gì? Phòng chống?
→ Trả lời: Tấn công giả mạo request. Cách chống: Dùng CSRF token, cookie SameSite=Strict.

XSS là gì? Phòng chống?
→ Trả lời: Tấn công chèn mã độc. Cách chống: Escape user input, dùng Content-Security-Policy.

Các công cụ debug Frontend?
→ Trả lời: Chrome DevTools, React DevTools, Redux DevTools, ESLint.

Tree Shaking là gì?
→ Trả lời: Kỹ thuật loại code không dùng khi build (vd: Webpack).

Lazy loading là gì?
→ Trả lời: Tải tài nguyên (ảnh, component) khi cần. React: React.lazy(), ảnh: loading="lazy".

Critical Rendering Path là gì?
→ Trả lời: Quá trình trình duyệt chuyển HTML/CSS/JS thành pixels trên màn hình. Tối ưu bằng minimize render-blocking resources.

FOUC là gì? Cách khắc phục?
→ Trả lời: "Flash of Unstyled Content": Hiện trang chưa load CSS. Khắc phục: load CSS trước, hoặc dùng inline CSS.

WebSockets vs HTTP?
→ Trả lời: WebSocket kết nối hai chiều real-time (chat), HTTP chỉ request-response.

Progressive Web App (PWA) là gì?
→ Trả lời: Web app có tính năng native: offline (service workers), push notification, installable.

Server-Sent Events (SSE)?
→ Trả lời: Cơ chế server gửi sự kiện đến client qua HTTP (1 chiều).

Web Workers dùng để làm gì?
→ Trả lời: Chạy script trên luồng nền → tránh block main thread.

Các phương pháp tối ưu hình ảnh?
→ Trả lời: Nén ảnh (TinyPNG), dùng WebP/AVIF, responsive images (srcset), lazy loading.

Bundle size tối ưu thế nào?
→ Trả lời: Code splitting, tree shaking, minify, gzip, dùng thư viện nhẹ.

Feature Detection vs Browser Sniffing?
→ Trả lời:

Feature Detection: Kiểm tra trình duyệt hỗ trợ tính năng không (dùng if('feature' in window)).

Browser Sniffing: Kiểm tra user-agent → không khuyến khích.

CORS-safe HTTP methods?
→ Trả lời: GET, HEAD, POST không yêu cầu preflight. PUT, DELETE yêu cầu preflight.
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
