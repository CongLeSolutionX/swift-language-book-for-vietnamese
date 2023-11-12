# Khả năng Tương Thích Phiên Bản

Tìm hiểu những chức năng nào có sẵn trong các chế độ ngôn ngữ cũ hơn.

Cuốn sách này mô tả Swift 5.9,
phiên bản mặc định của Swift được tích hợp trong Xcode 15.
Bạn có thể sử dụng Xcode 15 để xây dựng các target
được viết bằng Swift 5.9, Swift 4.2, hoặc Swift 4.

<!--
  - test: `swift-version`

  ```swifttest
  >> #if swift(>=5.9.1)
  >>     print("Too new")
  >> #elseif swift(>=5.9)
  >>     print("Just right")
  >> #else
  >>     print("Too old")
  >> #endif
  << Just right
  ```
-->

Khi bạn sử dụng Xcode 15 để xây dựng mã nguồn Swift 4 và Swift 4.2,
hầu hết các chức năng của Swift 5.9 đều có sẵn.
Tuy vậy, các thay đổi sau chỉ dành cho mã nguồn sử dụng Swift 5.9 trở lên:

- Các hàm trả về một loại opaque yêu cầu runtime Swift 5.1.
- Biểu thức `try?` không giới thiệu thêm một cấp độ tùy chọn nào 
  đối với các biểu thức đã trả về giá trị tùy chọn.
- Các biểu thức khởi tạo số nguyên lớn được suy luận
  để có kiểu số nguyên chính xác.
  Ví dụ, `UInt64(0xffff_ffff_ffff_ffff)` được đánh giá là giá trị chính xác
  thay vì tràn số.

Đồng bộ hóa yêu cầu Swift 5.9 hoặc phiên bản mới hơn,
và một phiên bản của thư viện chuẩn Swift
cung cấp các kiểu đồng bộ tương ứng.
Trên các nền tảng của Apple, đặt một mục tiêu triển khai
ít nhất là iOS 13, macOS 10.15, tvOS 13, hoặc watchOS 6.

Một target được viết bằng Swift 5.9 có thể phụ thuộc vào 
một target được viết bằng Swift 4.2 hoặc Swift 4,
và ngược lại.
Điều này có nghĩa là, nếu bạn có một dự án lớn
được chia thành nhiều framework,
bạn có thể chuyển đổi mã nguồn của mình từ Swift 4 sang Swift 5.9
từng framework một.

<!--
File nguồn này là một phần của dự án mã nguồn mở Swift.org

Bản quyền (c) 2014 - 2022 Apple Inc. và các tác giả dự án Swift
Được cấp phép theo giấy phép Apache v2.0 với Đặc lệ Thư viện Thời gian chạy

Xem https://swift.org/LICENSE.txt để biết thông tin về giấy phép
Xem https://swift.org/CONTRIBUTORS.txt để biết danh sách các tác giả dự án Swift
-->