# Bootstrap Form

## Bootstrap 5 Forms

- **Stacked Form**

  - Tất cả các phần tử `<input>` và `<textarea>` có class `.form-control` đều được style phù hơp
  - lưu ý rằng class `.form-label` ở mỗi phần tử label để đảm bảo padding chính xác.
  - Các checkbox có đánh dấu khác nhau. Chúng được bao bọc xung quanh phần tử vùng chứa bằng `.form-check` và các label có class `.form-check-label`, trong khi các checkbox và radio button sử dụng `.form-check-input`.

  ```htm
  <form action="/action_page.php">
    <div class="mb-3 mt-3">
      <label for="email" class="form-label">Email:</label>
      <input
        type="email"
        class="form-control"
        id="email"
        placeholder="Enter email"
        name="email"
      />
    </div>
    <div class="mb-3">
      <label for="pwd" class="form-label">Password:</label>
      <input
        type="password"
        class="form-control"
        id="pwd"
        placeholder="Enter password"
        name="pswd"
      />
    </div>
    <div class="mb-3">
      <label for="comment">Comments:</label>
      <textarea
        class="form-control"
        rows="5"
        id="comment"
        name="text"
      ></textarea>
    </div>
    <div class="form-check mb-3">
      <label class="form-check-label">
        <input class="form-check-input" type="checkbox" name="remember" />
        Remember me
      </label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
  ```

- **Form Row/Grid (Inline Forms)**

  - Nếu bạn muốn các phần tử của form cạnh nhau, hãy sử dụng `.row` và `.col`

  ```htm
  <form>
    <div class="row">
      <div class="col">
        <input
          type="text"
          class="form-control"
          placeholder="Enter email"
          name="email"
        />
      </div>
      <div class="col">
        <input
          type="password"
          class="form-control"
          placeholder="Enter password"
          name="pswd"
        />
      </div>
    </div>
  </form>
  ```

- **Form Control Size**

  - Bạn có thể thay đổi kích thước của input `.form-control` bằng `.form-control-lg` hoặc `.form-control-sm`
  - VD: `<input type="text" class="form-control form-control-lg" placeholder="Large input">`

- **Disabled and Readonly**

  - Sử dụng các thuộc tính disabled/readonly để làm cho input tắt hoặc ở trạng thái chỉ đọc

- **Plain text Inputs**

  - sử dụng class `.form-control-plaintext` để tạo style cho input không có đường viền, nhưng giữ margin và padding thích hợp

- **Color Picker**
  - Để tạo style input đúng với `type = "color"`, hãy sử dụng class `.form-control-color`
  - VD: `<input type="color" class="form-control form-control-color" value="#CCCCCC">`

## Bootstrap 5 Select

- **Select Menu**

  - Để tạo style cho select menu trong Bootstrap 5, hãy thêm class `.form-select` vào phần tử `<select>`
  - nếu muốn chọn nhiều element cùng lúc thì chỉ cần thêm thuộc tính `multiple`

  ```htm
  <label for="sel2" class="form-label">
    Mutiple select list (hold shift to select more than one)
  </label>
  <select multiple class="form-select" id="sel2" name="sellist2">
    <option>1</option>
    <option>2</option>
    <option>3</option>
    <option>4</option>
    <option>5</option>
  </select>
  ```

- **Select Menu Size**
  - chỉ cần dùng class `.form-select-lg` hoặc `.form-select-sm` để thay đổi kích thước của select menu
- **Disabled Select Menu**
  - chỉ cần thêm thuộc tính `disabled` để vô hiệu hoá select Menu
- **Data Lists**

  - Bootstrap cũng sẽ tạo kiểu cho danh sách dữ liệu, đây là danh sách các tùy chọn được xác định trước cho phần tử `<input>`

  ```htm
  <label for="browser" class="form-label"
    >Choose your browser from the list:</label
  >
  <input class="form-control" list="browsers" name="browser" id="browser" />
  <datalist id="browsers">
    <option value="Edge"></option>
    <option value="Firefox"></option>
    <option value="Chrome"></option>
    <option value="Opera"></option>
    <option value="Safari"></option>
  </datalist>
  ```

