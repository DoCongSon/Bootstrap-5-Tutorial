# Bootstrap base

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

## Bootstrap 5 Badges

- Badged là thẻ huy để bổ sung thông tin (VD: số thông báo tin nhắn)
- Sử dụng class `.badge` cùng với contextual classes (như `.bg-Secondary`) trong các phần tử `<span>` để tạo huy hiệu hình chữ nhật.
- Sử dụng class `.rounded-tablet` để làm cho các huy hiệu được bo tròn hơn
- **Badge inside an Element**
  - VD: huy hiệu trong 1 button

```htm
<button type="button" class="btn btn-primary">
  Messages <span class="badge bg-danger">4</span>
</button>
```

## Bootstrap 5 Progress Bars

- là 1 thanh tiến trình hiện thị mức độ người dùng
- Để tạo Progress Bars mặc định, hãy thêm class `.progress` vào phần tử vùng chứa và thêm class `.progress-bar` vào phần tử con của nó. Sử dụng thuộc tính _width_ trong CSS để đặt chiều rộng của thanh tiến trình
  - VD:

```htm
<div class="progress">
  <div class="progress-bar" style="width:70%"></div>
</div>
```

- Chiều cao của Progress Bars là 1rem (thường là 16px) theo mặc định. Sử dụng thuộc tính height trong CSS để thay đổi nó. Lưu ý rằng bạn phải đặt cùng một chiều cao cho vùng chứa tiến trình và thanh tiến trình
- Thêm văn bản bên trong thanh tiến trình để hiển thị phần trăm hiển thị 70%

```htm
<div class="progress">
  <div class="progress-bar" style="width:70%">70%</div>
</div>
```

- Theo mặc định, thanh tiến trình có màu xanh lam (primary). Sử dụng bất kỳ contextual background classes nào để thay đổi màu của nó

```htm
<div class="progress">
  <div class="progress-bar bg-success" style="width:20%"></div>
</div>
```

- Sử dụng class `.progress-bar-striped` để thêm các sọc trang trí vào các Progress Bars. Thêm class `.progress-bar-animation` để tạo hoạt ảnh cho Progress Bars
- Progress Bars cũng có thể được xếp chồng lên nhau

```htm
<div class="progress">
  <div class="progress-bar bg-success" style="width:40%">Free Space</div>
  <div class="progress-bar bg-warning" style="width:10%">Warning</div>
  <div class="progress-bar bg-danger" style="width:20%">Danger</div>
</div>
```

## Bootstrap 5 Spinners

- Để tạo một spinner / loader, hãy sử dụng class `.spinner-border`
  VD: `<div class="spinner-border"></div>`
- để thêm màu sắc hay sử dụng bấy kì class `.text-*` (\* : color ) nào:
  VD `<div class="spinner-border text-primary"></div>`
- Sử dụng class `.spinner-grow` nếu bạn muốn spinner / loader thành "grow" thay vì "spin"
- Sử dụng `.spinner-border-sm` hoặc `.spinner-grow-sm` nếu muốn spinner / loader nhỏ hơn
- bạn có thể sử dụng spin trong 1 button

```htm
<button class="btn btn-primary">
  <span class="spinner-border spinner-border-sm"></span>
  Loading..
</button>
```

## Bootstrap 5 Pagination

- **Basic Pagination**
  - Nếu bạn có một trang web với nhiều trang, bạn có thể muốn thêm một số loại phân trang cho mỗi trang.
  - Để tạo một phân trang cơ bản, hãy thêm class `.pagination` vào một phần tử `<ul>`. Sau đó, thêm `.page-item` vào từng phần tử `<li>` và một class `.page-link` vào mỗi liên kết bên trong `<li>`
  - VD:

```htm
<ul class="pagination">
  <li class="page-item"><a class="page-link" href="#">Previous</a></li>
  <li class="page-item"><a class="page-link" href="#">1</a></li>
  <li class="page-item"><a class="page-link" href="#">2</a></li>
  <li class="page-item"><a class="page-link" href="#">3</a></li>
  <li class="page-item"><a class="page-link" href="#">Next</a></li>
</ul>
```

- **Active/Disabled State**
  - class `.active` được sử dụng để "highlight" trang hiện tại.
  - class `.disabled` được sử dụng cho các liên kết không thể nhấp được
- **Pagination Sizing**
  - thêm class `.pagination-lg` cho phân trang lớn hoặc `.pagination-sm` cho phân trang nhỏ hơn
- **Pagination Alignment**

  - Sử dụng các class `justify-content-*` (\*: center, end) để căn chỉnh phân trang

- **Breadcrumbs**
  - Các class `.breadcrumb` và `.breadcrumb-item` cho biết vị trí của trang hiện tại trong phân cấp điều hướng:

```htm
<ul class="breadcrumb">
  <li class="breadcrumb-item"><a href="#">Photos</a></li>
  <li class="breadcrumb-item"><a href="#">Summer 2017</a></li>
  <li class="breadcrumb-item"><a href="#">Italy</a></li>
  <li class="breadcrumb-item active">Rome</li>
</ul>
```

