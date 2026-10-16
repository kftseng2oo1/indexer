# 🪔 智慧庫建檔工具 · RAG Wisdom Indexer

把佛經典籍切段後寫入 Twinklehub Worker 的向量資料庫，供佛法 AI 導師做 RAG 檢索。

**線上使用**：https://kftseng2oo1.github.io/indexer/

## 主要功能
- **⚙ 連線設定**：輸入管理員 Token（記在本機），檢查連線並查看典籍庫統計
- **📖 單筆建檔**：輸入典籍、章節、原文、白話、關鍵詞後寫入
- **📚 內建典籍語料**：例如《金剛經》各品，點擊載入後批次建檔（目前 118 冊、114 筆）
- **🗂 批次建檔**：貼上 JSON Array，先預覽解析再上傳
- **🗑 刪除段落**：依 ID 刪除
- 📋 操作紀錄與進度條

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- 後端：`twinklehub.kftseng2oo1.workers.dev`（Cloudflare Vectorize）
- 本機資料：`wisdom_admin_token`

## 相關 repo
- [buddha](https://github.com/kftseng2oo1/buddha)：阿拉燈佛法心靈導師（使用這個知識庫）
- [dama](https://github.com/kftseng2oo1/dama)：法身實相實修
