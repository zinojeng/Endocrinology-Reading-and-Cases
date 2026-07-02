# MEN1 分子遺傳學與監測（Molecular Genetics & Surveillance）

> 來源：Williams Textbook of Endocrinology, Ch.42 — MEN1 Genetics and Surveillance

---

## 1. 🧬 MEN1 基因與 menin 蛋白基礎

- **基因位置**：chromosome <u>11q13</u>
- **結構**：含 <u>10 exons</u>，跨越 <u>7.7 kb</u> genomic DNA
- **蛋白產物**：menin，<u>610 個 amino acid</u>（main transcript = <u>2.76-kb mRNA</u>）
- **menin 功能總綱**：調控 transcription、chromatin structure、genome stability、cellular proliferation；透過與 interacting protein partners 直接結合或調節關鍵 signaling pathway 來作用
- **轉錄體多樣性**：已辨識至少 <u>18 種</u> MEN1 transcripts，其中 15 種預測可轉譯成 146–652 amino acid 的蛋白
- **表現**：MEN1 transcript 在所有檢測過的人類組織皆表現，但 menin 蛋白量不一定與 transcript 量相關
- **演化保守性**：
  - 與 mouse / rat 的 DNA identity ~<u>89%</u>、protein identity ~<u>97%</u>
  - Orthologue 見於 zebrafish、Drosophila；但 **不存在於** yeast（S. cerevisiae）與 nematode（C. elegans）
  - 族群層級研究顯示 coding region 對 missense / nonsense variation 有高度 constraint（強烈演化選擇壓力）

> 📌 **重點 (High-Yield)**：
> - MEN1 = <u>11q13</u>、<u>10 exons</u>、menin = <u>610 aa</u>。
> - menin 是 scaffold（鷹架）蛋白，主要在 nucleus，是內分泌組織的 **tumor suppressor**。

---

## 2. 🧬 Two-Hit (Knudson) 機制 — 圖解式條列

MEN1 是典型遵循 Knudson **"two-hit"** model 的遺傳性腫瘤症候群：腫瘤需要 MEN1 基因 **biallelic inactivation（兩個 allele 都失活）** 才會形成。

```
   [生殖細胞層級]                       [體細胞層級 / 腫瘤組織]
   ┌─────────────────┐                 ┌──────────────────────────┐
   │  FIRST HIT      │                 │  SECOND HIT              │
   │  (germline)     │   ───────►      │  (somatic)               │
   │                 │                 │                          │
   │  遺傳一個        │                 │  野生型 (wild-type)       │
   │  heterozygous   │                 │  MEN1 allele 失活         │
   │  pathogenic     │                 │                          │
   │  MEN1 variant   │                 │  → 腫瘤形成               │
   └─────────────────┘                 └──────────────────────────┘
         每個細胞都帶                          只發生在腫瘤細胞
```

- **First hit（第一擊）**：病人 **生殖細胞層級** 帶有一個 heterozygous pathogenic MEN1 variant（即所有細胞都有，~10% 為 de novo 突變）。
- **Second hit（第二擊）**：腫瘤組織中 **野生型 allele 的體細胞失活**，常見機制：
  - **最常見**：11q13 locus 的大片段 somatic deletion → 在腫瘤 DNA 上表現為 **LOH（loss of heterozygosity）**
  - **替代機制**：point mutation（nonsense / missense）或 small indels → 此時 **LOH 不會出現（not apparent）**
- **結論**：腫瘤展現 MEN1 的 **biallelic inactivation**，與 Knudson two-hit model 一致，支持 menin 在內分泌組織具 **tumor-suppressor** 功能。

### ⚠️ 易混淆：LOH 一定會出現嗎？

| Second hit 機制 | 是否出現 LOH |
|---|---|
| 大片段 deletion（最常見） | ✅ 會（LOH apparent） |
| Point mutation / small indel | ❌ 不會（LOH not apparent） |