## Bootstrap 5 Checkboxes and Radio buttons

- **Checkboxes**

  - Để tạo kiểu cho checkbox, hãy sử dụng phần tử `<div>` với class = "form-check" để đảm bảo margin thích hợp cho label và checkbox.
  - Sau đó, thêm class `.form-check-label` vào các phần tử label và `.form-check-input` vào phần tử checkbox đúng bên trong div `.form-check`.
  - Sử dụng thuộc tính `checked` nếu bạn muốn hộp kiểm được chọn theo mặc định.

  ```htm
  <div class="form-check">
    <input
      class="form-check-input"
      type="checkbox"
      id="check1"
      name="option1"
      value="something"
      checked
    />
    <label class="form-check-label">Option 1</label>
  </div>
  ```

- **Radio buttons**

  - sử dụng giống checkbox nhưng chỉ định người dùng chỉ được chọn 1 phần tử
  - lưu ý: thuộc tính `name` phải giống nhau

- **Toggle Switches**

  - Nếu bạn muốn checkbox có style như một công tắc bật/tắt, hãy sử dụng class `.form-switch` cùng với `.form-check`

  ```htm
  <div class="form-check form-switch">
    <input
      class="form-check-input"
      type="checkbox"
      id="mySwitch"
      name="darkmode"
      value="yes"
      checked
    />
    <label class="form-check-label" for="mySwitch">Dark Mode</label>
  </div>
  ```

## Bootstrap 5 Range

- **Custom Range**
  - Để style cho input Range, hãy thêm class `.form-range` vào phần tử input có type = "range"
  ```htm
  <label for="customRange" class="form-label">Custom range</label>
  <input type="range" class="form-range" id="customRange" />
  ```
- **Steps**
  - Theo mặc định, khoảng cách giữa các số trong phạm vi là 1. Bạn có thể thay đổi nó bằng cách sử dụng thuộc tính `step`
  - VD: `<input type="range" class="form-range" step="10">`
- **Min and Max**
  - Theo mặc định, giá trị nhỏ nhất là 0 và giá trị lớn nhất là 100. Bạn có thể sử dụng thuộc tính `min` / `max` để thay đổi nó
  - VD: `<input type="range" class="form-range" min="0" max="4">`

## Bootstrap 5 Input Groups

- **Input Groups**

  - class `.input-group` là div chứa để nâng cao đầu vào bằng cách thêm biểu tượng, văn bản hoặc nút vào phía trước hoặc phía sau trường nhập dưới dạng "văn bản trợ giúp".
  - Để tạo kiểu cho văn bản trợ giúp đã chỉ định, hãy sử dụng class `.input-group-text`

  ```htm
  <form>
    <div class="input-group">
      <span class="input-group-text">@</span>
      <input type="text" class="form-control" placeholder="Username" />
    </div>

    <div class="input-group">
      <input type="text" class="form-control" placeholder="Your Email" />
      <span class="input-group-text">@example.com</span>
    </div>
  </form>
  ```

- **Input Group Size**
  - Sử dụng class `.input-group-sm` cho nhóm input nhỏ và `.input-group-lg` cho nhóm input lớn
- **Multiple Inputs and Helpers**

  - có thể thêm nhiều phần bổ trợ hoặc nhiều input như sau

  ```htm
  <!-- Multiple inputs -->
  <div class="input-group mb-3">
    <span class="input-group-text">Person</span>
    <input type="text" class="form-control" placeholder="First Name" />
    <input type="text" class="form-control" placeholder="Last Name" />
  </div>

  <!-- Multiple addons / help text -->
  <div class="input-group mb-3">
    <span class="input-group-text">One</span>
    <span class="input-group-text">Two</span>
    <span class="input-group-text">Three</span>
    <input type="text" class="form-control" />
  </div>
  ```

