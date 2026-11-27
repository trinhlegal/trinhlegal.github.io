# trinhlegal.com

Mã nguồn trang web **trinhlegal.com** của Trịnh Nguyễn Phương (Mr. Phương), hỗ trợ pháp lý tại Lào Cai.
Trang chạy bằng Jekyll trên GitHub Pages. Mọi thay đổi đẩy lên nhánh chính sẽ tự xuất bản sau khoảng 1 đến 3 phút.

## 1. Thông tin chung

| Mục | Nội dung |
|---|---|
| Tên miền | https://trinhlegal.com |
| Chuyên mục bài viết | https://trinhlegal.com/go-roi-phap-ly/ ("Gỡ rối pháp lý") |
| Nền tảng | Jekyll, GitHub Pages |
| Fanpage liên kết | Mr Phương - Hỗ trợ pháp lý Lào Cai |
| Người quản trị | Trịnh Nguyễn Phương |

## 2. Cấu trúc thư mục chính

| Thư mục, tệp | Vai trò |
|---|---|
| `_posts/` | Toàn bộ bài viết chuyên mục "Gỡ rối pháp lý", mỗi bài một tệp `.md` |
| `index.html` | Trang chủ (tự hiện 3 bài mới nhất) |
| `go-roi-phap-ly/index.html` | Trang danh sách bài của chuyên mục, có nút lọc theo mảng |
| `_layouts/bai-viet.html` | Khung trang bài viết (mọi bài trong `_posts` tự dùng) |
| `_layouts/trang.html` | Khung trang thường |
| `_includes/dau-trang.html`, `thanh-dieu-huong.html`, `chan-trang.html` | Đầu trang, menu, chân trang dùng chung |
| `_includes/chan-bai.html` | Chân bài, nút Zalo và gọi điện, tự gắn theo trường `nhom` |
| `_config.yml` | Cấu hình chung: tên trang, đường dẫn bài, tệp loại trừ không xuất bản |
| `CNAME` | Khai báo tên miền trinhlegal.com, không xóa, không sửa |

## 3. Cách đăng bài mới

**Bước 1.** Tạo tệp trong `_posts/`, tên dạng `YYYY-MM-DD-ten-bai-khong-dau.md`.
Ví dụ: `2026-11-27-di-chuc-tu-viet-hay-cong-chung.md`

**Bước 2.** Đầu tệp khai báo như sau:

```yaml
---
title: "Di chúc tự viết hay công chứng: điều kiện để di chúc không bị tuyên vô hiệu"
description: "Tóm tắt 1 đến 2 câu, hiện trên Google và khi chia sẻ Facebook, Zalo."
date: 2026-11-27 07:55:00 +0700
mang: "Thừa kế"
nhom: ca-nhan
can_cu_den_ngay: "27/11/2026"
---
```

| Trường | Giá trị cho phép |
|---|---|
| `mang` | Đất đai / Thừa kế / Hôn nhân gia đình / Lao động / Đăng ký kinh doanh / Dự án đầu tư |
| `nhom` | `ca-nhan` / `doanh-nghiep` / `lao-dong` (quyết định chân bài tự gắn) |
| `can_cu_den_ngay` | Ngày chốt kiểm tra văn bản pháp luật dẫn chiếu |

**Bước 3.** Viết nội dung bằng Markdown bên dưới phần khai báo. Không tự chèn chân bài, trang tự gắn theo `nhom`.

**Bước 4.** Commit và đẩy lên. Kiểm tra lại bài trên trang sau 2 đến 3 phút.

## 4. Lưu ý kỹ thuật

1. Giờ trong trường `date` phải sớm hơn thời điểm đẩy bài. GitHub Pages không hiện bài có ngày giờ tương lai.
2. Thứ tự bài sắp theo `date`, mới nhất lên đầu. Muốn đổi vị trí thì sửa giờ, không sửa tên tệp.
3. Trang chủ tự hiện 3 bài mới nhất.
4. Đường dẫn bài lấy theo phần chữ trong tên tệp (bỏ ngày), dạng `trinhlegal.com/go-roi-phap-ly/ten-bai/`. Đổi tên tệp sẽ đổi đường dẫn bài, làm hỏng link đã chia sẻ trên Fanpage. Hạn chế đổi tên sau khi đăng.
5. Bài không hiện: xem tab **Actions** trên GitHub, nếu có dấu đỏ thì mở lỗi để sửa (thường do sai cú pháp phần khai báo đầu tệp).

