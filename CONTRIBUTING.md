# 台灣扣件產業 AI 轉型白皮書 - 協作與貢獻指南 (CONTRIBUTING)

> [!NOTE]
> 歡迎加入台灣首創扣件開源產業智庫！本專案旨在透過產、官、學、研的社群共創，為全台扣件聚落（特別是高雄岡山、路竹地區）建立最具權威與時效性的轉型指引。

---

## 🤝 我們歡迎哪些貢獻？

本專案採用 **Docs-as-Code** 機制進行文件維運。我們非常歡迎以下維度的貢獻：

1. **歐盟 CBAM 碳關稅政策修訂**：提報最新憑證計價、申報格式、法規豁免條款變動。
2. **舊機改造感測器相容性數據**：共享實務上各式感測器與智慧機上盒（SMB）在傳統打頭/輾牙機上的安裝與高頻濾波配置。
3. **金屬中心/產發署補助計畫避坑經驗**：分享您申請補助計畫的成功與不通過實戰案例剖析。
4. **扣件廠 AI 轉型成功案例**：增補南部扣件廠導入 OEE 最佳化、邊緣 PdM 或自適應排程的真實量化數據。

---

## 🛠️ 如何提交您的貢獻？

### 1. 通過 Issue 回報政策與技術動態
如果您發現法規變更或技術相容性問題，但不想直接修改程式碼，請點擊 Repository 的 **Issues** 選項，挑選以下模板進行提交：
* **[CBAM 碳關稅政策更新模板](.github/ISSUE_TEMPLATE/01_cbam_update.md)**
* **[感測器/機上盒相容性回報模板](.github/ISSUE_TEMPLATE/02_sensor_compat.md)**

### 2. 通過 Pull Request (PR) 增補案例或正文
如果您希望直接增補或修改正文內容，請依循以下步驟：

1. **Fork 本倉庫** 到您的個人 GitHub 帳戶下。
2. **建立功能分支 (Feature Branch)**：
   ```bash
   git checkout -b feature/your-contribution-name
   ```
3. **進行文件編輯**：
   * 編輯 `src/` 目錄下的對應 Markdown 檔案。
   * 請確保數學公式符合 LaTeX 標準，並由 `$` (行內公式) 或 `$$` (區塊公式) 進行包裝。
4. **送審前的數據合規防線 (重要)**：
   * **去敏感化**：為保護商業機密，提報之案例應使用代稱（如：*高雄岡山車用螺絲 A 廠*），隱去具體工廠名稱。
   * **數據真實性**：新增的案例數據必須依循白皮書第四單元的 **$OEE = A \times P \times Q$** 拆解公式與財務精算假設，列出轉型前後的數值對比，禁止使用「大幅改善」、「極大縮短」等非量化詞彙。
5. **提交 Commit 並 Push**：
   ```bash
   git commit -m "docs: 增補岡山A廠導入邊緣PdM後之OEE量化改善數據"
   git push origin feature/your-contribution-name
   ```
6. **發起 Pull Request (PR)**：
   * 點擊您的 Fork 倉庫首頁的 **Compare & pull request**。
   * 詳細填寫 **[PR 案例提報模板](.github/ISSUE_TEMPLATE/03_case_study.md)**。
   * 勾選同意本專案之開源授權聲明。

---

## ⚖️ 開源授權聲明 (License Agreement)

> [!IMPORTANT]
> 當您向本專案提交 Pull Request (PR) 被 Merge 後，即代表您同意將您貢獻的文字、表格與數據，以 **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** 協議進行開源授權。
> 
> 這保障了學術界、工廠與 SI 廠商的自由引用與改作權利，同時禁止任何商業營利機構直接複製轉售本白皮書。

感謝您為台灣扣件產業的雙軸轉型貢獻一份心力！
