# 台灣扣件產業 AI 轉型白皮書
## 邁向智造時代：從自動化到全局打通的 AI 落地指引 (文件編號：TW-FASTENER-AI-2026-V1.1)

---

![CBAM-2026-Ready](https://img.shields.io/badge/CBAM--2026-Ready-green?style=for-the-badge&logo=eco&logoColor=white)
![Version](https://img.shields.io/badge/Version-1.1--Stable-blue?style=for-the-badge&logo=github&logoColor=white)
![License](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-purple?style=for-the-badge&logo=creative-commons&logoColor=white)
![Build](https://img.shields.io/badge/CI%2FCD-Docs%20Auto--Compile-orange?style=for-the-badge&logo=github-actions&logoColor=white)

---

## 🎯 專案定位：台灣扣件與金屬加工業 AI 數據化改造實戰指引

本專案將《台灣扣件產業 AI 轉型白皮書》全面進行「代碼化（Docs as Code）」，這是一份協助台灣螺絲廠**「把老機台接上數據、降低報廢與停機，順便自動產出歐盟 CBAM 碳足跡與生產履歷」**的實戰改造總包指引。

本智庫打破傳統白皮書「發布即定格、印出即過期」的限制，透過 Git 的版本控制與社群共創（Issue/PR）機制，動態因應 2026 年正式實施之歐盟 CBAM 碳關稅法規與前沿邊緣 AI 演算法，將知識開源與實戰應用緊密結合。

---

## 💼 核心商業服務與實戰工具（B2B 智造落地）

為了將白皮書轉化為「看得懂、能交付、能收錢」的工程與商務工具，本倉庫提供以下核心服務與商務對接文件：

1. 📂 **[核心服務與商品報價結構 (SERVICES.md)](SERVICES.md)**：精算「五大核心產品服務包」，從 8-15 萬的數據健檢包，到百萬級的主力示範線改造與 AI PdM 品質預警，打造中小型廠「自籌款極小化、轉型效益極大化」的變現漏斗。
2. 📋 **[商品 A：廠區現勘診斷標準評估 SOP 表單 (sop_assessment_form.md)](sop_assessment_form.md)**：專為現場診斷設計的表單。涵蓋傳統舊機改造的電氣/接地、高頻應變規安裝空間、PLC 通訊診斷與 AQVC 就緒度判定矩陣，是走入扣件廠房的硬核工程診斷書。
3. ✉️ **[致螺絲公會蔡永裕理事長戰略提案信 (proposal_letter_tifi.md)](proposal_letter_tifi.md)**：深度綁定公會帶領會員廠「打群架、破 CBAM 綠色關稅壁壘、保衛出口訂單」之政治與商業利益的合作提案信。

---

## 🧭 白皮書快速導覽

您可以點擊下方連結，直接閱讀各單元的 Docs-as-Code 開源 Markdown 檔案：

| 單元章節 | 核心主題內容 | 關鍵技術與操作指標 |
| :--- | :--- | :--- |
| 📖 **[導言與架構](src/index.md)** | 本白皮書之使命與產官學研推動架構 | 組織變革、產學研協同起點 |
| 🌍 **[單元一：地緣政治與現況](src/unit1-geopolitics.md)** | 川普鋼鐵關稅、2026 CBAM 正式期與斷層急迫性 | 匯率震盪、師傅凋零、碳邊境調整機制 |
| ⚙️ **[單元二：AQVC 數據與選型](src/unit2-aqvc-framework.md)** | 扣件 AQVC 數據就緒度框架與三層模型選型策略 | XGBoost 白盒子、CNN/LSTM 黑盒子、遷移學習 |
| ⚡ **[單元三：舊機改造與智慧排程](src/unit3-retrofit-mas.md)** | 10kHz 壓電式舊機非破壞改造、邊緣 PdM 與 MAS 排程 | 推論延遲 <10ms、緊急煞車迴路、多代理人應變 |
| 📊 **[單元四：量化 KPI 與 ROI 精算](src/unit4-oee-roi.md)** | OEE 三因子微觀數學拆解與 5 年期 ROI 精算模型 | $OEE = A \times P \times Q$、PSI 漂移監控、3.6年回收期 |
| ♻️ **[單元五：MLOps 與範疇三聯防](src/unit5-mlops-scope3.md)** | Docker 容器化邊緣部署、AI Champion 與 Catena-X 碳排 | DPP 數位產品履歷、外包廠數據信任平台 |
| 🏛️ **[單元六：政府資源對接實務](src/unit6-subsidy-guide.md)** | 金屬中心『扣動旋件』、低碳智慧升級補助 55.3% 避坑法 | 補助款最高 500 萬、基準線公式化、SI 廠商審查 |
| 🚀 **[單元七：24個月落地藍圖](src/unit7-roadmap-kpi.md)** | 3 大行動倡議、24個月落地時程甘特圖與組織 KPI | 小步快跑 PoC、產官學研協同、台灣智造新名片 |

---

## ⚡ 核心量化指標（LaTeX 渲染數學公式）

### 1. 微觀整體設備效率（OEE）AI 調控公式
$$OEE = A \times P \times Q$$
* **時間稼動率 ($A$)**：$A = \frac{T_{\text{run}}}{T_{\text{planned}}} = \frac{T_{\text{planned}} - (T_{\text{breakdown}} + T_{\text{setup}})}{T_{\text{planned}}}$
* **生產性能率 ($P$)**：$P = \frac{C_{\text{actual}} \times T_{\text{ideal}}}{T_{\text{run}}}$
* **品質合格率 ($Q$)**：$Q = \frac{C_{\text{actual}} - C_{\text{defect}}}{C_{\text{actual}}}$

### 2. 模型概念漂移（Model Drift）監控指標
當群體穩定性指標 $PSI > 0.25$ 時，表示產線物理特徵（模具磨損、線材批次變異）已發生實質偏移，系統將自動觸發地端 MLOps 自動重訓與影子測試更新機制：
$$PSI = \sum \left( (Actual\% - Expected\%) \times \ln\left(\frac{Actual\%}{Expected\%}\right) \right)$$

---

## 📅 24個月數位智造轉型落地藍圖

以下為專為台灣中小型扣件廠設計的 24 個月落地路線圖，詳細各階段工作內容請參閱 **[單元七](src/unit7-roadmap-kpi.md)**：

```plaintext
【Phase 1: 基礎數據盤點】 M01 - M03
   ├── 進行舊機 IoT 非破壞性改造 (加裝 10kHz 壓力與成形感測器)
   └── 實現示範線 100% 機台聯網與 OPC-UA 數據連續寫入
                               ▼
【Phase 2: 核心 AI 場景PoC】 M04 - M09
   ├── 部署邊緣端預測性維護 (PdM <10ms 煞車聯動)
   └── 引入 AI-AOI 檢測，降低過殺率 80% 以上，漏檢率 < 100 ppm
                               ▼
【Phase 3: 智慧排程與補助】 M10 - M12
   ├── 導入 MAS 多代理人與強化學習自適應動態排程系統
   └── 對接金屬中心補助 (最高 500 萬元) 降低企業自籌 CapEx 壓力
                               ▼
【Phase 4: 全局 MLOps 與綠色聯防】 M13 - M24
   ├── 建置邊緣 Docker 自動重訓維運閉環 (PSI > 0.25)
   └── 聯合外包熱處理與電鍍廠，建立範疇三碳排數據安全交換信任平台
```

---

## 📊 互動式轉型 ROI 計算器

本專案在 `docs/interactive-tool/` 目錄中，內置了我們先前開發的 **「台灣扣件產業 AI 轉型 ROI & OEE 互動計算器」**。

您可以透過部署在 GitHub Pages 上的網址動態拖動滑桿，試算您工廠的 OEE 等級、CapEx/OpEx 投入、5年累計品質節省成本，以及精確的財務回收黃金交叉點（Payback Period）：
🔗 **[https://taiwan-smart-fastener-alliance.github.io/taiwan-fastener-ai-whitepaper/interactive-tool/](https://taiwan-smart-fastener-alliance.github.io/taiwan-fastener-ai-whitepaper/interactive-tool/)**

---

## 🤝 產官學研協同與貢獻指南

本專案採用 **CC BY-NC-SA 4.0** 授權，歡迎學術界、SI 系統整合商、南部扣件廠自由 Fork 與引用。

* **回報歐盟 CBAM 最新碳關稅/計價變動**：請提交 **[CBAM Issue 模板](.github/ISSUE_TEMPLATE/01_cbam_update.md)**。
* **回報舊機改造 IoT 感測器相容性**：請提交 **[Sensor Issue 模板](.github/ISSUE_TEMPLATE/02_sensor_compat.md)**。
* **增補南部工廠 AI 轉型成功實證數據**：請依據 **[CONTRIBUTING.md](CONTRIBUTING.md)** 的數據去敏感化規範提交 Pull Request。

---

> 💡 **專案指導單位**：經濟部產業發展署、金屬工業研究發展中心 (MIRDC)
> 💡 **主辦與技術維護**：快哉問網路行銷 & 鳳凰 AI 實驗室