## 5. Quy ước commit

Ghi rõ việc đã làm để tra lại lịch sử:

- `Đăng bài: <tên ngắn>`
- `Đính chính bài: <tên ngắn> - <nội dung sửa>`
- `Giao diện: <nội dung sửa>`

## 6. Rà soát căn cứ pháp lý định kỳ

Mỗi bài ghi `can_cu_den_ngay`. Khi có văn bản mới thay thế, sửa đổi, phải cập nhật bài và đổi ngày này.

| Thời điểm | Việc cần làm |
|---|---|
| 01/01/2027 | Rà bài di chúc theo Luật số 04/2026/QH16 sửa đổi Luật Công chứng |
| Trước 28/02/2027 | Rà bài dự án khách sạn (thời hạn các nghị quyết đặc thù) |
| 01/3/2027 | Rà bài lao động theo luật sửa đổi Bộ luật Lao động |
| 01/7/2027 | Rà các bài đất đai, hôn nhân gia đình theo Luật Đất đai (sửa đổi) |

## 7. Kế hoạch 30 bài chuyên mục "Gỡ rối pháp lý"

Viết lần lượt theo số thứ tự, bỏ qua bài đã đăng. Ưu tiên nhóm 1 đến 4 (người dân, người lao động), nhóm 5 và 6 (doanh nghiệp) viết sau.
Sau khi đăng: đổi trạng thái bài trong bảng này thành "Đã đăng" kèm ngày, ghi đường dẫn bài.
Bài mới đăng sau phải xác định vị trí hiển thị trước khi đặt giờ trong trường `date`.

### Nhóm 1. Đất đai (`mang: Đất đai`, `nhom: ca-nhan`)
Mọi bài nhóm này có đoạn lưu ý Luật Đất đai (sửa đổi) thông qua 21/11/2026, hiệu lực 01/7/2027.

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 01 | Cấp Sổ đỏ lần đầu cho đất sử dụng ổn định không có giấy tờ | Đã đăng 26/11/2026 |
| 02 | Tách thửa đất ở: diện tích tối thiểu, lối đi chung, lỗi bị trả hồ sơ | Đã đăng 26/11/2026 |
| 03 | Chuyển đất vườn, ao sang đất ở: cách tính tiền sử dụng đất, hồ sơ | Chưa đăng |
| 04 | Mua đất giấy viết tay, vi bằng: rủi ro và hướng hợp thức hóa | Đã đăng 26/11/2026 |
| 05 | Tranh chấp ranh giới đất liền kề: hòa giải tại xã, phường và khởi kiện | Chưa đăng |

### Nhóm 2. Thừa kế (`mang: Thừa kế`, `nhom: ca-nhan`)

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 06 | Di chúc tự viết hay công chứng: điều kiện để di chúc không bị vô hiệu | Đã đăng 27/11/2026 |
| 07 | Chia thừa kế quyền sử dụng đất khi không có di chúc | Chưa đăng |
| 08 | Người thừa kế ở nước ngoài hoặc không hợp tác ký văn bản phân chia di sản | Chưa đăng |
| 09 | Người thừa kế không phụ thuộc nội dung di chúc | Chưa đăng |
| 10 | Tặng cho nhà đất hay để thừa kế: so sánh thuế, phí, rủi ro tranh chấp | Chưa đăng |

### Nhóm 3. Hôn nhân và gia đình (`mang: Hôn nhân gia đình`, `nhom: ca-nhan`)

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 11 | Nhà đất có trước và trong hôn nhân: tài sản chung hay tài sản riêng | Đã đăng 27/11/2026 |
| 12 | Thuận tình ly hôn và đơn phương ly hôn: hồ sơ, nơi nộp, thời gian | Chưa đăng |
| 13 | Giành quyền nuôi con khi ly hôn | Chưa đăng |
| 14 | Cấp dưỡng sau ly hôn và yêu cầu thi hành án khi một bên trốn tránh | Chưa đăng |
| 15 | Thỏa thuận tài sản vợ chồng trước khi kết hôn | Chưa đăng |

