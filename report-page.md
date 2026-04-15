# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
- Cài đặt và tính toán Entropy, độ dư thừa thông tin của một chuỗi ký tự.
- Cài đặt thuật toán Euclid mở rộng để tìm nghịch đảo modulo.
- Rèn luyện kỹ năng sử dụng Git/GitHub để quản lý mã nguồn và viết báo cáo.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|--------:|-----------:|---|
| aaaa |       0 |          8 |  |
| abcd |       2 |          6 |  |
| hello world | 2.84535 |    5.15465 |  |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|----------------------|
| 3 | 7 | 5 | 5                    |
| 10 | 17 | 12 | 12                   |
| 6 | 9 | Không tồn tại | Không tồn tại        |

## 4. Kết luận
Thông qua bài lab này, em đã chuyển hóa thành công các công thức toán học trừu tượng thành mã nguồn thực tế. Điều em nhận thấy thú vị nhất là việc thấy rõ nghịch lý: chuỗi càng dễ đoán (như `aaaa`) thì Entropy càng thấp và độ dư thừa càng cao.

Khó khăn lớn nhất trong quá trình cài đặt là thao tác với các phép chia lấy dư số âm trong C++. Toán học cho phép số dư âm, nhưng trong mật mã học ta cần số dư dương. Việc áp dụng biểu thức `(x % m + m) % m` ở bước cuối của hàm `mod_inverse()` đã giúp em giải quyết triệt để vấn đề này. Bài lab cũng giúp em làm quen hơn với quy trình làm việc chuyên nghiệp qua GitHub.