- **Input Group with Checkboxes and Radios**

  - Bạn cũng có thể sử dụng checkbox hoặc radio thay vì text

  ```htm
  <div class="input-group mb-3">
    <div class="input-group-text">
      <input type="checkbox" />
    </div>
    <input type="text" class="form-control" placeholder="Some text" />
  </div>

  <div class="input-group mb-3">
    <div class="input-group-text">
      <input type="radio" />
    </div>
    <input type="text" class="form-control" placeholder="Some text" />
  </div>
  ```

- **Input Group Buttons**

```htm
<div class="input-group mb-3">
  <button class="btn btn-outline-primary" type="button">Basic Button</button>
  <input type="text" class="form-control" placeholder="Some text" />
</div>

<div class="input-group mb-3">
  <input type="text" class="form-control" placeholder="Search" />
  <button class="btn btn-success" type="submit">Go</button>
</div>

<div class="input-group mb-3">
  <input type="text" class="form-control" placeholder="Something clever.." />
  <button class="btn btn-primary" type="button">OK</button>
  <button class="btn btn-danger" type="button">Cancel</button>
</div>
```

- **Input Group with Dropdown Button**

```htm
<div class="input-group mt-3 mb-3">
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
  <input type="text" class="form-control" placeholder="Username" />
</div>
```

## Bootstrap 5 Form Floating Labels

- **Floating Labels / Animated Labels**

  - Theo mặc định, khi sử dụng label, chúng thường xuất hiện ở đầu input
  - với Floating Labels, bạn có thể chèn label bên trong input và làm cho chúng nổi lên trên (animation) khi bạn click vào input

  ```htm
  <div class="form-floating mb-3 mt-3">
    <input
      type="text"
      class="form-control"
      id="email"
      placeholder="Enter email"
      name="email"
    />
    <label for="email">Email</label>
  </div>

  <div class="form-floating mt-3 mb-3">
    <input
      type="text"
      class="form-control"
      id="pwd"
      placeholder="Enter password"
      name="pswd"
    />
    <label for="pwd">Password</label>
  </div>
  ```
  - Lưu ý về Floating Labels: Các phần tử `<label>` phải đứng sau phần tử `<input>` và thuộc tính `placeholder` là bắt buộc cho mỗi phần tử `<input>` (ngay cả khi nó không được hiển thị).
- **Textarea**
  - hoạt động tương tự như input
- **Select Menus**
  - Bạn cũng có thể sử dụng "floating label" trên các select menu. Tuy nhiên, chúng sẽ không nổi (animation). label sẽ luôn xuất hiện ở góc trên cùng bên trái, bên trong select menu

## Bootstrap 5 Form Validation

- Bạn có thể sử dụng các class Validation khác nhau để cung cấp phản hồi có giá trị cho người dùng. Thêm `.was-validated` hoặc `.needs-validation` vào phần tử `<form>`, tùy thuộc vào việc bạn muốn cung cấp phản hồi xác thực trước hay sau khi gửi biểu mẫu. Các input sẽ có đường viền màu xanh lá cây (hợp lệ) hoặc màu đỏ (không hợp lệ) để cho biết những gì còn thiếu trong biểu mẫu. Bạn cũng có thể thêm thông báo `.valid-feedback` hoặc `.invalid-feedback` để cho người dùng biết rõ ràng những gì còn thiếu hoặc cần phải hoàn thành trước khi gửi biểu mẫu.
- Trong ví dụ này sử dụng `.was-validated` để validation trước khi gửi biểu mẫu.

```htm
<form action="/action_page.php" class="was-validated">
  <div class="mb-3 mt-3">
    <label for="uname" class="form-label">Username:</label>
    <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Please fill out this field.</div>
  </div>
  <div class="mb-3">
    <label for="pwd" class="form-label">Password:</label>
    <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Please fill out this field.</div>
  </div>
  <div class="form-check mb-3">
    <input class="form-check-input" type="checkbox" id="myCheck" name="remember" required>
    <label class="form-check-label" for="myCheck">I agree on blabla.</label>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Check this checkbox to continue.</div>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```