> 📌 **重點 (High-Yield)**：
> - MEN1 = **germline first hit + somatic second hit**，腫瘤呈 **biallelic inactivation**。
> - 第二擊最常見是大片段 deletion（→ LOH）；若是 point mutation/indel 則 **看不到 LOH**。

---

## 3. 🧬 Germline MEN1 Mutations（生殖細胞突變）

- 迄今已報告 **>1200 種** germline MEN1 pathogenic variants，其中約 **~600 種** 為不同的 germline mutation
- **遺傳方式**：最常來自受影響的父母（autosomal dominant）；**~10%** 為 de novo
- **突變型態分布**：
  - **~70%** 預測導致 LOF（透過 menin 蛋白 premature truncation）：
    - frameshift del/ins：<u>40%–45%</u>
    - nonsense：<u>14%–20%</u>
    - splice-site：<u>~10%</u>
  - missense：<u>20%–25%</u>
  - in-frame del/ins：<u>~5%</u>
  - gross deletion（部分或全部 MEN1）：<u>1%–2.5%</u>
- **分布**：突變遍及整個 coding region，但有 **熱點 codons**（被 ≥5 種不同突變影響）：
  - <u>45, 69, 70, 139, 156, 183, 220, 253, 418, 436, 516</u>
- **熱點成因假說**：
  1. 部分突變位於 **repetitive DNA sequence** → 符合 **replication-slippage** 致突變模型
  2. 族群特異性 **founder mutation**（可由 haplotype analysis 確認）

### 🩺 Genotype–Phenotype 相關性

- **基本結論：缺乏明顯的 genotype-phenotype correlation**
  - 同一大家族、同一突變，成員可發展出 **不同範圍的腫瘤**
- 已報告（但需進一步驗證）的例外：影響 menin 與 **CHES1（checkpoint kinase 1）** 及 **JUND transcription factor** 交互作用區域的突變，與特定不良預後相關

### 🔬 特殊表型變異（Phenotypic variants）

| 變異型 | 突變 | 表型特徵 |
|---|---|---|
| **Burin / prolactinoma variant** | nonsense：<u>Tyr312Ter</u>、<u>Arg460Ter</u> | prolactinoma 高發、gastrinoma 低發 |
| **Tasmania 家族** | splice-site：<u>c.446-3C>G</u> | **不出現** somatotropinoma |
| **FIHP**（familial isolated hyperparathyroidism） | 部分為 missense（也有 truncating） | 只發展 parathyroid tumor |

- **FIHP vs MEN1**：FIHP 的 **missense 突變比例較高**（~<u>38%</u> vs <u>23%</u>，*p* <0.01）；部分 FIHP missense 仍保留 menin 蛋白穩定性與生物活性 → 對應較輕表型。但有些 FIHP 帶與 MEN1 相同的 truncating 突變 → 暗示有 **genetic modifiers**
- 其他現象：thymic NET、pituitary、adrenal tumor 可在某些家族 **clustering**（潛在 genetic modifier）；近期有報告提及 **genetic anticipation** 可能性（但子代較早發現可能源於 ascertainment bias）

### ⚠️ 找不到 MEN1 突變的情況

- **~5%–25%** 臨床診斷 MEN1 者在 coding region 找不到突變，可能原因：
  - 突變位於 **promoter 或 untranslated region**
  - 為 **phenocopy**（其他基因突變）
  - 為 **mosaic MEN1 mutation**：先前檢測可能漏掉，臨床表現與 germline 突變者無顯著差異 → 可能需要 **affected tissue 分析** 或 **high-depth NGS**
- 這群 coding-region 陰性者相較有突變者：首個內分泌腫瘤 **發病較晚**、極少發展第三個 MEN1 manifestation、壽命較長 → 許多可能只是 **兩個巧合的散發性內分泌腫瘤**，而非真正遺傳性 MEN1

