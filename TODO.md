# TODO - Hoàn thiện theo README (AES-128 Lab)

## Step 1: Đối chiếu yêu cầu README vs code
- [x] Đọc `README.md`, `encrypt.cpp`, `decrypt.cpp`, `structures.h`, `report-1page.md`, `Makefile`, `.github/scripts/check_submission.sh`
- [ ] Xác định các chỗ code sai mô tả liên quan đến binary I/O ciphertext

## Step 2: Sửa code I/O ciphertext cho đúng binary
- [ ] `encrypt.cpp`: ghi ciphertext ra `message.aes` bằng `.write()` (không dùng `operator<<` cho bytes)
- [ ] `encrypt.cpp`: in hex đúng định dạng (0-padded 2 digits)
- [ ] `decrypt.cpp`: đọc `message.aes` bằng `.read()` để lấy đúng số byte file
- [ ] `decrypt.cpp`: decrypt theo kích thước file / 16 block


## Step 3: Sync cách mô tả/format với README + report
- [x] Cập nhật `README.md` phần input/output/padding/ciphertext byte
- [x] Cập nhật `report-1page.md` đoạn mô tả kết quả/cách viết/đọc ciphertext


## Step 4: Rà soát tests/logs (không chạy lệnh nhưng đảm bảo logic khớp)
- [x] Kiểm tra `tests/*.sh` và cập nhật logic phù hợp binary-safe I/O trong code
- [x] Kiểm tra `logs/` (không thay đổi bắt buộc)

## Step 5: Kết thúc
- [x] Đảm bảo không còn mismatch giữa code, README và script check


