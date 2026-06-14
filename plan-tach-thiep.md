# Kế hoạch tách thiệp cưới - 2 Option: Nhà Trai & Nhà Gái

## Cấu trúc thư mục

```
tuan-ngoc-08082026/
├── index.html              # GIỮ NGUYÊN - không sửa
├── nha-trai/
│   └── index.html          # Thiệp nhà trai: Trần Tuân - Khánh Ngọc
├── nha-gai/
│   └── index.html          # Thiệp nhà gái: Khánh Ngọc - Trần Tuân
├── assets/                 # Dùng chung
├── audio/                  # Dùng chung
├── elements/               # Dùng chung
├── uploads/                # Dùng chung
└── plan-tach-thiep.md      # File này
```

## So sánh 2 thiệp

| Thành phần | index.html (gốc) | nha-trai/index.html | nha-gai/index.html |
|---|---|---|---|
| **Thứ tự tên** | Trần Tuân & Khánh Ngọc | Trần Tuân & Khánh Ngọc | Khánh Ngọc & Trần Tuân |
| **Title** | Thiệp cưới - Trần Tuân & Khánh Ngọc | Thiệp cưới - Trần Tuân & Khánh Ngọc | Thiệp cưới - Khánh Ngọc & Trần Tuân |
| **Hero text** | Tuân (trái) - Ngọc (phải) | Tuân (trái) - Ngọc (phải) | Ngọc (trái) - Tuân (phải) |
| **Opening cover** | Trần Tuân & Khánh Ngọc | Trần Tuân & Khánh Ngọc | Khánh Ngọc & Trần Tuân |
| **Cha (Nhà Trai)** | Trần Văn Linh | Trần Văn Linh | Trần Văn Linh |
| **Mẹ (Nhà Trai)** | Vũ Thị Trang | Vũ Thị Trang | Vũ Thị Trang |
| **Cha (Nhà Gái)** | Nguyễn Đình Xuân | Nguyễn Đình Xuân | Nguyễn Đình Xuân |
| **Mẹ (Nhà Gái)** | Nguyễn Thị Anh Tuyết | Nguyễn Thị Anh Tuyết | Nguyễn Thị Anh Tuyết |
| **Timeline** | 8:30 Dẫn khách → 9:00 Lễ Hôn Phối → 10:00 Chụp photobooth → 11:00 Khai tiệc | Giống hệt (tạm thời) | Giống hệt (vốn là timeline nhà gái) |
| **RSVP slug** | tran-tuan-khanh-ngoc-08-08-2026 | tran-tuan-khanh-ngoc-nha-trai | tran-tuan-khanh-ngoc-nha-gai |
| **Assets** | - | Dùng chung từ thư mục gốc | Dùng chung từ thư mục gốc |

## Các thay đổi cụ thể trong mỗi file

### Cả 2 file
- Các đường dẫn assets như `uploads/...`, `elements/...`, `assets/...`, `audio/...` giữ nguyên (dùng chung)

### nha-trai/index.html
1. **Title**: `Thiệp cưới - Trần Tuân & Khánh Ngọc` (giống gốc)
2. **Hero text**: Giữ nguyên "Tuân" bên trái, "Ngọc" bên phải
3. **Opening names**: Giữ nguyên "Trần Tuân" & "Khánh Ngọc"
4. **RSVP slug**: đổi thành `tran-tuan-khanh-ngoc-nha-trai`
5. **localStorage key**: đổi tương ứng
6. **Canonical URL**: đổi thành `nha-trai/tran-tuan-khanh-ngoc`

### nha-gai/index.html
1. **Title**: `Thiệp cưới - Khánh Ngọc & Trần Tuân`
2. **Hero text**: Đảo - "Ngọc" bên trái, "Tuân" bên phải
   - Đổi text node `element_text_pzmveooy408` từ "Tuân" → "Ngọc"
   - Đổi text node `element_text_ri19iyk1q2f` từ "Ngọc" → "Tuân"
3. **Opening names**: Đảo - "Khánh Ngọc" trước, "Trần Tuân" sau
4. **RSVP slug**: đổi thành `tran-tuan-khanh-ngoc-nha-gai`
5. **localStorage key**: đổi tương ứng
6. **Canonical URL**: đổi thành `nha-gai/khanh-ngoc-tran-tuan`

## Các bước thực hiện
1. Tạo thư mục `nha-trai/` và `nha-gai/`
2. Copy `index.html` vào mỗi thư mục
3. Chỉnh sửa từng file theo bảng trên
4. Mở file trong trình duyệt để kiểm tra