### ⚠️ 背景族群變異（解讀陷阱）

- GnomAD 資料：2 個 common missense variant（MAF >0.5%；<u>p.Arg176Gln</u>、<u>p.Ala546Thr</u>）與 >200 個 rare missense variant → **絕大多數無臨床意義**

> 📌 **重點 (High-Yield)**：
> - **~70%** germline 突變為 truncating LOF；**~10%** de novo；**genotype-phenotype 無相關**。
> - 記住兩個 phenocopy/variant 數字：**~5%–25%** 臨床 MEN1 無 coding 突變；phenocopy 佔 **~5%–10%** kindreds。
> - 別把 GnomAD 的 common missense（R176Q、A546T）誤判為致病。

---

## 4. 🧬 MEN1 Phenocopies 與其他基因突變

- **Phenocopy 定義/情境**（佔 ~<u>5%–10%</u> MEN1 kindreds）：
  1. 家族性 MEN1 中，出現 MEN1 相關腫瘤（如 pituitary / parathyroid）但 **不帶家族 MEN1 突變** 的個案
  2. 臨床上像 MEN1（≥2 個 MEN1 相關內分泌腫瘤）卻 **無 MEN1 突變**，而是帶其他基因突變

| 基因 | 編碼/功能 | 相關疾病 |
|---|---|---|
| **CDC73** | — | HPT-JT syndrome |
| **CASR** | CaSR | FHH1（familial benign hypocalciuric hypercalcemia type 1）/ FIHP |
| **AIP** | aryl hydrocarbon receptor interacting protein | FIPA（familial isolated pituitary adenoma） |
| **CDKN1B** | — | **MEN4** |
| **MAX** | — | 推測的 **MEN5** 表型（近期報告） |

- **臨床原則**：典型或非典型 MEN1 表現但找不到 MEN1 突變者，應考慮 **phenocopy 或替代基因診斷**；只要家族有已知 MEN1 突變，**所有家族成員不論臨床狀態都應接受基因檢測**

> 📌 **重點 (High-Yield)**：
> - Phenocopy 候選基因記憶法 → **「73-CASR-AIP-CDKN1B(MEN4)-MAX(MEN5)」**。
> - CDC73→HPT-JT、CASR→FHH1、AIP→FIPA、CDKN1B→MEN4、MAX→MEN5。

---

## 5. 🧬 Somatic MEN1 Mutations（散發腫瘤中的體細胞突變）

Somatic inactivating MEN1 突變廣泛見於對應的 **散發性** MEN1 相關腫瘤 → MEN1 是 inherited 與 non-inherited 腫瘤的關鍵 driver。

| 腫瘤類型 | Somatic LOF MEN1 突變頻率 |
|---|---|
| Parathyroid tumor | ~<u>35%</u> |
| NF pancreatic NET | <u>40%–45%</u> |
| Gastrinoma | ~<u>40%</u> |
| Insulinoma | <u>0%–15%</u> |
| Pituitary tumor | <u>3%–5%</u> |
| Pulmonary carcinoid | ~<u>15%–20%</u> |
| Small intestinal NET | <u><3%</u> |
| Adrenocortical tumor | <u><3%</u> |
| Angiofibroma | <u>10%</u> |
| Lipoma | ~<u>30%</u> |
| 非 MEN1 腫瘤：uterine leiomyosarcoma | <u>6%</u> |

📊 **表格解讀**：

- **臨床效用目前有限**，但未來 tumor genotyping 或許可協助 **個人化治療**。
- **預後資訊**：散發 **pancreatic NET** 帶 somatic MEN1 突變者，存活率優於無突變者。
- 易混淆：**insulinoma（0%–15%）與 pituitary（3%–5%）的 somatic MEN1 突變率最低**；NF pancreatic NET（40%–45%）最高。

