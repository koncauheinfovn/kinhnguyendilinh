# K'Ho GitHub data

Gói này gồm hai bộ dữ liệu:

1. `truyen_dan_gian_kho_data.*` - Truyện cổ tiếng K'Ho (Njrềng) - Vùng Phitô  
   - Biến JS: `window.TRUYEN_DAN_GIAN_KHO_DATA`  
   - 65 bài, 506 trang PDF.

2. `kinh_nguyen_kho_di_linh_data.*` - Kinh nguyện K'Ho Di Linh  
   - Biến JS: `window.KINH_NGUYEN_KHO_DI_LINH_DATA`  
   - 101 bài, 13 mục.

3. `kho_combined_data.*` - bản gộp cả hai bộ dữ liệu  
   - Biến JS: `window.KHO_COMBINED_DATA`

Mỗi bộ có đủ:

- `.js`: dùng trực tiếp qua thẻ `<script>`.
- `.min.js`: bản nén gọn để đưa lên GitHub/CDN.
- `.json`: JSON thuần để dùng `fetch`.
- `.unicode.txt`: bản chữ Unicode đã chuẩn hóa NFC để kiểm tra nhanh.

Lưu ý Unicode:

- File PDF truyện cổ có lớp chữ legacy, đã chuyển sang Unicode hiển thị trong trường `text`/`html`.
- Trường `sourceText` trong dữ liệu truyện cổ giữ nguyên lớp chữ gốc của PDF để đối chiếu.
- File DOCX Kinh nguyện đã là Unicode nên chỉ chuẩn hóa NFC, không chuyển mã legacy.
