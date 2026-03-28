# LogiSync - Hệ thống hỗ trợ hoạt động Logistics

---

## Giới thiệu

LogiSync là nền tảng quản lý logistics toàn diện dành cho Supplier, Buyer và Carrier, hỗ trợ toàn bộ quy trình từ đặt hàng, vận chuyển, theo dõi GPS đến thanh toán và đối soát.

---

## Tính năng chính

- Quản lý Workspace đa vai trò (Supplier / Buyer / Carrier)
- Quản lý sản phẩm & catalog
- Quản lý đơn hàng & thương lượng nhiều vòng
- Điều phối vận chuyển & theo dõi GPS real-time
- ETA & tracking lộ trình
- e-POD (chứng từ giao hàng điện tử)
- Quản lý công nợ, hóa đơn & thanh toán
- Dashboard & báo cáo doanh thu
- Thông báo real-time (Email + Push)
- Audit log & bảo mật dữ liệu

---

## Cài đặt nhanh

### 1. Chuẩn bị môi trường

```bash
pnpm install
pnpm prepare
```

---

### 2. Chạy hạ tầng (Database / Redis / MinIO)

```bash
docker compose up -d
```

Chạy ở chế độ nền (background)

---

### 3. Chạy ứng dụng (Development)

```bash
pnpm dev           # Chạy toàn bộ hệ thống (nặng)
pnpm dev:api       # Backend (NestJS)
pnpm dev:web       # Frontend (Next.js)
pnpm dev:mobile    # Mobile (React Native)
```

---

## Quy trình Commit

Dự án sử dụng **Conventional Commits**.

❌ Không dùng:

```bash
git commit -m "..."
```

✅ Quy trình đúng:

```bash
git add .
pnpm commit
git push
```

Sử dụng giao diện chọn loại commit: `feat`, `fix`, `chore`,...

---

## Code Quality

### Lint

```bash
pnpm lint
```

### Format

```bash
pnpm format
```

Sử dụng **Biome** để kiểm tra và format code

---

## Docker Commands

### Start

```bash
docker compose up -d
```

### Stop

```bash
docker compose down
```