## Bootstrap 5 List Groups

- **Basic List Groups**
  - là 1 đanh sách không có thứ tự với các mục danh sách
  - Để tạo một nhóm danh sách cơ bản, hãy sử dụng phần tử `<ul>` với class `.list-group` và phần tử `<li>` với class `.list-group-item`

```htm
<ul class="list-group">
  <li class="list-group-item">First item</li>
  <li class="list-group-item">Second item</li>
  <li class="list-group-item">Third item</li>
</ul>
```

- **Active/Disabled State**

  - class `.active` được sử dụng để "highlight" item hiện tại.
  - class `.disabled` được sử dụng cho các item không thể nhấp được và có màu nhạt hơn

- **List Group With Linked Items**

  - Để tạo nhóm danh sách với các mục được liên kết, hãy sử dụng `<div>`thay vì `<ul>` và `<a>` thay vì `<li>`. Theo tùy chọn, thêm class `.list-group-item-action` nếu bạn muốn có màu nền xám khi di chuột.

- **Flush / Remove Borders**

  - Sử dụng class `.list-group-flush` để loại bỏ một số đường viền và các góc tròn

- **Numbered List Groups**

  - Sử dụng class `.list-group-number` để tạo các mục danh sách với các số phía trước chúng

- **Horizontal List Groups**

  - Nếu bạn muốn các mục trong danh sách hiển thị theo chiều ngang thay vì chiều dọc hãy thêm class `.list-group-horizontal` cạnh `.list-group`

- **Contextual Classes**

  - Contextual Classes có thể được sử dụng để thêm màu cho các mục trong danh sách
  - VD: `.list-group-item-success, list-group-item-secondary, list-group-item-info, list-group-item-warning, .list-group-item-danger, .list-group-item-primary, list-group-item-dark and list-group-item-light`

- **List Group with Badges**
  - có thể hiệN thị huy hiệu vào item như sau:

```htm
<ul class="list-group">
  <li class="list-group-item d-flex justify-content-between align-items-center">
    Inbox
    <span class="badge bg-primary rounded-pill">12</span>
  </li>
  <li class="list-group-item d-flex justify-content-between align-items-center">
    Ads
    <span class="badge bg-primary rounded-pill">50</span>
  </li>
  <li class="list-group-item d-flex justify-content-between align-items-center">
    Junk
    <span class="badge bg-primary rounded-pill">99</span>
  </li>
</ul>
```

## Bootstrap 5 Cards

- **Basic Card**

  - Một thẻ cơ bản được tạo bằng class `.card` và nội dung bên trong thẻ có class `.card-body`
  - class `.card-header` thêm tiêu đề vào thẻ và class `.card-footer` thêm phần chân trang vào thẻ

  ```htm
  <div class="card">
    <div class="card-header">Header</div>
    <div class="card-body">Content</div>
    <div class="card-footer">Footer</div>
  </div>
  ```

- **Contextual Cards**

  - Để thêm màu nền cho thẻ, hãy sử dụng contextual classes (`.bg-primary`, `.bg-success`, `.bg-info`, `.bg-warning`, `.bg-danger`, `.bg-secondary`, `.bg-dark` and `.bg-light`)

- **Titles, text, and links**

  - Sử dụng `.card-title` để thêm tiêu đề thẻ vào bất kỳ phần tử Heading nào (`<h1> -> <h6>`). class `.card-text` được sử dụng để xóa margin-bottom cho phần tử `<p>` nếu nó là phần tử con cuối cùng (hoặc phần tử duy nhất) bên trong `.card-body`. class `.card-link` thêm màu xanh lam vào bất kỳ liên kết nào và hiệu ứng di chuột.

- **Card Images**

  - Thêm `.card-img-top` hoặc `.card-img-bottom` vào `<img>` để đặt hình ảnh ở trên hoặc ở dưới bên trong thẻ. Lưu ý rằng chúng tôi đã thêm hình ảnh bên ngoài `.card-body` để kéo dài toàn bộ chiều rộng

  ```htm
  <div class="card" style="width:400px">
    <img class="card-img-top" src="img_avatar1.png" alt="Card image" />
    <div class="card-body">
      <h4 class="card-title">John Doe</h4>
      <p class="card-text">Some example text.</p>
      <a href="#" class="btn btn-primary">See Profile</a>
    </div>
  </div>
  ```

- để biến hình ảnh thành nền sử dụng `.card-img-overlay` để thêm văn bản đè lên hình ảnh

```htm
<div class="card" style="width:500px">
  <img class="card-img-top" src="img_avatar1.png" alt="Card image" />
  <div class="card-img-overlay">
    <h4 class="card-title">John Doe</h4>
    <p class="card-text">Some example text.</p>
    <a href="#" class="btn btn-primary">See Profile</a>
  </div>
</div>
```

## Bootstrap 5 Dropdowns

