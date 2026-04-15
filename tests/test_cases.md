# Test cases – FIT4012 Lab 1

Đánh dấu [x] khi đã chạy và kiểm tra kết quả.

## 1. Entropy / Redundancy
- [x] Input: `aaaa` -> entropy thấp, redundancy cao
- [x] Input: `abcd` -> entropy cao hơn `aaaa`
- [x] Input: `hello world` -> entropy và redundancy được tính hợp lệ

## 2. Modulo inverse
- [x] `a=3, m=7` -> nghịch đảo modulo là 5
- [x] `a=10, m=17` -> nghịch đảo modulo là 12
- [x] `a=6, m=9` -> không tồn tại nghịch đảo modulo

## 3. Ghi chú
### 3.1 Mở rộng test Entropy / Redundancy
- [ ] Input: `abababab` -> Chuỗi có 2 ký tự lặp đều nhau (Kỳ vọng: Entropy = 1.0, Redundancy = 7.0).
- [ ] Input: `12345678` -> Chuỗi gồm 8 ký tự hoàn toàn khác biệt (Kỳ vọng: Entropy = 3.0, Redundancy = 5.0).
- [ ] Input: `    ` (4 dấu cách) -> Chuỗi chỉ chứa dấu cách (Kỳ vọng: Entropy = 0.0, Redundancy = 8.0).

### 3.2 Mở rộng test Modulo inverse
- [ ] `a=17, m=101` -> Nghịch đảo modulo là 6 (Kiểm tra với modulus là số nguyên tố lớn).
- [ ] `a=23, m=120` -> Nghịch đảo modulo là 47 (Kiểm tra xem hàm xử lý số lớn có bị tràn hay sai số không).
- [ ] `a=15, m=25` -> Không tồn tại nghịch đảo modulo (Kiểm tra trường hợp $\gcd(a, m) = 5 > 1$).