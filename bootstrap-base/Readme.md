# Bootstrap based

## Bootstrap 5 Containers

- **container** class cung cấp 1 vùng chứa có chiều rộng cố định, đáp ứng
  || Extra small < 576px|Small ≥ 576px|Medium ≥ 768px|Large ≥ 992px|Extra Large ≥ 1200px|XXL ≥ 1400px|
  | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
  |**max-width**|100%|540px|720px|960px|1140px|1320px|
- **container-fluid** class cung cấp 1 vùng chứa trải rộng toàn bộ chiều rộng của khung
  max-width luôn là 100%
- Responsive Containers
  Bạn cũng có thể sử dụng các lớp .container-sm | md | lg | xl để xác định khi nào vùng chứa sẽ đáp ứng.Chiều rộng tối đa của vùng chứa sẽ thay đổi trên các kích thước màn hình / chế độ xem khác nhau:
  |class| Extra small < 576px|Small ≥ 576px|Medium ≥ 768px|Large ≥ 992px|Extra Large ≥ 1200px|XXL ≥ 1400px|
  | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
  |.container-sm|100%|540px|720px|960px|1140px|1320px|
  |.container-md|100%|100%|720px|960px|1140px|1320px|
  |.container-lg|100%|100%|100%|960px|1140px|1320px|
  |.container-xl|100%|100%|100%|100%|1140px|1320px|
  |.container-xxl|100%|100%|100%|100%|100%|1320px|

## Bootstrap 5 Grid System

- là hệ thống lưới của bootstrap được xây dựng từ flex-box cho phép tối đa 12 cột trên 1 trang
- nó sẽ tự động sắp xếp lại tuỳ theo độ rộng của màn hình
- grid classes
  - .col- (extra small devices - screen width less than 576px)
  - .col-sm- (small devices - screen width equal to or greater than 576px)
  - .col-md- (medium devices - screen width equal to or greater than 768px)
  - .col-lg- (large devices - screen width equal to or greater than 992px)
  - .col-xl- (xlarge devices - screen width equal to or greater than 1200px)
  - .col-xxl- (xxlarge devices - screen width equal to or greater than 1400px)

## Bootstrap 5 Text/Typography

- theo mặc định Bootstrap 5 sử dụng kích thước phông chữ là 1rem (16px theo mặc định) và chiều cao dòng của nó là 1,5. Ngoài ra, tất cả các phần tử `<p>` đều có margin-top: 0 và margin-bottom: 1rem (16px theo mặc định).
- `<h1> - <h6>`
  - Bootstrap 5 định kiểu các thẻ tiêu đề HTML (`<h1> -> <h6>`) với phông chữ đậm hơn và kích thước phông chữ đáp ứng.
  - ngoài ra cũng có thể dùng class _.h1_ -> _.h6_ dể làm cho các phần tử khác hoạt động giống heading
- **Display Headings**
  - Display heading nổi bật hơn các heading bình thường (kích thước phông chữ lớn hơn và phông chữ mỏng hơn) và có 6 class để lựa chọn: _.display-1_ -> _.display-6_
- `<small>`
  - phần tử HTML `<small>` hay class _.small_ dùng để tạo ra tiêu đề phụ.
- `<mark>`
  - phần tử HTML `<mark>` hay class _.mark_ dùng để highlight text. text được highlight sẽ có background color và 1 chút padding
- `<abbr>`
  - phần tử HTML `<abbr>` dùng để tạo kiểu cho chữ có phần gạch chân bằng chấm và cusrsor hỏi chấm khi dược hover
- `<blockquote>`
  - phần tử HTML `<blockquote>` hay class _.blockquote_ dùng để trích dẫn các nội dụng từ nguồn khác
  - class _.blockquote-footer_ để đăt tên nguồn
- `<dl>`

  - phần tử HTML `<dl>` sử dụng để tạo kiểu cho các đanh sách mô tả
  - ví dụ:
    **Coffee**

    - black hot drink

    **Milk**

    - white cold drink

- `<code>`
  - phần tử HTML `<code>` dùng để hiện thị code
- `<kbd>`
  - phần tử HTML `<kbd>`dùng cho các kí tự hướng dẫn
  - ví dụ: ctrl s để lưu
- `<pre>`
  - phần tử HTML `<pre>` giữ nguyên định dạng khi viết nhiều dòng
- **More Typography Classes**
  |class|description|
  |---|---|
  |.lead|làm cho 1 đoạn văn nổi bật hơn|
  |.text-start|căn trái văn bản|
  |.text-break|ngăn văn bản dài bị vỡ bố cục|
  |.text-center|căn giữa văn bản|
  |.text-decoration-none|xoá gạch chân thẻ link|
  |.text-end|căn phải văn bản|
  |.text-nowrap|văn bản không xuống dòng|
  |.text-lowercase|chuyển văn bản thành chữ thường|
  |.text-uppercase|chuyển văn bản thành thữ hoa|
  |.text-capitalize|viết hoa kí tự đầu tiên của từng từ|
  |.initialism|Hiển thị văn bản bên trong phần tử `<abbr>` ở font-size nhỏ hơn một chút|
  |.list-unstyled|Loại bỏ list-style mặc định và margin trái trên các list items (hoạt động trên cả `<ul>` và `<ol>`). Lớp này chỉ áp dụng cho các mục danh sách con ngay lập tức (để xóa kiểu danh sách mặc định khỏi bất kỳ danh sách lồng nhau nào, hãy áp dụng lớp này cho mọi danh sách lồng nhau)|
  |.list-inline|Đặt tất cả các mục danh sách trên một dòng (được sử dụng cùng với class _.list-inline-item_ trên mỗi phần tử `<li>`)|

