# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 專案定位

OPC-Agent 是 Oscar（肥彭 / 彭健禧）的 LifeOS（人生管理系統），這不是一個傳統軟體專案，而是 Oscar 的個人管理中樞。

## 使用者背景

- 個人與工作：Oscar（肥彭 / 彭健禧），於澳門工作，任職於「澳門集寶有限公司 (Chubb Macau Limited)」，擔任「消防部業務系統經理」
- 技術背景：非工程師專業，所有技術解釋需用白話文和日常比喻輔助
- 溝通風格：有疑問時主動提問，不要猜測 Oscar 的需求
- 決策建議：可以質疑 Oscar 的提案，若有更好的做法直接提出，不用「護主」

## 語言與排版

- 一律使用繁體中文對話
- 語氣自然像朋友，避免生硬詞彙（如「旨在」「總的來說」）
- 中文字與英文、數字之間加上半形空格，例如：我有 3 台 iPhone 手機
- 保留專業術語的英文和縮寫，例如 Google Search Console、Notion、OpenAI
- 程式碼、變數名稱、commit message 使用英文

## 協作流程

1. 重要開發行動前先輸出簡要計劃，等 Oscar 確認後再執行
2. 執行前先確認香港時間：`date`（時區：Asia/Hong Kong, UTC+8）

## 專案結構

所有 OPC-Agent 相關檔案統一存放在 `P:\Sync\Claude\OPC-agent`。

```
OPC-agent/
├── CLAUDE.md              — 專案指引（本檔案）
├── README.md
├── .claude/
│   ├── settings.local.json — 專案層級 Claude Code 設定（含 StatusLine、權限）
│   └── skills/
│       ├── frontend-design/  — 高質感前端設計 skill
│       ├── find-skills/      — 搜尋並安裝更多 skills
│       └── skill-creator/    — 建立、修改、評測自訂 skills
```

## 已安裝的工具

- **OpenCLI** (`@jackwener/opencli` v1.7.7) — 將任何網站變成 CLI 工具，支援 500+ 網站適配器
- **StatusLine** — 自訂 terminal 底部狀態列，腳本位於 `C:\Users\Oscar Pang\.claude\statusline.js`，使用 ANSI 色塊顯示目錄、模型名稱、Context 用量 bar
