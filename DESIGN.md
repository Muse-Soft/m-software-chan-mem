# DESIGN.md — Chân Mềm — Studio chăm sóc thú cưng

Landing page visual-first cho studio chăm sóc thú cưng Chân Mềm.
Tài liệu này là quyết định DỨT KHOÁT để Dev dựng theo đúng — không dùng mô tả chung chung.
Task Linear: TEC-184 · Epic: TEC-182 · Repo: https://github.com/Muse-Soft/m-software-chan-mem

## 1. Bảng màu (mã hex + vai trò từng màu)

| Mã hex | Tên gọi | Dùng ở đâu — bắt buộc |
|---|---|---|
| `#FAF1EC` | Hồng phấn nhạt — nền chính | Nền toàn trang, nền các mục xen kẽ (hero, lưới khách quen, form) |
| `#FFFFFF` | Trắng tinh — nền thẻ | Nền thẻ dịch vụ, thẻ khách quen, thẻ bước quy trình, khung form đặt lịch |
| `#33272E` | Tím than — chữ chính | Tiêu đề mọi cấp, nội dung chính, giá dịch vụ, chữ trên nền sáng |
| `#6E5A63` | Tím xám — chữ phụ | Mô tả phụ, ghi chú, placeholder trong form, chân trang |
| `#D96C57` | Hồng san hô — nhấn chính | Nút chính (Đặt lịch, Xem dịch vụ), giá nổi bật, tiêu đề mục được nhấn, đường gạch dưới tiêu đề hero, icon bước quy trình |
| `#F3DDD6` | Hồng phấn đậm — nền phụ | Nền mục xen kẽ (dịch vụ, quy trình 4 bước), nền thẻ giá, viền nhẹ quanh ảnh |
| `#E8CFC4` | Hồng be — viền | Viền thẻ, viền nút phụ, đường phân cách giữa các mục |

Quy tắc: nền chính luôn là `#FAF1EC` hoặc trắng thẻ — không dùng nền tối cho toàn trang.
Nút chính: nền `#D96C57`, chữ trắng `#FFFFFF`, bo tròn 999px (dạng viên nang).
Nút phụ: viền 1px `#E8CFC4`, chữ `#33272E`, nền trong suốt.
Không dùng thêm màu nhấn nào khác ngoài bảng trên.

## 2. Font chữ

- Font tiêu đề: **Fraunces** (Google Fonts, weight 600 cho tiêu đề lớn, 500 cho tiêu đề mục).
  Dùng cho: tên thương hiệu "Chân Mềm", tiêu đề hero, tiêu đề mọi mục, tên dịch vụ.
- Font nội dung: **Be Vietnam Pro** (Google Fonts, weight 400 cho nội dung, 500 cho nhãn/nhấn nhẹ).
  Dùng cho: mô tả, giá, nhãn form, nút bấm, chân trang.
- Cỡ chữ: hero 48–64px (desktop) / 32–40px (mobile); tiêu đề mục 32px / 26px;
  tên dịch vụ 20px; nội dung 16px; ghi chú 14px. Chiều cao dòng nội dung 1,6.

## 3. Phong cách tham chiếu — MỘT phong cách duy nhất

**Studio thú cưng tối giản kiểu Hàn, sáng và thân thiện.**

Đặc điểm bắt buộc: không gian sáng, nhiều khoảng trắng, ảnh thú cưng chiếm diện tích lớn;
bố cục lưới đều, góc bo mềm (thẻ bo 20px, ảnh bo 24px); không họa tiết rườm rà,
không nền tối, không màu neon. Cảm giác khi nhìn vào: sạch, nhẹ, ấm — như một studio
chăm sóc thú cưng ở Seoul chụp ảnh cho khách quen.

## 4. Quy tắc hình ảnh

- Ảnh là nội dung chính: mỗi mục có ít nhất 1 ảnh lớn, không dùng ảnh minh họa nhỏ lấp chỗ trống.
- Tỉ lệ khung: hero 16:9 (desktop) / 4:5 (mobile, ảnh dọc); ảnh dịch vụ 4:3;
  ảnh khách quen 1:1 (vuông); ảnh quy trình 3:2.
- Tông ảnh: sáng pastel, ánh sáng mềm, nền sáng, màu lông thú cưng rõ và thật;
  ảnh mẫu phải đồng tông với bảng màu (hồng phấn, be, trắng) — cấm ảnh tối, ảnh gắt,
  ảnh lệch tông lạnh/xanh dương đậm.
- Ảnh mẫu: dùng ảnh mẫu chất lượng cao (Unsplash/Pexels) có khai báo là ảnh mẫu trong
  ghi chú; khi khách gửi ảnh thật thì thay đúng tỉ lệ khung trên, không đổi bố cục.

## 5. Bố cục — 6 mục theo thứ tự

1. **Hero**: ảnh lớn chó/mèo sau khi được chăm sóc, nền sáng; tiêu đề "Chân Mềm"
   + câu dẫn 1 dòng về studio chăm sóc thú cưng + nút chính "Đặt lịch ngay".
2. **Dịch vụ — 3 nhóm**: Tắm vệ sinh · Cắt tỉa tạo kiểu · Trông giữ theo ngày.
   Mỗi nhóm 1 thẻ trắng: ảnh 4:3, tên dịch vụ, mô tả 2 dòng, giá (ghi rõ là giá mẫu
   nếu chưa có giá thật).
3. **Lưới khách quen**: 6–8 ảnh vuông 1:1 của thú cưng khách quen kèm tên (tên mẫu
   nếu chưa có tên thật), nền `#FAF1EC`.
4. **Quy trình 4 bước**: Đặt lịch → Tư vấn & kiểm tra → Chăm sóc → Bàn giao & dặn dò.
   4 thẻ trắng trên nền `#F3DDD6`, icon bước màu `#D96C57`, số bước to bằng Fraunces.
5. **Form đặt lịch (chỉ giao diện)**: tên chủ nuôi, tên thú cưng, dịch vụ cần,
   ngày mong muốn + nút "Gửi yêu cầu đặt lịch". Form chưa gửi dữ liệu thật — ghi rõ
   "bản demo, form chỉ giao diện" ngay dưới nút.
6. **Liên hệ & chân trang**: địa chỉ, số điện thoại, giờ mở cửa (ghi rõ
   [CẦN BỔ SUNG] nếu chưa có thông tin thật), bản quyền Chân Mềm.

## 6. Quy tắc khác

- Khoảng trắng: lề mục trên/dưới 80px (desktop) / 48px (mobile); khoảng cách giữa
  các thẻ 24px.
- Responsive: 1 cột trên mobile, lưới 3 cột dịch vụ / 4 cột khách quen trên desktop;
  nút chính full-width trên mobile.
- Thông tin thật chưa có thì để [CẦN BỔ SUNG], tuyệt đối không tự bịa địa chỉ,
  số điện thoại, giá thật.