- **Basic Dropdown**

  - class `.dropdown` chỉ ra một menu thả xuống.
  - Để mở menu thả xuống, hãy sử dụng button hoặc liên kết có class `.dropdown-toggle` và attribute (thuộc tính) data-bs-toggle = "dropdown".
  - Thêm class `.dropdown-menu` vào phần tử `<div>` để tạo menu thả xuống. Sau đó, thêm class `.dropdown-item` vào từng phần tử (liên kết hoặc nút) bên trong menu thả xuống.
  - VD:

  ```htm
  <div class="dropdown">
    <button
      type="button"
      class="btn btn-primary dropdown-toggle"
      data-bs-toggle="dropdown"
    >
      Dropdown button
    </button>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Link 1</a></li>
      <li><a class="dropdown-item" href="#">Link 2</a></li>
      <li><a class="dropdown-item" href="#">Link 3</a></li>
    </ul>
  </div>
  ```

- class `.dropdown-divider` được sử dụng để phân tách các liên kết bên trong menu thả xuống bằng một đường viền ngang mỏng

  - VD: `<li><hr class="dropdown-divider"></hr></li>`

- class `.dropdown-header` được sử dụng để thêm các tiêu đề bên trong menu thả xuống.

  - VD: `<li><h5 class="dropdown-header">Dropdown header 1</h5></li>`

- class `.dropdown-item-text` được sử dụng để thêm văn bản thuần túy vào một mục thả xuống hoặc được sử dụng trên các liên kết để tạo kiểu liên kết mặc định.

  - VD: `<li><a class="dropdown-item-text" href="#">Text Link</a></li>`
    `<li><span class="dropdown-item-text">Just Text</span></li>`

- **Disable and Active items**:

  - sử dụng thêm class `.active` hoặc `.disabled` để "highlight" item hoặc làm cho nó mờ đi không bấm được

- **Dropdown Position**

  - Bạn cũng có thể tạo menu "drop end" hoặc "drop start" bằng cách thêm class `.dropend` hoặc `.dropstart` vào phần tử thả xuống. Lưu ý rằng dấu mũi tên được thêm tự động
  - VD: `<div class="dropdown dropend">`

- **Dropup**

  - Nếu bạn muốn menu thả xuống mở rộng lên trên thay vì xuống dưới, hãy thay đổi phần tử `<div>` với class `.dropdown` thành `.dropup`

- **Dropdown Menu Right**
  - Để căn phải menu thả xuống, hãy thêm class `.dropdown-menu-end` vào phần tử có `.dropdown-menu`

## Bootstrap 5 Collapse

- Collapsibles rất hữu ích khi bạn muốn ẩn và hiển thị một lượng lớn nội dung
-
- **Basic Collapsible**

  - class `.collapse` chỉ ra một phần tử có thể thu gọn (một `<div>` trong ví dụ); đây là nội dung sẽ được hiển thị hoặc ẩn bằng một lần nhấp vào nút.
  - Để kiểm soát (hiển thị / ẩn) nội dung có thể thu gọn, hãy thêm thuộc tính `data-bs-toggle = "collapse"` vào phần tử `<a>` hoặc `<button>`. Sau đó, thêm thuộc tính `data-bs-target = "#id"` để kết nối nút với nội dung có thể thu gọn (`<div id = "demo">`).
  - Lưu ý: Đối với các phần tử `<a>`, bạn có thể sử dụng thuộc tính `href` thay vì thuộc tính `data-bs-target`
  - VD:

  ```htm
  <button data-bs-toggle="collapse" data-bs-target="#demo">Collapsible</button>
  <div id="demo" class="collapse">Lorem ipsum dolor text....</div>
  ```

- Theo mặc định, nội dung thu gọn được ẩn. Tuy nhiên, bạn có thể thêm class `.show` để hiển thị nội dung theo mặc định

  - `<div id="demo" class="collapse show">Lorem ipsum dolor text....</div>`

- **Accordion**

  - Ví dụ sau đây cho thấy một accordion đơn giản bằng cách mở rộng thành phần thẻ.
  - Lưu ý: Sử dụng thuộc tính `data-bs-parent` để đảm bảo rằng tất cả các phần tử có thể thu gọn trong phần tử gốc được chỉ định sẽ bị đóng khi một trong các mục có thể thu gọn được hiển thị.
  - VD:

  ```htm
  <div id="accordion">
    <div class="card">
      <div class="card-header">
        <a class="btn" data-bs-toggle="collapse" href="#collapseOne">
          Collapsible Group Item #1
        </a>
      </div>
      <div id="collapseOne" class="collapse show" data-bs-parent="#accordion">
        <div class="card-body">Lorem ipsum..</div>
      </div>
    </div>

    <div class="card">
      <div class="card-header">
        <a class="collapsed btn" data-bs-toggle="collapse" href="#collapseTwo">
          Collapsible Group Item #2
        </a>
      </div>
      <div id="collapseTwo" class="collapse" data-bs-parent="#accordion">
        <div class="card-body">Lorem ipsum..</div>
      </div>
    </div>

    <div class="card">
      <div class="card-header">
        <a
          class="collapsed btn"
          data-bs-toggle="collapse"
          href="#collapseThree"
        >
          Collapsible Group Item #3
        </a>
      </div>
      <div id="collapseThree" class="collapse" data-bs-parent="#accordion">
        <div class="card-body">Lorem ipsum..</div>
      </div>
    </div>
  </div>
  ```

