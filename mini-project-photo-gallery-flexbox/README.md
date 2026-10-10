# Mini Project - Photo Gallery bằng Flexbox

## Mục tiêu

Xây dựng thư viện ảnh responsive bằng Flexbox mà không cần Media Query.

## Các bước đã thực hiện

### Bước 1 - Tạo cấu trúc HTML

Tạo file gallery.html.

Bên trong tạo:

- page-header
- gallery-container
- 9 gallery-item
- mỗi gallery-item chứa một ảnh
- gallery-caption
- footer

### Bước 2 - Reset CSS

Sử dụng:

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

### Bước 3 - Kích hoạt Flexbox

Trong gallery-container sử dụng:

display: flex;

### Bước 4 - Cho phép xuống hàng

Sử dụng:

flex-wrap: wrap;

Khi không đủ không gian,
các gallery-item tự động chuyển xuống dòng tiếp theo.

### Bước 5 - Căn chỉnh và tạo khoảng cách

Sử dụng:

justify-content: center;

gap: 16px;

### Bước 6 - Làm item linh hoạt

Sử dụng:

flex: 1 1 300px;

Ý nghĩa:

- flex-grow = 1
- flex-shrink = 1
- flex-basis = 300px

Các item có thể tự động lớn lên hoặc co lại tùy không gian.

### Bước 7 - Làm ảnh lấp đầy item

Sử dụng:

width: 100%;
height: 100%;
object-fit: cover;

object-fit: cover giúp ảnh không bị méo.

### Bước 8 - Thêm hiệu ứng hover

Khi hover:

- gallery-item được nâng lên
- ảnh zoom nhẹ
- ảnh tối nhẹ
- caption hiện rõ hơn

### Bước 9 - Kiểm tra responsive

Thu nhỏ cửa sổ trình duyệt.

Flexbox tự động thay đổi số lượng cột mà không cần Media Query.

Ví dụ:

Desktop:
3 hoặc nhiều item trên một hàng.

Tablet:
2 item trên một hàng.

Mobile:
1 item hoặc các item nhỏ hơn tùy kích thước màn hình.

## Cấu trúc project

mini-project-photo-gallery-flexbox
|
|-- gallery.html
|-- style.css
|-- README.md

## Kiến thức Flexbox sử dụng

- display: flex
- flex-wrap: wrap
- justify-content
- gap
- flex-grow
- flex-shrink
- flex-basis
- flex shorthand
