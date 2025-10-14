# Project Context

## Purpose
- 建立一頁式中文介紹頁，快速傳達 GitHub Spec Kit 與 Spec-Driven Development（SDD）的核心價值。
- 維護專案內文檔（`project.md`, `AGENTS.md` 等），確保後續 AI 或協作者能依流程作業。
- 蒐集並彙整官方資源，提供入門步驟、核心哲學與協作指南。

## Tech Stack
- 靜態網頁：HTML5、原生 CSS（可在單一檔案內使用 `<style>`）。
- 字體：Google Fonts（Orbitron、Inter）以及系統中文字體。
- 工具：可搭配 `openspec` 指令與 Specify CLI，但網站本身無需後端。

## Project Conventions

### Code Style
- 使用語意化 HTML 標籤（`section`, `article`, `nav`, `main` 等）並以 BCP-47 `zh-Hant` 指定語系。
- CSS 採變數管理色彩與間距；避免引入未使用的樣式或框架。
- 優先支援桌機與手機（RWD），確保可讀性與對比度。
- 僅在內容需要時加入少量註解，避免冗長說明。

### Architecture Patterns
- 單頁式結構：Hero、SDD 介紹、快速入門、核心哲學、開發階段、AI 協作者、資源區塊。
- 圖像與靜態資源放在 `images/`；其他文件維持在根目錄或 `openspec/` 相對應位置。
- 若未來新增多頁，維持 `docs/` 為 GitHub Pages 根目錄。

### Testing Strategy
- 以人工檢視為主：確認排版、超連結、字型載入與深色背景可讀性。
- 若整合自動化檢查，優先考慮 Lighthouse 或簡易 HTML 驗證器，但目前非必須。

### Git Workflow
- 建議採用功能分支：`feat/xxx`、`docs/xxx`；完成後合併至 `main`。
- Commit 訊息採動詞開頭的英文或中文（例如 `chore: update project docs`）。
- 避免重置或覆蓋使用者既有修改。

## Domain Context
- GitHub Spec Kit 支援以規格為中心的開發流程，核心指令包含 `/specify`、`/plan`、`/tasks`。
- Development 分為 Proposal、Implementation、Archiving 三階段，需搭配 `openspec` 驗證。
- 主要讀者為熟悉 AI 協作與產品開發的工程師或 PM，需要快速理解 SDD 優勢與落地步驟。

## Important Constraints
- 依照 `STYLE.md` 規範，建立時需隨機選擇（或事先指定）其中一種風格並貫徹設計描述。
- 內容需保持精準引用 Spec Kit 官方資訊，避免傳遞未驗證的功能或流程。
- 保留 `AGENTS.md` 中 `<!-- OPENSPEC:START -->` 管理區塊，禁止移除或更動標記。

## External Dependencies
- Google Fonts（Orbitron、Inter）供未來科技風排版使用。
- GitHub Spec Kit 官方連結：`https://github.com/github/spec-kit`、`https://github.github.io/spec-kit/`。
- 若引用影片或其他媒體，需確保來源可公開存取。