## Bootstrap 5 Navs

- **Nav Menus**

  - Nếu bạn muốn tạo một menu ngang đơn giản, hãy thêm class `.nav` vào phần tử `<ul>`, tiếp theo là `.nav-item` cho mỗi `<li>` và thêm `.nav-link` vào các liên kết của chúng

  ```htm
  <ul class="nav justify-content-center">
    <li class="nav-item">
      <a class="nav-link" href="#">Link</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#">Link</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#">Link</a>
    </li>
    <li class="nav-item">
      <a class="nav-link disabled" href="#">Disabled</a>
    </li>
  </ul>
  ```

  - Thêm `.justify-content-center` để căn giữa, `.justify-content-end` để căn phải điều hướng.
  - Thêm class `.flex-column` để tạo điều hướng theo chiều dọc:
    `<ul class="nav flex-column">`

- **Tabs**

  - Biến menu điều hướng thành các tab điều hướng với class `.nav-tabs`. Thêm class `.active` vào liên kết hoạt động / hiện tại.

  ```htm
  <ul class="nav nav-tabs">
    <li class="nav-item">
      <a class="nav-link active" href="#">Active</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#">Link</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#">Link</a>
    </li>
    <li class="nav-item">
      <a class="nav-link disabled" href="#">Disabled</a>
    </li>
  </ul>
  ```

- Biến menu điều hướng thành hình các "viên thuốc" điều hướng với class `.nav-Drugs`.

  - Căn đều các tab / viên thuốc bằng class `.nav-justify` (chiều rộng bằng nhau)
    `<ul class="nav nav-pills nav-justified">..</ul>`
    `<ul class="nav nav-tabs nav-justified">..</ul>`

- **Toggleable / Dynamic Tabs**

  - Để làm cho các tab có thể chuyển đổi, hãy thêm thuộc tính `data-toggle = "tab"` vào từng liên kết. Sau đó, thêm một class `.tab-pane` với một ID duy nhất cho mọi tab và bọc chúng bên trong phần tử `<div>` với class `.tab-content`.
  - Nếu bạn muốn các tab mờ dần khi nhấp vào chúng, hãy thêm lớp `.fade` vào `.tab-pane`

  ```htm
  <!-- Nav tabs -->
  <ul class="nav nav-tabs">
    <li class="nav-item">
      <a class="nav-link active" data-bs-toggle="tab" href="#home">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-bs-toggle="tab" href="#menu1">Menu 1</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-bs-toggle="tab" href="#menu2">Menu 2</a>
    </li>
  </ul>

  <!-- Tab panes -->
  <div class="tab-content">
    <div class="tab-pane container active" id="home">...</div>
    <div class="tab-pane container fade" id="menu1">...</div>
    <div class="tab-pane container fade" id="menu2">...</div>
  </div>
  ```

- **Toggleable / Dynamic Pills**
  - giống hoàn toàn với toggleable / dynamic tabs chỉ thay thuộc tính `data-toggle = "tab"` bằng thuộc tính `data-toggle = "pill"`

## Bootstrap 5 Navbars

- **Basic Navbar**

  - Với Bootstrap, một thanh điều hướng có thể mở rộng hoặc thu gọn, tùy thuộc vào kích thước màn hình.
  - Thanh điều hướng tiêu chuẩn được tạo với class `.navbar`, theo sau là class thu gọn đáp ứng: `.navbar-expand-xxl | xl | lg | md | sm` (xếp thanh điều hướng theo chiều dọc trên màn hình xxl | xl | lg| md | sm).
  - Để thêm liên kết bên trong thanh điều hướng, hãy sử dụng phần tử `<ul>` (hoặc `<div>`) với `class = "navbar-nav"`. Sau đó, thêm phần tử `<li>` có class `.nav-item` theo sau là phần tử `<a>` có class `.nav-link`

  ```htm
  <!-- A grey horizontal navbar that becomes vertical on small screens -->
  <nav class="navbar navbar-expand-sm bg-light">
    <div class="container-fluid">
      <!-- Links -->
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#">Link 1</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 2</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 3</a>
        </li>
      </ul>
    </div>
  </nav>
  ```

  - để thanh điềU hướng luôn nằm dọc chỉ cần xoá class `.navbar-expand-*`
  - Thêm class `.justify-content-center` để căn giữa thanh điều hướng
  - Sử dụng bất kỳ class `.bg-color` nào để thay đổi màu nền của thanh điều hướng (`.bg-primary`, `.bg-success`, `.bg-info`, `.bg-warning`, `.bg-risk`, `.bg-Secondary`, `.bg -dark` và `.bg-light`)
    - Mẹo: Thêm màu văn bản trắng vào tất cả các liên kết trong thanh điều hướng với class `.navbar-dark` hoặc sử dụng class `.navbar-light` để thêm màu văn bản đen.