## Bootstrap 5 Colors

- **Text Colors**
  - Để tạo màu cho chữ sử dụng class `.text-[color]`
  - VD: `.text-muted, .text-primary, .text-success, .text-info, .text-warning, .text-danger, .text-secondary, .text-white, .text-dark, .text-body`
  - Để tạo opacity cho chữ chỉ cần thêm % opacity vào sau class
  - VD: `.text-danger-50, .text-success-80`
- **Background Colors**
  - dể tạo background color sử dụng class `.bg-[color]`
  - VD: `.bg-primary, .bg-success, .bg-info, .bg-warning, .bg-danger, .bg-secondary, .bg-dark and .bg-light`

## Bootstrap 5 Tables

- **Basic Table**
  - class `.table` vào phần tử html `<table>` để tạo kiểu 1 bảng đơn giản có padding nhẹ và có thanh horizontal để phân cách các dòng
- **Striped Rows**
  - thêm class `.table-striped` để tạo màu sọc sen kẽ cho các dòng
- **Bordered Table**
  - thêm class `.table-bordered` để thêm border cho bảng
- **Hover Rows**
  - thêm class `.table-hover` để tạo hiệU ứng hover vào dòng thì background color thành gray
- **Black/Dark Table**
  - thêm class `.table-dark` để đặt background color thành black
- **Dark Striped Table**
  - kết hợp 2 class `.table-dank .table-striped` để tạo bảng vừa nền đèn và có màu sọc sen kẽ cho các dòng
- **Hoverable Dark Table**
  - thêm class `.table-hover` để tạo hiệU ứng hover vào dòng thì background color thành gray
- **Borderless Table**
  - thêm class `.table-borderless` để xoá toàn bộ border khỏi bảng
- **Contextual Classes**
  - Contextual Classes có thể được sử dụng để tô màu toàn bộ bảng (`<table>`), các hàng trong bảng (`<tr>`) hoặc các ô trong bảng (`<td>`).
  - các Contextual Classes có thể được sử dụng là:
    | class | description |
    | ---------------- | ---------------------------------------------------------------------------------- |
    | .table-primary | Màu xanh lam: Biểu thị một hành động quan trọng |
    | .table-success | Màu xanh lá cây: Biểu thị một hành động thành công hoặc tích cực |
    | .table-danger | Màu đỏ: Biểu thị một hành động nguy hiểm hoặc có khả năng tiêu cực |
    | .table-info | Màu xanh lam nhạt: Biểu thị hành động hoặc thay đổi mang tính thông tin trung tính |
    | .table-warning | Màu cam: Cho biết một cảnh báo có thể cần chú ý |
    | .table-active | Màu xám: Áp dụng màu hover cho hàng trong bảng hoặc ô trong bảng |
    | .table-secondary | Màu xám: Biểu thị một hành động kém quan trọng hơn một chút |
    | .table-light | Màu xám nhạt: màu nền của bảng hoặc hàng trong bảng |
    | .table-dark | Màu xám đậm: màu nền của bảng hoặc hàng trong bảng |
- **Table Head Colors**
  - thêm contextual classes vào phần tử html `<thead>` để đỔi màu nền heading của bảng
- **Small table**
  - thêm class `.table-sm` vào phần tử html `<table>` để làm cho bảng nhỏ hơn (giảm 1 nửa padding của ô)
- **Responsive Tables**
  - thêm class `.table-responsive` để thêm thanh cuộn ngang khi cần thiết (khi chiều ngang của bảng lớn hơn vùng hiện thị)
  - có thể quyết định khi nào thì có thanh cuộn tuỳ theo độ rộNg của màn hình
    | class | Screen width |
    |--|--|
    | .table-responsive-sm | < 576px |
    | .table-responsive-md | < 768px |
    | .table-responsive-lg | < 992px |
    | .table-responsive-xl | < 1200px |
    | .table-responsive-xxl | < 1400px |

## Bootstrap 5 Images

- thêm class `.rounded` để thêm border-radius vào thẻ `<img>`
- thêm class `.rounded-circle` để hình ảnh thành hình tròn
- thêm class `.img-thumbnail` để tạo viền cho ảnh (border)
- **Căn hình ảnh**
  - dùng class `.float-start` hoặc `.float-end` để căn trái hoặc phải
  - để căn giữa dùng class `.mx-auto` (margin: auto) và `.d-block` (display: block)