### Nhóm 4. Tranh chấp lao động (`mang: Lao động`, `nhom: lao-dong`)
Lưu ý luật sửa đổi Bộ luật Lao động, Luật BHXH hiệu lực 01/3/2027. Tình huống ví dụ không dùng công nhân may.

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 16 | Phân biệt thử việc, hợp đồng xác định và không xác định thời hạn | Đã đăng 27/11/2026 |
| 17 | Doanh nghiệp đơn phương chấm dứt hợp đồng lao động đúng luật | Đã đăng 27/11/2026 |
| 18 | Sa thải: 4 lỗi thủ tục khiến doanh nghiệp thua kiện | Chưa đăng |
| 19 | Người lao động nghỉ ngang: bồi thường, hoàn trả chi phí đào tạo | Chưa đăng |
| 20 | Tranh chấp tiền lương, nợ BHXH, trợ cấp thôi việc | Chưa đăng |

### Nhóm 5. Thay đổi đăng ký kinh doanh (`mang: Đăng ký kinh doanh`, `nhom: doanh-nghiep`)

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 21 | Thay người đại diện theo pháp luật: trách nhiệm của người cũ | Đã đăng 27/11/2026 |
| 22 | Tăng, giảm vốn điều lệ: thời hạn góp vốn, hồ sơ, chủ sở hữu hưởng lợi | Chưa đăng |
| 23 | Chuyển trụ sở sang xã, phường hoặc tỉnh khác: thủ tục thuế trước | Chưa đăng |
| 24 | Bổ sung ngành nghề kinh doanh có điều kiện | Chưa đăng |
| 25 | Chuyển nhượng vốn góp, thay đổi thành viên, cổ đông và thuế TNCN | Chưa đăng |

### Nhóm 6. Hồ sơ dự án đầu tư (`mang: Dự án đầu tư`, `nhom: doanh-nghiep`)
Bài 26A đã đăng (khách sạn 3 sao trên đất ở đô thị). Khi viết bài 26, 28, 29 tránh trùng nội dung.

| Bài | Chủ đề | Trạng thái |
|---|---|---|
| 26A | Cá nhân có đất muốn công ty xây khách sạn 3 sao (ngoài kế hoạch) | Đã đăng 27/11/2026 |
| 26 | Chấp thuận chủ trương đầu tư dự án nhà xưởng ngoài khu công nghiệp | Chưa đăng |
| 27 | Dự án thương mại: thuê đất trả tiền hằng năm hay một lần | Chưa đăng |
| 28 | Dự án dịch vụ: từ chủ trương đầu tư đến giấy phép xây dựng | Chưa đăng |
| 29 | Thẩm định PCCC, ĐTM, giấy phép môi trường trước khi khởi công | Chưa đăng |
| 30 | Điều chỉnh chủ trương đầu tư, gia hạn tiến độ dự án chậm | Chưa đăng |

## 8. Quy tắc biên tập bắt buộc cho mọi bài mới

1. Chỉ dẫn văn bản còn hiệu lực tại ngày đăng. Không đoán số điều, khoản. Văn bản đã thông qua nhưng chưa có hiệu lực chỉ nêu dạng "sắp áp dụng" kèm ngày hiệu lực.
2. Địa danh theo mô hình 2 cấp từ 01/7/2025 (tỉnh, xã, phường). Không dùng quận, huyện, thị xã. Nơi nộp hồ sơ ghi "Trung tâm Phục vụ hành chính công xã, phường".
3. Đi từ tình huống thực tế, viết đơn giản cho người dân đọc hiểu. Đoạn văn 3 đến 4 dòng.
4. Không cam kết kết quả. Cuối bài luôn khuyến nghị kiểm tra hồ sơ thực tế.
5. Không dùng gạch ngang dài, chữ in hoa để nhấn mạnh, từ sáo rỗng.
6. Không nêu mức phạt, lệ phí, thuế suất khi chưa đối chiếu văn bản gốc mới nhất.
7. Ghi `can_cu_den_ngay` đúng ngày đã kiểm tra căn cứ.

## 9. Lưu ý bảo mật

Tệp README này đã được loại trừ trong `_config.yml` nên không xuất bản lên trang web, chỉ hiện trên GitHub.
Kho này để công khai. Không đưa lên đây mật khẩu, mã truy cập, số tài khoản, hồ sơ khách hàng, tài liệu nội bộ của bất kỳ đơn vị nào.

---
Nội dung trên trang mang tính tham khảo, không thay thế ý kiến tư vấn trên hồ sơ cụ thể.
