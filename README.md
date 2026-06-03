# Williams Textbook of Endocrinology — Fellow 精讀筆記

針對 **Williams Textbook of Endocrinology** 各章節，由原始 PDF 經 **LlamaParse** 解析後，再重新整理為 endocrinology fellow 適用的**精讀筆記**：條列式、繁中解說 + 英文專名、附**記憶法 / 口訣 / 比較表 / 表格解讀**，重點以**粗體**與 <u>底線</u> 標示。

每個章節獨立成一個資料夾。

## ⬇️ Clone 前請先安裝 Git LFS

本 repo 的大型投影片 PDF（FellowCamp 的糖尿病 64MB、內分泌 34MB）以 **[Git LFS](https://git-lfs.github.com/)** 儲存。**未安裝 git-lfs 直接 clone，PDF 會變成幾十 bytes 的指標檔（pointer），無法開啟。**

```bash
# 1. 安裝（macOS）
brew install git-lfs        # Windows: winget install GitHub.GitLFS ; Linux: apt install git-lfs
git lfs install             # 每台電腦設定一次即可

# 2. clone（會自動下載 LFS 檔案）
git clone https://github.com/zinojeng/Williams-Textbook-of-Endocrinology.git

# 若先前已 clone 才裝 LFS，補抓實際檔案：
git lfs pull
```

> 一般 Markdown 筆記不受影響；只有 `*.pdf` 走 LFS。`.gitattributes` 已設定，之後新增的 PDF 會自動納入 LFS。

## 🏕️ FellowCamp 2026（專科考試準備）

> [**FellowCamp-2026/**](FellowCamp-2026/) — 115 年度內分泌新陳代謝科專科醫師訓練課程重點整理（給 2026 輔導員與考生）。含**糖尿病／內分泌「如何準備專科考試」兩科深度重點**（逐字稿＋投影片）、準讀版策略總綱，及其餘 8 場次（臨床試驗、動態試驗、骨骼、腦垂體、甲狀腺、副甲狀腺、腎上腺、性腺）摘要。

## 章節索引

| 章 | 主題 | 連結 | 中英對照 |
|----|------|------|----------|
| Ch.42 | Endocrine Neoplasia Syndromes（MEN1–5、MEON） | [Ch42-Endocrine-Neoplasia-Syndromes/](Ch42-Endocrine-Neoplasia-Syndromes/) | [🇹🇼🇬🇧 Ch42 bilingual](Ch42-Endocrine-Neoplasia-Syndromes/_source/Ch42-bilingual-EN-ZH.md) |
| Ch.43 | Neuroendocrine Tumors and Disorders（NEN/NET/NEC） | [Ch43-Neuroendocrine-Tumors-and-Disorders/](Ch43-Neuroendocrine-Tumors-and-Disorders/) | [🇹🇼🇬🇧 Ch43 bilingual](Ch43-Neuroendocrine-Tumors-and-Disorders/_source/Ch43-bilingual-EN-ZH.md) |
| Ch.44 | The Immunoendocrinopathy Syndromes（APS-I/II、IPEX…） | [Ch44-Immunoendocrinopathy-Syndromes/](Ch44-Immunoendocrinopathy-Syndromes/) | [🇹🇼🇬🇧 Ch44 bilingual](Ch44-Immunoendocrinopathy-Syndromes/_source/Ch44-bilingual-EN-ZH.md) |

---

*內容忠於原文、數字未外推。臨床決策請以最新指引與原文為準。*
