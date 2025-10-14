# VibeCodingSpecKit

![logo_small](./images/logo_small.png)

Vibe Coding Spec Kit => Spec Kit（或稱 GitHub Spec-Kit）是一個由 GitHub 推出的**規格驅動開發 (Specification-Driven Development, SDD)** 開源框架，它旨在結構化並統一多款 AI 程式設計工具（如 Claude Code、GitHub Copilot、Gemini CLI 等）的開發流程。

Spec Kit 的核心目標是解決傳統上使用 AI 寫程式時「丟一句話給 AI 然後祈禱」的低效與不確定性，轉而透過**結構化的三階段指令**，讓 AI 能夠遵循統一的規格文件進行協作開發，從而提升程式碼的品質、一致性與可維護性。

Spec Kit 的核心元素與流程主要包含以下幾個部分：

1.  **憲法系統 (Constitution)**：
    * 這是專案的核心約束框架，用於**規範 AI 的行為**，防止其偏離專案標準。
    * 它強制定義了**技術選擇、開發流程、品質標準、測試要求**等，確保所有功能都遵循相同的原則。

2.  **核心三階段指令 (Core Commands)**：
    * **`/specify` (規格)**：
        * 提供高層次的提示，用於定義**產品需求文件 (PRD)** 中的功能規格。
        * 專注於回答 **「是什麼 (What)」** 和 **「為什麼 (Why)」**，描述專案目標、核心問題、主要功能、成功標準等，但**不關注具體的技術細節**。
    * **`/plan` (計畫)**：
        * 基於功能規格，說明**「如何 (How)」** 實際建構專案。
        * 涉及技術棧、資料庫選擇、系統架構、性能問題等。
    * **`/tasks` (任務)**：
        * 將整個計畫分解為具體的、可執行的、有明確驗收標準的**任務清單**。
        * 通常會將任務控制在 2-4 小時的完成時間，標記任務間的依賴關係，並標註可並行執行的任務，甚至可導向 **TDD/BDD (測試驅動/行為驅動開發)** 的測試案例。

**總結來說：**

Spec Kit 不僅僅是一個工具，它更是一種**標準化的開發思維模式**，透過明確定義規格、計畫和任務，讓開發者能夠有效駕馭多個 AI 助手，確保 AI 產出的程式碼能夠準確對齊軟體專案的架構和品質要求，實現真正的**規格驅動開發 (SDD)**。

* *備註：根據您的開發背景（C++、C#、Javascript、Python、Flask、React），Spec Kit 這種規格驅動的開發方式，特別有助於您在多語言、多技術棧專案中，保持 AI 協作產出的一致性與品質。*

# PROMPT
```bash
依據 https://github.com/github/spec-kit 的內容的彙整製作一頁式的介紹說明網頁，並幫我填寫 project.md 與 AGENTS.md 的內容，網頁風格請參考 STYLE.md。
```
# 執行
- 建立 docs/index.html:1 一頁式介紹，採「未來科技風」排版，整合 SDD 核心概念、Specify CLI 入門流程、三階段開發流程與 AI 協作資訊，並加入行動呼籲與官方資源連結。       
- 充實 openspec/project.md:1，說明專案目的、技術棧、樣式與協作規範，以及與 Spec Kit 相關的領域背景與外部依賴。
- 擴充 AGENTS.md:6，提供上線前檢查、協作與內容標準，確保未來 AI 協作者遵循 openspec 管理區塊與風格指示。

# 參考
https://github.com/github/spec-kit

## 風格
參考檔案: [STYLE](./STYLE.md)


