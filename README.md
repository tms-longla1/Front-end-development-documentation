# 🚀 Dự Án Frontend - Checklist Phân Tích & Cài Đặt Ban Đầu

## 📌 1. Phân Tích Yêu Cầu Dự Án

### 🔍 Yêu cầu SEO?
- **Có yêu cầu SEO** (thường là các domain như E-commerce, Job Matching, v.v.):
  - Bắt buộc sử dụng các framework **SSR** như:
    - `Next.js` (React)
    - `Nuxt.js` (Vue)

- **Không yêu cầu SEO**:
  - Có thể sử dụng:
    - `Vue.js`
    - `React.js`
  - ➜ Giúp giảm tải và giảm chi phí server

---

### 🌐 Dự án có yêu cầu đa ngôn ngữ (I18n)?
- Nếu có ➜ Cài đặt thư viện I18n tương ứng (`vue-i18n`, `react-i18next`, v.v.)

---

## 🏗️ 2. Cài Đặt Code Base

### ✅ Linting & Formatting Tools (bắt buộc)
- `Prettier`
- `ESLint`
- `Commitlint`
- `Husky`

---

### 🎨 Cài đặt Class Library (tùy chọn)
- `TailwindCSS` (Khuyến khích dùng vì nhẹ và dễ custom UI)

---

### 🧩 Component Library (tùy chọn)

#### 🔹 React:
- `Shadcn/ui` ➜ Nhẹ, dễ kết hợp Tailwind
- `MUI` ➜ Ngôn ngữ thiết kế Material Design, kết hợp được với Tailwind

#### 🔸 Vue:
- `Shadcn/ui` ➜ Nhẹ, dễ kết hợp Tailwind
- `PrimeVue` ➜ Component chi tiết, kết hợp tốt với Tailwind
- `Vuetify` ➜ Dựa theo Material Design, khó kết hợp Tailwind
- `Ant Design Vue`, `Element UI` ➜ Cơ bản, khó tích hợp Tailwind

---

### 🔄 Query Library (tùy chọn)
- `TanStack Query` ➜ Quản lý data fetching hiệu quả

---

### 🧠 State Management

#### Vue:
- `Pinia` (khuyến nghị)

#### React:
- `Redux`
- `Recoil`
- `Zustand`

---

## ⚙️ 3. Triển Khai Dự Án

### 📊 Thường xuyên chạy `analyze` sau khi build:
- Kiểm tra các warning
- Tối ưu hiệu năng tải trang

---

## 🚀 4. Deploy Dự Án

- Cấu hình `NGINX`
- Dùng `Docker` để đóng gói và deploy
- Dùng `PM2` nếu dự án là **SSR Framework (Nuxt, Next)** để quản lý process

---

> ✅ Hãy đảm bảo luôn đồng bộ codebase với team và tuân theo chuẩn coding đã định!