> 📌 **重點 (High-Yield)**：
> - 散發腫瘤中 somatic MEN1 突變：**NF-pNET 最高（40–45%）**，**insulinoma / pituitary 最低**。
> - 散發 pNET 有 somatic MEN1 突變 → **預後較佳**。

---

## 6. 🔬 Menin 蛋白功能與 tumorigenesis 機制

- **定位**：普遍表現，主要在 **nucleus**（C-terminus 有至少 3 個 nuclear localization signals）；也見於 cytoplasm（調控 signaling pathway）
- **角色**：**scaffold protein**，與 >20 種蛋白/分子交互作用，參與：transcriptional & epigenetic regulation、genome stability、DNA repair、cell division、cell signaling、cell motility
- **⚠️ 矛盾雙面性（context- & cell-type-specific）**：
  - 對 transcription 可同時為 **activator 與 repressor**
  - 在 MEN1 相關腫瘤是 **tumor suppressor**；但在 leukemia、pediatric glioma、prostate / hepatocellular / breast cancer 是 **oncogenic cofactor / oncogene**
- **研究限制**：缺乏生理相關的 endocrine cell line / ex vivo model

### 🐭 Men1 小鼠模型重點

| 模型 | 表現 |
|---|---|
| **Men1⁺ᐟ⁻（heterozygous）** | 重現 MEN1 主要特徵：pancreatic islet、anterior pituitary、parathyroid、adrenal gland 多發腫瘤；腫瘤呈 **time-dependent**，約 **~9 個月** 開始；腫瘤確認 **LOH + menin 表現喪失**（biallelic inactivation） |
| **Men1⁻ᐟ⁻（homozygous）** | **胚胎致死**（embryonic day <u>E10.5–14.5</u>）：craniofacial defects、hemorrhage、edema、neural tube defects、early pancreatic endocrine development 異常；時間/表型依小鼠 background strain 而異（genetic modifier） |
| **Conditional / 組織特異性** | parathyroid、pancreatic（α-cell、β-cell）特異模型；tamoxifen-inducible β-cell knockout（Rip-Cre + ER-Cre）→ 急性 Men1 失活後 **快速 islet cell proliferation**，可研究 tumorigenesis 早期事件與新療法 |

- **Preclinical 應用治療方向**：gene therapy、new SSAs、epigenetic modulators、β-catenin antagonists、MEK1/2 inhibitors

> 📌 **重點 (High-Yield)**：
> - menin = nuclear scaffold；在 MEN1 是 **tumor suppressor**，在 leukemia 等是 **oncogene**（雙面性）。
> - Men1⁺ᐟ⁻ 小鼠約 **9 個月** 起多發內分泌腫瘤；Men1⁻ᐟ⁻ **E10.5–14.5 胚胎致死**。

---

## 7. 🩺 Genetic Testing（基因檢測適應症）

### MEN1 突變分析的三大臨床用途

1. **確認臨床診斷**
2. 找出 **帶突變的家族成員** → 需腫瘤篩檢與早期治療
3. 找出 **不帶家族 germline 突變的家族成員** → 可給予安心保證（reassure）

### 📋 現行指引建議檢測 MEN1 的對象

1. **Index case**：有 **≥2 個** MEN1 相關腫瘤（parathyroid、pancreatic islet、pituitary）
2. **所有 first-degree relatives**：已知 MEN1 突變帶原者的一等親，**不論有無症狀**
3. **疑似或非典型表現者**：
   - parathyroid adenoma <u><30 歲</u> 且/或 multigland parathyroid disease
   - **任何年齡** 出現的 gastrinoma 或 multiple pancreatic NET
   - ≥2 個 MEN1 相關腫瘤但 **不限於** 經典三聯（如 parathyroid + adrenal tumor）

### 📊 各 cohort MEN1 突變偵測率（支持上述建議）

