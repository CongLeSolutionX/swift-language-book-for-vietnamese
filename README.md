# Ngôn Ngữ Lập Trình Swift

Cuốn sách "Ngôn Ngữ Lập Trình Swift" cho người Việt.
Repo này là bản clone của [phiên bản chính thức].

Repository này chứa nguồn của *Ngôn Ngữ Lập Trình Swift*
(thỉnh thoảng được viết tắt là TSPL),
được xuất bản trên [docs.swift.org][published]
và được xây dựng sử dụng [Swift-DocC][docc].

## Đóng Góp

Đối với những thay đổi nhỏ,
như sửa lỗi chính tả và các đoạn văn ngắn,
hãy fork repository này và tạo một pull request.

Quá trình đóng góp chính thức cho tài liệu này vẫn đang được phát triển.
Trong thời gian chờ đợi,
bắt đầu một chuỗi thảo luận tại [Diễn đàn Swift][forum] cho những thay đổi lớn
để thảo luận về phương hướng và xác định các vấn đề tiềm ẩn
trước khi bạn dành nhiều thời gian vào viết lách.

Nội dung trong cuốn sách này tuân theo [Hướng Dẫn Phong Cách của Apple][asg]
và [hướng dẫn phong cách của cuốn sách này][tspl-style].

Báo cáo lỗi về nội dung sử dụng [trang vấn đề][bugs] trên Github.

Thảo luận và đóng góp tuân theo [Quy tắc Ứng xử của Swift][conduct].

Để biết thêm thông tin, xem [Đóng góp vào Ngôn Ngữ Lập Trình Swift][contributing].

[asg]: https://help.apple.com/applestyleguide/
[bugs]: https://github.com/apple/swift-book/issues
[conduct]: https://www.swift.org/code-of-conduct
[contributing]: /CONTRIBUTING.md
[forum]: https://forums.swift.org/c/swift-documentation/92
[tspl-style]: /Style.md
[published]: https://docs.swift.org/swift-book/documentation/the-swift-programming-language/
[docc]: https://github.com/apple/swift-docc
[phiên bản chính thức]: https://github.com/apple/swift-book

## Xây Dựng

Chạy lệnh `docc preview TSPL.docc`
trong thư mục gốc của repository này.

Sau khi chạy DocC, mở liên kết mà `docc` tạo ra
để xem trước nội dung trên trình duyệt của bạn.

> Lưu ý:
>
> Nếu bạn cài đặt DocC bằng cách tải toolchain từ Swift.org,
> `docc` nằm trong `usr/bin/`,
> tương đối với đường dẫn cài đặt của toolchain.
> Đảm bảo rằng biến môi trường `PATH` của shell của bạn
> bao gồm thư mục đó.
>
> Nếu bạn cài đặt DocC bằng cách tải Xcode,
> chạy `xcrun docc preview TSPL.docc` thay vì lệnh trước.