- **Brand / Logo**

  - class `.navbar-brand` được sử dụng để làm nổi bật thương hiệu / logo / tên dự án trên trang của bạn
  - Khi sử dụng class `.navbar-brand` với hình ảnh, Bootstrap 5 sẽ tự động tạo kiểu hình ảnh cho vừa với thanh điều hướng theo chiều dọc.
  - VD:

  ```htm
  <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img
          src="logo.png"
          alt="Avatar Logo"
          style="width:40px;"
          class="rounded-pill"
        />
      </a>
    </div>
  </nav>
  ```

- **Navbar Text**

  - Sử dụng class `.navbar-text` để căn chỉnh theo chiều dọc bất kỳ phần tử nào bên trong thanh điều hướng không phải là liên kết (đảm bảo padding và màu văn bản phù hợp)

  ```htm
  <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
    <div class="container-fluid">
      <span class="navbar-text">Navbar text</span>
    </div>
  </nav>
  ```

- **Navbar Toggle**

  - Thường xuyên, đặc biệt là trên màn hình nhỏ, bạn muốn ẩn các liên kết điều hướng và thay thế chúng bằng một nút sẽ hiển thị chúng khi nhấp vào.

  - Để tạo thanh điều hướng có thể thu gọn, hãy sử dụng button có `class = "navbar-toggler"`, `data-bs-toggle = "collapse"` và `data-bs-target = "#thetarget"`. Sau đó, bọc nội dung thanh điều hướng (liên kết, v.v.) bên trong phần tử `<div>` bằng `class = "collapse navbar-collapse"`, theo sau là một id khớp với mục tiêu dữ liệu của nút: "thetarget".

  ```htm
  <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Logo</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#collapsibleNavbar"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="collapsibleNavbar">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  ```

  - Mẹo: Bạn cũng có thể xóa class `.navbar-expand-md` để luôn luôn ẩn các liên kết điều hướng và hiển thị nút bật tắt

- **Navbar With Dropdown**

```htm
<li class="nav-item dropdown">
  <a
    class="nav-link dropdown-toggle"
    href="#"
    role="button"
    data-bs-toggle="dropdown"
    >Dropdown</a
  >
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#">Link</a></li>
    <li><a class="dropdown-item" href="#">Another link</a></li>
    <li><a class="dropdown-item" href="#">A third link</a></li>
  </ul>
</li>
```

- **Navbar Forms and Buttons**

```htm
<nav class="navbar navbar-expand-sm navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="javascript:void(0)">Logo</a>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#mynavbar"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="mynavbar">
      <ul class="navbar-nav me-auto">
        <li class="nav-item">
          <a class="nav-link" href="javascript:void(0)">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="javascript:void(0)">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="javascript:void(0)">Link</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="text" placeholder="Search" />
        <button class="btn btn-primary" type="button">Search</button>
      </form>
    </div>
  </div>
</nav>
```

- **Fixed/Sticky Navigation Bar**
  - class `.fixed-top` làm cho thanh điều hướng được cố định ở trên cùng, class `.fixed-bottom` làm cho thanh điều hướng được cố định ở bên dưới cùng
    `<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top"> ... </nav>`
  - Sử dụng class `.sticky-top` để làm cho thanh điều hướng cố định / ở đầu trang khi bạn cuộn qua nó. Lưu ý class này không hoạt động trong IE11 trở về trước (nó sẽ coi là `position:relative`).

## Bootstrap 5 Carousel

```htm
<!-- Carousel -->
<div id="demo" class="carousel slide" data-bs-ride="carousel">
  <!-- Indicators/dots -->
  <div class="carousel-indicators">
    <button
      type="button"
      data-bs-target="#demo"
      data-bs-slide-to="0"
      class="active"
    ></button>
    <button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
    <button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
  </div>

  <!-- The slideshow/carousel -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="la.jpg" alt="Los Angeles" class="d-block w-100" />
    </div>
    <div class="carousel-item">
      <img src="chicago.jpg" alt="Chicago" class="d-block w-100" />
    </div>
    <div class="carousel-item">
      <img src="ny.jpg" alt="New York" class="d-block w-100" />
    </div>
  </div>

  <!-- Left and right controls/icons -->
  <button
    class="carousel-control-prev"
    type="button"
    data-bs-target="#demo"
    data-bs-slide="prev"
  >
    <span class="carousel-control-prev-icon"></span>
  </button>
  <button
    class="carousel-control-next"
    type="button"
    data-bs-target="#demo"
    data-bs-slide="next"
  >
    <span class="carousel-control-next-icon"></span>
  </button>
</div>
```

