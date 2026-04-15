# Run Log – FIT4012 Lab 1

## Entropy / Redundancy
- [x] Đã chạy với input `aaaa`
- [x] Đã chạy với input `abcd`
- [x] Đã chạy với input `hello world`

## Modulo inverse
- [x] Đã chạy với `3 7`
- [x] Đã chạy với `10 17`
- [x] Đã chạy với `6 9`

## Điều em học được từ bài lab
Thông qua bài lab này, em đã chuyển hóa thành công các công thức toán học trừu tượng thành mã nguồn thực tế. Điều em nhận thấy thú vị nhất là việc thấy rõ nghịch lý: chuỗi càng dễ đoán (như `aaaa`) thì Entropy càng thấp và độ dư thừa càng cao.

Khó khăn lớn nhất trong quá trình cài đặt là thao tác với các phép chia lấy dư số âm trong C++. Toán học cho phép số dư âm, nhưng trong mật mã học ta cần số dư dương. Việc áp dụng biểu thức `(x % m + m) % m` ở bước cuối của hàm `mod_inverse()` đã giúp em giải quyết triệt để vấn đề này. Bài lab cũng giúp em làm quen hơn với quy trình làm việc chuyên nghiệp qua GitHub.
