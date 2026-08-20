# 美甲膠庫存紀錄表（專案藍圖）

> 本檔為跨 Agent 通用的專案藍圖（AGENTS.md 開放標準）。任何 Agent 的每個 session 都應先讀本檔＋`handoff.md`。

## 專案簡介
此專案旨在建立一個美甲膠庫存紀錄表，幫助使用者有效追蹤與管理美甲膠的庫存狀況（例如品牌、色號、剩餘量與過期時間等）。

## 關鍵時程
- 專案啟動：2026-08-20（初始化專案與需求確認）

## 目標與路線圖
- [x] 階段一：需求分析與庫存紀錄表格式設計（Google Sheets 雲端資料庫）
- [x] 階段二：實作庫存紀錄與管理功能（CRUD、標籤選色、手機端最佳化）
- [x] 階段三：測試與優化（3個月即期提醒、終極樂觀更新、0秒刪除響應）

## 資料夾結構
```
. (專案根目錄)
├── .gitignore
├── agents.md
└── handoff.md
```

## 同步層級（本專案初始化至第 3 層級）

| 層級 | 平台 | 位置 | 讀取時機 |
|------|------|------|---------|
| L1 | 本地（GDrive） | `agents.md`＋`handoff.md` | 每個 session |
| L2 | GitHub | 專案：[wsx88634/nail-gel-inventory](https://github.com/wsx88634/nail-gel-inventory) <br> 網頁：[手機版入口](https://wsx88634.github.io/nail-gel-inventory/) | 指定時 |
| L3 | Obsidian | [美甲膠庫存紀錄表/專案工作流程.md](file:///G:/%E6%88%91%E7%9A%84%E9%9B%B2%E7%AB%AF%E7%A1%AC%E7%A2%9F/secondbrain/%E7%BE%8E%E7%94%B2%E8%86%A0%E5%BA%AB%E5%AD%98%E7%B4%80%E9%8C%84%E8%A1%A8/%E5%B0%88%E6%A1%88%E5%B7%A5%E4%BD%9C%E6%B5%81%E7%A8%8B.md) | 有需要時 |

## 工作約定
- 任何 Agent、任何電腦：**開工先讀 `handoff.md`，收工必更新 `handoff.md`**
- 修改共用檔案前先讀最新內容，避免覆蓋其他 Agent 的變更
- 所有回應與文件使用繁體中文
- 修改前先確認計畫，優先保留原有資料結構
