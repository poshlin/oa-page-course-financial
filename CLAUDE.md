# oa-page-fin-platform（財商學習平台）

本專案的設計系統定義在根目錄的 `DESIGN.md`。產生或修改任何 UI 元件前，一律先讀它。

本 repo 的特殊規則（與其他 oa-page 不同，勿「好心修正」）：

1. **本頁採 Coin Quest 平台自身視覺**（保旭 2026-08-11 拍板）：主色是平台的 `#F5A623`，**不是**官網亮橘 `#FFA300`。看到 `#F5A623` 不是筆誤，禁止改回亮橘。實心鈕一律配深墨 `#2D2D2D` 字、禁白字，並寫 `border: 2px solid transparent`。
2. **留單 CTA**：`<button type="button" data-oa-cta="hero|middle|bottom|sticky">`，modal 由母站 shell 綁定提供；本 repo 本機開啟點了沒反應＝正常，不是 bug，別自己加 href 或 JS。
3. **不自帶 header/footer/nav**：注入官網時站頭站尾由官網提供。body 從 skip-link＋breadcrumb 開始。
4. **內容事實唯一來源**＝`~/Documents/oa-coin-quest/research/` 的 `deck-transcript.md` 與 `staging-inventory.md`。頁上每個數字都必須能回溯到這兩檔或品牌記憶（14 年／10 萬+ 學員）。
5. **價格與 SKU 組合（含平台使用權月數）一律不放**——定價 Albert 修正中。「45 堂」堂數結構是保旭核可可放的唯一課程數字。
6. 彩色 emoji 全站禁用（引用平台 UI 文案時把 emoji 去掉）；叩叮／波比素材禁 AI 生成，用真素材或占位區。
