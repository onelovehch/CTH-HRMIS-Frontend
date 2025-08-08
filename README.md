# CTH-HRMIS Frontend (CTH-2025-frontend)

> **Vue 3 + Vite SPA** for the CTH Human-Resource Management Information System backend API.
>
> 已完成 **登入頁、使用者清單/新增、部門管理、組織管理** 4 個主要畫面。

---

## ✨ 特色

| 模組        | 技術                                              | 備註                                             |
| --------- | ----------------------------------------------- | ---------------------------------------------- |
| **登入**    | Composition API + Pinia + `jwt-decode`          | Token 失效自動 Refresh；Vue Router Navigation Guard |
| **使用者管理** | Element-Plus 表格 + 分頁<br>動態表單驗證 (`vee-validate`) | 支援新增 / 編輯 / 刪除                                 |
| **部門管理**  | Cascader 選單顯示層級結構                               | API `/api/departments`                         |
| **組織管理**  | Tree Table 排列、匯入 / 匯出 JSON                      | 預留組織圖按鈕；呼叫 Backend 產生 SVG                      |
| **全域樣式**  | Tailwind CSS + Dark Mode 切換                     | Vite plugin `@vueuse/head` 動態網頁標題              |

---

## 🏗️ 專案結構

```text
cth-hrmis-frontend/
├── public/              # 靜態檔、favicon
├── src/
│   ├── api/             # Axios 實例 & API functions
│   ├── assets/
│   ├── components/
│   ├── layouts/         # MainLayout, AuthLayout
│   ├── router/
│   ├── stores/          # Pinia modules
│   ├── views/           # Login.vue, Users.vue, Departments.vue, Orgs.vue
│   └── utils/
├── .env.example         # VITE_API_BASE, VITE_APP_TITLE
├── vite.config.ts
└── README.md            # 本檔
```

---
## 🔗 前端 Repo

後端專案請見 👉 [https://github.com/onelovehch/CTH‑HRMIS-Backend]

---
## 📝 License

Released under the MIT License © 2025 onelovehch