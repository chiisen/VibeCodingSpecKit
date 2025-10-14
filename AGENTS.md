<!-- OPENSPEC:START -->
# OpenSpec Instructions

These instructions are for AI assistants working in this project.

Always open `@/openspec/AGENTS.md` when the request:
- Mentions planning or proposals (words like proposal, spec, change, plan)
- Introduces new capabilities, breaking changes, architecture shifts, or big performance/security work
- Sounds ambiguous and you need the authoritative spec before coding

Use `@/openspec/AGENTS.md` to learn:
- How to create and apply change proposals
- Spec format and conventions
- Project structure and guidelines

Keep this managed block so 'openspec update' can refresh the instructions.

<!-- OPENSPEC:END -->

## Onboarding Checklist
- 閱讀 `openspec/project.md` 了解專案目的、技術棧與作業約束。
- 進入 `openspec/AGENTS.md` Review 相關章程與三階段工作流程。
- 檢視 `docs/index.html` 既有內容，維持單頁式資訊結構與中文描述語氣。

## Collaboration Guidelines
- 遵循規格驅動原則：任何重大頁面改動需先提出變更目的與影響，必要時建立 openspec 變更檔。
- 設計風格必須對應 `STYLE.md` 指示，並在頁面標註本次選用的主題風格。
- 編輯檔案時優先使用 `apply_patch`，保留現有 BOM 與 UTF-8 編碼。
- 若需要新增圖片，放置於 `images/` 並更新引用路徑。

## Content Standards
- 內容來源以 GitHub Spec Kit 官方文件與 README 為準，避免臆測或未證實的承諾。
- 強調 Spec-Driven Development 的流程（Proposal → Implementation → Archive）與 Specify CLI 使用方式。
- 網頁與文件以繁體中文撰寫，適度保留英文專有名詞（SDD、CLI、AI Agents 等）。

## Useful References
- 官方 Repo：<https://github.com/github/spec-kit>
- 官方文件：<https://github.github.io/spec-kit/>
- 主要維護者：@localden、@jflam（僅於描述與聯絡資訊中引用）

## Review Expectations
- 提交變更前，確認排版在桌機與手機寬度下仍具可讀性。
- 驗證所有外部連結可正常開啟；若引用 CLI 指令需再三比對官方 README。
- 如有新增流程或規範，請同步更新 `openspec/project.md` 與相關說明檔，維持一致性。