| 臨床情境 | MEN1 突變偵測率 |
|---|---|
| ≥2 主要內分泌腫瘤 + 家族史 | <u>>70%</u> |
| ≥1 主要腫瘤 + 一等親有主要腫瘤 | ~<u>60%</u> |
| 散發 MEN1 相關內分泌腫瘤轉介者 | <u>6%</u>（且僅見於多發腫瘤或 <30 歲者） |
| Index 有 **3 個** MEN1 相關腫瘤 | <u>80%</u> |
| 同上 + 家族史有受影響親屬 | <u>>90%</u> |
| 單一 MEN1 相關腫瘤 | <u>15%</u> |
| 單一腫瘤 + **無** 家族史 | <u>0%</u> |

- **PHPT + PHPT 家族史（n=205）研究**：~<u>45%</u> 有 MEN1 突變；獨立預測因子與 odds ratio：
  - **multigland disease → OR ~14**
  - **male sex → OR ~1.5**
  - **age <45 → OR ~8**

📊 **表格解讀**：腫瘤越多、越年輕、越有家族史 → 突變偵測率越高（>90%）；反之單一腫瘤 + 無家族史 → 0%。**不做基因檢測 = 錯失早期診斷機會。**

### 🩺 檢測流程與倫理

- **Cascade / predictive testing**：診斷後應對所有 first-degree relatives 提供 predictive testing，**愈早愈好**（延遲會增加 morbidity）
- **兒童檢測**：因早發 MEN1 相關腫瘤 penetrance 高，建議 at-risk 無症狀兒童於 **生命第一個十年（first decade）** 提供檢測（多以父母同意進行）
- **生育相關**：提供 preconception counseling；IVF + **PGD（preimplantation genetic diagnosis）** 可供帶原者選擇
- **倫理考量**：家族影響、生育決策、財務/社會歧視 → 需 pretest counseling 與透明溝通

### 🔬 檢測技術標準

- 在 **accredited** 實驗室，sequence 所有 exonic + splice-site region → 偵測 SNV / small indel
- 直接定序陰性 → 加做 **whole/partial gene deletion** 偵測（如 **MLPA** 或其他 copy number 分析）
- 變異判讀依 **ACMG guidelines**（已有 MEN1-specific 調整版）；rare missense 可用 in silico 方法輔助分類

> 📌 **重點 (High-Yield)**：
> - 檢測三大適應症：**index ≥2 腫瘤 / 所有一等親 / 非典型（PHPT <30、任何年齡 gastrinoma 或 multiple pNET）**。
> - PHPT 家族史的突變獨立預測因子記憶：**multigland (OR~14) > age<45 (OR~8) > male (OR~1.5)**。
> - 兒童於 **first decade** 檢測；定序陰性務必加 **MLPA** 排除 gross deletion。

---

## 8. 🩺 Tumor Surveillance（監測時程表，Table 42.2）

> 原則：所有高風險者（突變帶原者）應定期 **clinical + biochemical + radiologic** 篩檢，以早期偵測與治療、降低 morbidity/mortality。雖屬合理，**高品質實證尚未確立**，多數臨床醫師仍建議 interval surveillance（頻率與範圍仍有爭議）。

### Table 42.2 — Suggested Screening Guidelines for Individuals at Risk of MEN1

| MEN1 相關腫瘤 | 起始篩檢年齡（歲） | 生化篩檢（每年） | 影像篩檢（間隔） |
|---|---|---|---|
| **Parathyroid** | <u>8</u> | Calcium, PTH | None |
| **Pancreatic — Gastrinoma** | <u>20</u> | Fasting gastrin | None |
| **Pancreatic — Insulinoma** | <u>5</u> | Fasting glucose (± insulin) | None |
| **Pancreatic — Other PNET**（如 nonfunctioning） | <u>10</u> | Chromogranin A、GI hormone profile ᵃ（glucagon、pancreatic polypeptide、VIP） | MRI abdomen, EUS（每年） |
| **Pituitary — Prolactinoma** | <u>5</u> | Prolactin | None |
| **Pituitary — Somatotropinoma** | <u>5</u> | IGF1 | None |
| **Pituitary — Other adenoma**（如 NF NET） | <u>10</u> ᵇ | None（除非有功能性腫瘤之症狀/徵象，如 corticotroph adenoma） | MRI pituitary（每 3 年） |
| **Adrenocortical** | <u><10</u> | None（除非功能性腫瘤之症狀/徵象，或影像 >1 cm） | MRI abdomen（每年） |
| **Thymic / bronchial carcinoid** | <u>15</u> | None | CT 或 MRI chest（每 1–2 年） |

