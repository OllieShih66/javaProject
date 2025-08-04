# 🛒 lutu專案＿商城

> **Java / Spring Boot / MySQL / Redis / RESTful API 開發實作**

本專案為 Java 軟體工程師轉職培訓中的團隊專題，我主要負責商城之購物車、結帳流程與訂單管理功能，整體以 Spring Boot 為核心，結合 RESTful API 設計、資料庫建模與 Redis 快取等實作，實現一個具備實務功能的後端服務。

---

## 🔧 使用技術

| 類別 | 技術 |
|------|------|
| 開發語言 | Java |
| 後端框架 | Spring Boot、Spring Web、Spring Data JPA |
| 資料庫 | MySQL、Redis |
| 前後端串接 | RESTful API、DTO、JSON |
| 工具 | Git、Postman、Eclipse IDEA |

---

## 🎯 主要功能（我負責的部分）

- **購物車系統：**
  - 加入/移除商品、修改數量、儲存使用者選項
  - 登入會員使用 Redis 快取，未登入使用 sessionStorage
  - 設計購物車合併邏輯，登入時將訪客與會員購物車合併

- **訂單管理與結帳流程：**
  - 訂單建立、金額計算、折扣驗證
  - 結帳時需登入驗證，填寫付款、出貨與收件資訊
  - 成立訂單後可進入會員後台進行取消、退貨、評論等操作

- **例外處理與資料驗證：**
  - 使用 `@Valid` 與自訂 Exception Handling 處理輸入錯誤
  - 強化資料完整性與開發除錯效率

---

## 📁 專案結構概覽

```plaintext
lutu/
├── controller/
├── service/
├── repository/
├── model/ (entity/DTO)
├── config/
└── application.properties
```

* 使用標準三層架構（Controller-Service-Repository）
* 採用 DTO 模式隔離 Entity 與外部傳輸資料
* 整合 Redis 作為購物車暫存與快取優化

---

## 🧑‍💻 我的貢獻與收穫
- 熟悉 Java Spring Boot 專案實作流程
- 完成多支 REST API 的設計與測試
- 學會處理後端邏輯、資料驗證與快取優化
- 建立清楚的程式架構與培養 Git 團隊開發習慣