| Class                       | Description                                                                                                                                                                                 |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| .carousel                   | tạo ra carousel                                                                                                                                                                             |
| .carousel-indicators        | Thêm các chỉ báo cho băng chuyền. Đây là những chấm nhỏ ở cuối mỗi trang trình bày (cho biết có bao nhiêu trang trình bày trong băng chuyền và trang trình bày mà người dùng hiện đang xem) |
| .carousel-inner             | thêm các slide vào carousel                                                                                                                                                                 |
| .carousel-item              | Chỉ định nội dung của từng slide                                                                                                                                                            |
| .carousel-control-prev      | Thêm nút bên trái (trước) vào băng chuyền, cho phép người dùng quay lại giữa các trang trình bày                                                                                            |
| .carousel-control-next      | Thêm nút bên phải (tiếp theo) vào băng chuyền, cho phép người dùng chuyển tiếp giữa các trang trình bày                                                                                     |
| .carousel-control-prev-icon | Được sử dụng cùng với .carousel-control-prev để tạo nút "trước đó"                                                                                                                          |
| .carousel-control-next-icon | Được sử dụng cùng với .carousel-control-next để tạo nút "tiếp theo"                                                                                                                         |
| .slide                      | Thêm hiệu ứng chuyển tiếp CSS và hoạt ảnh khi trượt từ mục này sang mục tiếp theo. Xóa lớp này nếu bạn không muốn có hiệu ứng này                                                           |

- **Add Captions to Slides**

  - Thêm các phần tử bên trong `<div class = "carousel-caption">` trong mỗi `<div class = "carousel-item">` để tạo chú thích cho mỗi trang trình bày

  ```htm
  <div class="carousel-item">
    <img src="la.jpg" alt="Los Angeles" />
    <div class="carousel-caption">
      <h3>Los Angeles</h3>
      <p>We had such a great time in LA!</p>
    </div>
  </div>
  ```

## Bootstrap 5 Modal

- Modal là một hộp thoại / cửa sổ bật lên được hiển thị trên trang hiện tại

```htm
<!-- Button to Open the Modal -->
<button
  type="button"
  class="btn btn-primary"
  data-bs-toggle="modal"
  data-bs-target="#myModal"
>
  Open modal
</button>

<!-- The Modal -->
<div class="modal fade" id="myModal">
  <div class="modal-dialog">
    <div class="modal-content">
      <!-- Modal Header -->
      <div class="modal-header">
        <h4 class="modal-title">Modal Heading</h4>
        <button
          type="button"
          class="btn-close"
          data-bs-dismiss="modal"
        ></button>
      </div>

      <!-- Modal body -->
      <div class="modal-body">Modal body..</div>

      <!-- Modal footer -->
      <div class="modal-footer">
        <button type="button" class="btn btn-danger" data-bs-dismiss="modal">
          Close
        </button>
      </div>
    </div>
  </div>
</div>
```

- Sử dụng class `.fade` để thêm hiệu ứng mờ dần khi mở và đóng modal
- **Modal Size**

  - Thay đổi kích thước của modal bằng cách thêm class `.modal-sm` cho modal nhỏ (max-width 300px), class `.modal-lg` cho modal lớn (max-width 800px) hoặc `.modal-xl` cho modal cực lớn (tối đa -chiều rộng 1140px). Mặc định là max-width 500px.
  - Thêm class kích thước vào phần tử `<div>` với hộp thoại `.modal-class`
  - VD: `<div class="modal-dialog modal-sm">`

- **Fullscreen Modals**

  - Nếu bạn muốn modal kéo dài toàn bộ chiều rộng và chiều cao của trang, hãy sử dụng class `.modal-fullscreen`
  - VD: `<div class="modal-dialog modal-fullscreen">`

- **Responsive Fullscreen Modals**

  - Bạn cũng có thể kiểm soát khi nào modal ở chế độ toàn màn hình với các class `.modal-fullscreen-*-*`

    | Class                      | Description                         |
    | -------------------------- | ----------------------------------- |
    | .modal-fullscreen-sm-down  | fullscreen nếu màn hình dưới 576px  |
    | .modal-fullscreen-md-down  | fullscreen nếu màn hình dưới 768px  |
    | .modal-fullscreen-lg-down  | fullscreen nếu màn hình dưới 992px  |
    | .modal-fullscreen-xl-down  | fullscreen nếu màn hình dưới 1200px |
    | .modal-fullscreen-xxl-down | fullscreen nếu màn hình dưới 1400px |

- **Centered Modal**
  - Căn giữa modal theo chiều dọc và chiều ngang trong trang với class `.modal-dialog-centered`
  - VD: `<div class="modal-dialog modal-dialog-centered">`
- **Scrolling Modal**
  - Khi bạn có nhiều nội dung bên trong modal một thanh cuộn sẽ được thêm vào trang.
  - Tuy nhiên, có thể bạn chỉ muốn cuộn bên trong modal thay vì ở trong trang thì sử dụng class `.modal-dialog-scrollable` vào `.modal-dialog`
  - VD: `<div class="modal-dialog modal-dialog-scrollable">`

## Bootstrap 5 Tooltip