ᵃ Chromogranin A、pancreatic polypeptide、glucagon 在 NF-PNET 可升高，但 **敏感度/特異度低**，價值有爭議。
ᵇ Pituitary tumor 在 MEN1 病人最年輕 5 歲即見；若無症狀/徵象/生化證據，pituitary imaging 可延至 >10 歲以與 pancreatic imaging 同步。

📊 **表格解讀（臨床意義與易混淆處）**：

- **生化 vs 影像不對稱**：parathyroid、gastrinoma、insulinoma、prolactinoma、somatotropinoma **只需生化、不需影像（None）**；需要 **影像** 的是 other PNET（MRI/EUS 每年）、other pituitary（MRI 每 3 年）、adrenocortical（MRI 每年）、thymic/bronchial（CT/MRI chest 每 1–2 年）。
- **起始年齡兩極**：最早 = **5 歲**（insulinoma、prolactinoma、somatotropinoma）；最晚 = **20 歲（gastrinoma）**、**15 歲（thymic/bronchial）**。
- **Adrenocortical 起始 <10 歲、影像 MRI 每年**，但生化只在功能性或 >1 cm 才驗 → 易與其他「每年影像」項目混淆。

### 🧠 起始年齡記憶法

| 年齡 | 項目 | 口訣 |
|---|---|---|
| **5** | Insulinoma、Prolactinoma、Somatotropinoma | 「**5 歲三胞胎**：胰島素瘤 + 兩個垂體功能瘤」 |
| **<10** | Adrenocortical | 「腎上腺**未滿 10**」 |
| **8** | Parathyroid | 「副甲狀腺**先 8 歲**」 |
| **10** | Other PNET、Other pituitary（可延至 >10） | 「**10 歲影像開跑**（胰 + 垂體）」 |
| **15** | Thymic/bronchial carcinoid | 「胸腔**15**」 |
| **20** | Gastrinoma | 「胃泌素瘤**最晚 20**」 |

### ⚠️ 兩大爭議區（起始年齡與影像方式）

1. **NF pancreatic NET**：
   - 現行指引建議自 **10 歲** 開始 pancreatic imaging（second decade 高 penetrance 支持）
   - 部分中心主張延至 **≥16 歲**
   - 近期研究建議 **13–14 歲** 起篩（依「臨床相關」NF-pNET[≥2 cm 或快速生長] 預測頻率 ~<u>2.5%</u>）
2. **Thymic NET**：生長快、病程兇 → 傾向 thoracic CT/MRI 每 1–2 年；但此瘤僅見於少數 MEN1 病人，**高頻率掃描（CT 累積輻射）可能不恰當**
- **結論**：需 **個別化**，依資源與病人意願調整，病人應參與決策。

> 📌 **重點 (High-Yield)**：
> - 起始年齡必背：**parathyroid 8、insulinoma/prolactinoma/somatotropinoma 5、gastrinoma 20、thymic/bronchial 15、adrenal <10、PNET/pituitary 影像 10**。
> - 影像頻率：**pancreas MRI/EUS 每年、pituitary MRI 每 3 年、adrenal MRI 每年、chest CT/MRI 每 1–2 年**。
> - 兩大爭議：**NF-pNET 起始年齡（10 vs 16 vs 13–14）** 與 **thymic NET 掃描頻率/輻射**。
