# Bootstrap Grid

## Bootstrap 5 Grid System

- **The Grid System**

  - Hệ thống grid đáp ứng và các cột sẽ tự động sắp xếp lại tùy thuộc vào kích thước màn hình.
  - Đảm bảo rằng tổng cộng tối đa 12 hoặc ít hơn (không bắt buộc bạn phải sử dụng tất cả 12 cột có sẵn).

- **Grid Classes**
  - Hệ thống lưới Bootstrap 5 có sáu lớp
    - .col- (thiết bị cực nhỏ - chiều rộng màn hình nhỏ hơn 576px)
    - .col-sm- (thiết bị nhỏ - chiều rộng màn hình bằng hoặc lớn hơn 576px)
    - .col-md- (thiết bị trung bình - chiều rộng màn hình bằng hoặc lớn hơn 768px)
    - .col-lg- (thiết bị lớn - chiều rộng màn hình bằng hoặc lớn hơn 992px)
    - .col-xl- (thiết bị phóng to - chiều rộng màn hình bằng hoặc lớn hơn 1200px)
    - .col-xxl- (thiết bị xxlarge - chiều rộng màn hình bằng hoặc lớn hơn 1400px)
  - Các lớp trên có thể được kết hợp để tạo ra các bố cục năng động và linh hoạt hơn.
  - Mẹo: Mỗi lớp mở rộng quy mô, vì vậy nếu bạn muốn đặt cùng độ rộng cho sm và md, bạn chỉ cần chỉ định sm.

## Bootstrap 5 Grid Stacked to horizontal

- **Stacked-to-horizontal**

  - Ví dụ sau cho thấy bố cục hai cột đơn giản "xếp chồng lên nhau", có nghĩa là nó sẽ dẫn đến sự phân chia 50%/50% trên tất cả các màn hình, ngoại trừ các màn hình nhỏ sm, nó sẽ tự động xếp chồng (100%)

  ```htm
  <div class="container-fluid">
    <div class="row">
      <div class="col-sm-6 bg-primary">
        <p>Lorem ipsum...</p>
      </div>
      <div class="col-sm-6 bg-dark">
        <p>Sed ut perspiciatis...</p>
      </div>
    </div>
  </div>
  ```

 - Mẹo: Bạn có thể biến bất kỳ bố cục có chiều rộng full thành bố cục đáp ứng có chiều rộng cố định bằng cách thay đổi class `.container-liquid` thành `.container`

- **Auto Layout Columns**
  - Trong Bootstrap 5, có một cách dễ dàng để tạo các cột có chiều rộng bằng nhau cho tất cả các thiết bị: chỉ cần xóa số khỏi `.col-size-*` và chỉ sử dụng class `.col-size` trên một số phần tử col được chỉ định. Bootstrap sẽ nhận biết có bao nhiêu cột và mỗi cột sẽ có cùng chiều rộng. Các lớp kích thước (sm, md, v.v.) xác định khi nào các cột phải đáp ứng.