- tooltip là một hộp thoại nhỏ được xuất hiện khi người dùng di chuyển con trỏ chuột qua một phần tử.
- Để tạo tooltip, hãy thêm thuộc tính `data-bs-toggle = "tooltip"` vào một phần tử.
- Sử dụng thuộc tính `title` để chỉ định văn bản sẽ được hiển thị bên trong tooltip
- VD: `<button type="button" class="btn btn-primary" data-bs-toggle="tooltip" title="Hooray!">Hover over me!</button>`
- Lưu ý: tooltip phải được khởi tạo bằng JavaScript để hoạt động.
- Đoạn code sau sẽ kích hoạt tất cả các tooltip trong tài liệu:
  ```javascript
  var tooltipTriggerList = [].slice.call(
    document.querySelectorAll('[data-bs-toggle="tooltip"]')
  );
  var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
    return new bootstrap.Tooltip(tooltipTriggerEl);
  });
  ```
- **Positioning Tooltips**

  - Theo mặc định, tooltip sẽ xuất hiện bên trên phần tử. Sử dụng thuộc tính `data-bs-position` để đặt vị trí của tooltip
  - VD:

  ```htm
  <a href="#" data-bs-toggle="tooltip" data-bs-placement="top" title="Hooray!"
    >Hover</a
  >
  <a
    href="#"
    data-bs-toggle="tooltip"
    data-bs-placement="bottom"
    title="Hooray!"
    >Hover</a
  >
  <a href="#" data-bs-toggle="tooltip" data-bs-placement="left" title="Hooray!"
    >Hover</a
  >
  <a href="#" data-bs-toggle="tooltip" data-bs-placement="right" title="Hooray!"
    >Hover</a
  >
  ```

## Bootstrap 5 Popover

- Popover gần giống tooltip nó là một hộp chú giải xuất hiện khi người dùng nhấp vào một phần tử. Sự khác biệt là Popover có thể chứa nhiều nội dung hơn.
- Để tạo Popover, hãy thêm thuộc tính `data-bs-toggle = "popover"` vào một phần tử.
- Sử dụng thuộc tính `title` để chỉ định văn bản tiêu đề của popover và sử dụng thuộc tính `data-bs-content` để chỉ định văn bản nội dung của popover
- VD `<button type="button" class="btn btn-primary" data-bs-toggle="popover" title="Popover Header" data-bs-content="Some content inside the popover">Toggle popover</button>`
- Lưu ý: Các popover phải được khởi tạo bằng JavaScript để hoạt động.
- Đoạn code sau sẽ kích hoạt tất cả các popover trong tài liệu:

```javascript
var popoverTriggerList = [].slice.call(
  document.querySelectorAll('[data-bs-toggle="popover"]')
);
var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
  return new bootstrap.Popover(popoverTriggerEl);
});
```

- **Positioning Popovers**

  - Theo mặc định, popover sẽ xuất hiện ở phía bên phải của phần tử. Sử dụng thuộc tính data-bs-position để xác định vị trí của popover

  ```htm
  <a
    href="#"
    title="Header"
    data-bs-toggle="popover"
    data-bs-placement="top"
    data-content="Content"
    >Top</a
  >
  <a
    href="#"
    title="Header"
    data-bs-toggle="popover"
    data-bs-placement="bottom"
    data-content="Content"
    >Bottom</a
  >
  <a
    href="#"
    title="Header"
    data-bs-toggle="popover"
    data-bs-placement="left"
    data-content="Content"
    >Left</a
  >
  <a
    href="#"
    title="Header"
    data-bs-toggle="popover"
    data-bs-placement="right"
    data-content="Content"
    >Right</a
  >
  ```

  - Lưu ý: Các thuộc tính vị trí không hoạt động như bạn mong đợi nếu nó không đủ chỗ cho chúng. Ví dụ: nếu bạn sử dụng vị trí trên cùng ở đầu trang (nơi nó không còn chỗ cho nó), thay vào đó nó sẽ hiển thị popover bên dưới phần tử hoặc bên phải (bất cứ nơi nào có chỗ cho nó)

- **Closing Popovers**

  - Theo mặc định, popover bị đóng khi bạn nhấp lại vào phần tử. Tuy nhiên, bạn có thể sử dụng thuộc tính `data-bs-trigger = "focus"`, thuộc tính này sẽ đóng popover khi nhấp vào bên ngoài phần tử.
  - VD: `<a href="#" title="Dismissible popover" data-bs-toggle="popover" data-bs-trigger="focus" data-bs-content="Click anywhere in the document to close this popover">Click me</a>`

- **Hoverable Popover**
  - Nếu bạn muốn popover được hiển thị khi bạn di chuyển con trỏ chuột qua phần tử, hãy sử dụng thuộc tính `data-bs-trigger` với giá trị "hover"
  - VD: `<a href="#" title="Dismissible popover" data-bs-toggle="popover" data-bs-trigger="hover" data-bs-content="Click anywhere in the document to close this popover">Click me</a>`

## Bootstrap 5 Toasts

- Toast là một hộp cảnh báo chỉ được hiển thị trong vài giây khi có điều gì đó xảy ra (khi người dùng nhấp vào nút, gửi biểu mẫu, v.v.)
- Để tạo Toast, hãy sử dụng class `.toast` và thêm `.toast-header` và `.toast-body` bên trong nó.
- Lưu ý: Toast được ẩn theo mặc định. Sử dụng class `.show` nếu bạn muốn hiển thị nó. Để đóng nó, hãy sử dụng phần tử `<button>` và thêm `data-bs-allow = "toast"`