- **Responsive Images**
  - thêm class `.img-fluid` vào phần tử html `<img>` để responsive hình ảnh theo chiều rộng phần tử cha
  - class `.img-fluid` áp dụng thuộc tính `max-width: 100%;` và `height: auto;`

## Bootstrap 5 Alerts

- **Alerts**
  - tạo ra các thông báo có kiểU được định trước
  - Alerts được tạo bằng cách sử dụng class `.alert` và 1 trong các Contextual Classes: `alert-success, .alert-info, .alert-warning, .alert-danger, .alert-primary, .alert-secondary, .alert-light or .alert-dark`
  - VD: `.alert .alert-success`
- **Alert Links**
  - Thêm class `.alert-link` vào bất kỳ liên kết nào bên trong alert box để tạo "matching colored links"(liên kết có màu phù hợp)
- **Closing Alerts**
  - Để đóng alert, hãy thêm một class .alert-dismissible vào vùng chứa Alert. Sau đó thêm `class = "btn-close"` và `data-bs-allow = "alert"` vào một liên kết hoặc một phần tử `<button>` (khi bạn nhấp vào hộp này, hộp cảnh báo sẽ biến mất).
  - VD:
  ```htm
  <div class="alert alert-success alert-dismissible">
    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
    <strong>Success!</strong> This alert box could indicate a successful or
    positive action.
  </div>
  ```
- **Animated Alerts**
  - thêm class `.fade` và `.show` để có hiệu ứng mờ đàn khi đóng alert

## Bootstrap 5 Buttons

- VD:

```htm
<button type="button" class="btn">Basic</button>
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-dark">Dark</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-link">Link</button>
```

- Các class của button có thể được sử dụng trên các phần tử `<a>`, `<button>` hoặc `<input>`
- **Button Outline**

```htm
<button type="button" class="btn btn-outline-primary">Primary</button>
<button type="button" class="btn btn-outline-secondary">Secondary</button>
<button type="button" class="btn btn-outline-success">Success</button>
<button type="button" class="btn btn-outline-info">Info</button>
<button type="button" class="btn btn-outline-warning">Warning</button>
<button type="button" class="btn btn-outline-danger">Danger</button>
<button type="button" class="btn btn-outline-dark">Dark</button>
<button type="button" class="btn btn-outline-light text-dark">Light</button>
```

- **Button Size**
  - sử dụng thêm class `.btn-sm` hoặc `btn-lg` cho loại button nhỏ hoặc lớn hơn
- **Block Level Buttons**
  - Để tạo nút cấp khối kéo dài toàn bộ chiều rộng của phần tử mẹ, hãy sử dụng class `.d-grid` "helper" trên phần tử mẹ
  - VD:
    ```htm
    <div class="d-grid">
      <button type="button" class="btn btn-primary btn-block">
        Full-Width Button
      </button>
    </div>
    ```
  - nếu có nhiều nút như vậy có thể kiểm soát khoảng cách của chúng với class `.gap-*`
  - VD:

```htm
<div class="d-grid gap-3">
  <button type="button" class="btn btn-primary btn-block">
    Full-Width Button
  </button>
  <button type="button" class="btn btn-primary btn-block">
    Full-Width Button
  </button>
  <button type="button" class="btn btn-primary btn-block">
    Full-Width Button
  </button>
</div>
```

- **Active/Disabled Buttons**
  - để Active button thêm class `.active`
  - để Disabled button thêm class attribute _disabled_ vào button. nếu là nút tạo từ phần tử `<a>` thì thêm class `.disabled` vì không hỗi trợ attribute _disabled_

## Bootstrap 5 Button Groups

- **Button Groups**
  - cho phép gộp các button lại với nhau thành 1 nhóm
  - chỉ cần dùng phần tử `<div>` và thêm class `.btn-group` đỂ tạo 1 nhóm các button
  - VD:

```htm
<div class="btn-group">
  <button type="button" class="btn btn-primary">Apple</button>
  <button type="button" class="btn btn-primary">Samsung</button>
  <button type="button" class="btn btn-primary">Sony</button>
</div>
```

- Thay vì đặt kích thước cho từng button trong một nhóm, hãy sử dụng class `.btn-group-lg` cho nhóm nút lớn hoặc `.btn-group-sm` cho nhóm nút nhỏ
- **Vertical Button Groups**
  - Sử dụng class `.btn-group-vertical` để tạo nhóm button theo chiều dọc
- **Button Groups Side by Side**
  - Các nhóm nút là _inline_ theo mặc định, điều này làm cho chúng xuất hiện cạnh nhau khi bạn có nhiều nhóm
- **Nesting Button Groups & Dropdown Menus**

```htm
<div class="btn-group">
  <button type="button" class="btn btn-primary">Apple</button>
  <button type="button" class="btn btn-primary">Samsung</button>
  <div class="btn-group">
    <button
      type="button"
      class="btn btn-primary dropdown-toggle"
      data-bs-toggle="dropdown"
    >
      Sony
    </button>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Tablet</a>
      <a class="dropdown-item" href="#">Smartphone</a>
    </div>
  </div>
</div>
```