```htm
<div class="toast show">
  <div class="toast-header">
    Toast Header
    <button type="button" class="btn-close" data-bs-dismiss="toast"></button>
  </div>
  <div class="toast-body">Some text inside the toast body</div>
</div>
```

- **Open a Toast**

  - Để hiển thị toast bằng một lần nhấp vào nút, bạn phải khởi tạo nó bằng JavaScript: chọn phần tử được chỉ định và gọi phương thức `toast()`.
  - Đoạn mã sau sẽ hiển thị tất cả toast trong tài liệu khi bạn nhấp vào một nút:

  ```javascript
  document.getElementById("toastbtn").onclick = function () {
    var toastElList = [].slice.call(document.querySelectorAll(".toast"));
    var toastList = toastElList.map(function (toastEl) {
      return new bootstrap.Toast(toastEl);
    });
    toastList.forEach((toast) => toast.show());
  };
  ```

## Bootstrap 5 Scrollspy

- Scrollspy được sử dụng để tự động cập nhật các liên kết trong danh sách điều hướng dựa trên vị trí cuộn.

```htm
<!-- The scrollable area -->
<body data-bs-spy="scroll" data-bs-target=".navbar" data-bs-offset="50">

<!-- The navbar - The <a> elements are used to jump to a section in the scrollable area -->
<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top">
...
  <ul class="navbar-nav">
    <li><a href="#section1">Section 1</a></li>
    ...
</nav>

<!-- Section 1 -->
<div id="section1">
  <h1>Section 1</h1>
  <p>Try to scroll this page and look at the navigation bar while scrolling!</p>
</div>
...

</body>
```

- Thêm `data-bs-spy = "scroll"` vào phần tử sẽ được sử dụng làm vùng có thể cuộn (thường là phần tử `<body>`).
- Sau đó, thêm thuộc tính `data-bs-target` với giá trị là id hoặc tên lớp của thanh điều hướng (`.navbar`). Điều này là để đảm bảo rằng thanh điều hướng được kết nối với vùng có thể cuộn.
- Lưu ý rằng các phần tử có thể cuộn phải khớp với ID của các liên kết bên trong các mục danh sách của thanh điều hướng (`<div id = "section1">` khớp với `<a href="#section1">`).
- Thuộc tính `data-bs-offset` tùy chọn chỉ định số lượng pixel cần bù từ trên cùng khi tính toán vị trí của cuộn. Điều này hữu ích khi bạn cảm thấy rằng các liên kết bên trong thanh điều hướng thay đổi trạng thái hoạt động quá sớm hoặc quá sớm khi chuyển đến các phần tử có thể cuộn. Mặc định là 10 pixel.
- Phần tử có `data-bs-spy = "scroll"` yêu cầu thuộc tính CSS position với giá trị "relative" để hoạt động bình thường.

## Bootstrap 5 Offcanvas

- Offcanvas tương tự như các modals (ẩn theo mặc định và hiển thị khi được kích hoạt), ngoại trừ nó thường được sử dụng làm menu điều hướng thanh bên.

```htm
<!-- Offcanvas Sidebar -->
<div class="offcanvas offcanvas-start" id="demo">
  <div class="offcanvas-header">
    <h1 class="offcanvas-title">Heading</h1>
    <button
      type="button"
      class="btn-close text-reset"
      data-bs-dismiss="offcanvas"
    ></button>
  </div>
  <div class="offcanvas-body">
    <p>Some text lorem ipsum.</p>
    <p>Some text lorem ipsum.</p>
    <button class="btn btn-secondary" type="button">A Button</button>
  </div>
</div>

<!-- Button to open the offcanvas sidebar -->
<button
  class="btn btn-primary"
  type="button"
  data-bs-toggle="offcanvas"
  data-bs-target="#demo"
>
  Open Offcanvas Sidebar
</button>
```

- class `.offcanvas` tạo thanh bên offcanvas.
- class `.offcanvas-start` định vị các offcanvas và làm cho nó có chiều rộng 400px. Xem ví dụ bên dưới để biết thêm các class định vị.
- class `.offcanvas-title` đảm bảo lề và chiều cao dòng thích hợp.
- Sau đó, thêm nội dung của bạn vào bên trong class `.offcanvas-body.`
- Để mở thanh bên offcanvas, bạn phải sử dụng `<button>` hoặc một phần tử `<a>` trỏ đến id của vùng chứa `.offcanvas` (#demo trong ví dụ trên).
- Để mở thanh bên offcanvas có phần tử `<a>`, bạn có thể trỏ tới `#demo` bằng thuộc tính `href`, thay vì thuộc tính `data-bs-target`.

- **Offcanvas Position**
  - Sử dụng .offcanvas-start | end | top | bottom để định vị các offcanvas sang trái, phải, trên hoặc dưới
  - VD: `<div class="offcanvas offcanvas-top" id="demo">`