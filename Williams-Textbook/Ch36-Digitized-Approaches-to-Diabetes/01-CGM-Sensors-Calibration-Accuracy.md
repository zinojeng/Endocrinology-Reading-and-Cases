# Ch.36 CGM 感測器、校正與準確度（CGM Sensors, Calibration & Accuracy）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — Sensor Calibration and Accuracy、為何 CGM 優於 SMBG 與 HbA1c、管理 hypoglycemia 與 glycemic variability，含 Table 36.1（各 CGM 系統屬性）

---

## 🩸 為什麼需要 continuous glucose monitoring (CGM)？

糖尿病的 glucose monitoring 標準照護長期以來是 <u>self-monitoring of blood glucose (SMBG)</u>，即以 fingerprick 採 **capillary blood**（毛細血管血）測量血糖（Fig. 36.1）。但這套方式有先天限制：

- **採樣稀疏 (sparse sampling)**：即使一天做到 **7-point profile**（三餐前後 + 睡前各一次），仍無法完整捕捉全日 glycemic profile。
- **疼痛與順從性差**：fingerprick lancing 會痛，導致 engagement 不佳，成為達標的 barrier。
- 大多數 **type 1 diabetes (T1D)** 與 **type 2 diabetes (T2D)** 患者都達不到建議的每日 SMBG 頻率 → 影響血糖控制、增加長期併發症風險。

因此可穿戴式 CGM 技術越來越普及，特別是用於 **insulin therapy** 的患者。

🔑 CGM 的基本原理：

- 量測 **interstitial fluid**（組織間液）中的 glucose，位於 **subcutaneous space**（皮下空間）。
- 兩種感測器型態：
  - <u>Transcutaneous（經皮）</u>：細 filament（細絲）穿過皮膚插入皮下（Fig. 36.3）。
  - <u>Implantable（植入式）</u>：感測器本體直接植入皮下組織。
- glucose 讀數每 **1 至 5 分鐘** 無線傳輸一次，傳到 reader、smartphone/smartwatch app，或在 **automated insulin delivery (AID)** 系統中傳到 insulin pump。
- **intermittently scanned CGM (isCGM)**：只有當使用者主動以 reader 或 app **掃描 (scan)** 感測器時才傳資料。

📅 穿戴時間 (wear time)：

- Transcutaneous 感測器：**7 至 14 天**，到期換新。
- Implantable 系統：目前可傳資料長達 **180 天** 才需更換。
- 所有感測器的表現會隨以下因素變化：
  - 穿戴週期（early / middle / late）
  - reference glucose 水平（high / in-range / low）
  - glucose 變化速率（rate of change）

📜 歷史與 nonadjunctive use：

- 第一代現代 CGM 於 **2000 年** 上市，作為 **diagnostic tool**，提供 **72 小時 retrospective data**，需以 SMBG 校正；當時 **不准** 用於 insulin dosing。
- 如今多款 CGM 已核准在 **無需確認性 SMBG (no confirmatory SMBG)** 的情況下做 insulin dosing 與 titration 決策，稱為 <u>nonadjunctive use（非輔助性使用）</u>。

> 📌 **重點 (High-Yield)**：
> - CGM 量的是 **interstitial fluid glucose**，不是血糖 → 存在 time-lag。
> - 感測器分 **transcutaneous（7–14 天）** 與 **implantable（達 180 天）** 兩類。
> - **isCGM** 需主動掃描才傳資料，real-time CGM 則自動連續傳。
> - **Nonadjunctive use** = 可不必再做 fingerprick 確認即可決定胰島素劑量，是 CGM 進化的關鍵里程碑。

---

## 🔬 Sensor Calibration（感測器校正）

不同 CGM 對 calibration 的需求不同，這會影響個別患者的裝置選擇（因為涉及 user engagement 與準確度）：

| 校正方式 | 機制 | 是否需 SMBG fingerprick | 代表裝置 |
| --- | --- | --- | --- |
| **Factory calibration（出廠校正）** | 出廠已校正，使用者完全不需校正 | ❌ 不需 | FreeStyle Libre 全系列、Dexcom G7、Medtronic Guardian 4/Simplera |
| **User / SMBG calibration（使用者校正）** | 每日以 SMBG fingerprick 校正（多為 twice-daily） | ✅ 需要 | Dexcom G4/G5、Medtronic Guardian Connect/3、Eversense E3 |
| **Calibration code（校正碼）** | 使用者在貼上感測器前輸入隨附的 calibration code | ❌ 不需 fingerprick（但需輸碼） | Dexcom One、G6 |

📊 表格解讀：

- **Factory calibrated** 是趨勢主流：減少使用者負擔、提升 engagement，因為不需做痛苦的 fingerprick。
- **calibration code** 與 factory calibration 容易混淆 → calibration code 仍是出廠提供的校正資訊，只是需使用者**手動輸入一組碼**，不需扎手指做 SMBG。
- 需 **SMBG 校正** 的裝置（如 Dexcom G4/G5、Medtronic Guardian、Eversense）有額外風險：若使用者因不適或技術不佳而**不願意/做不好 SMBG**，會直接拖累 CGM 系統的 accuracy。
- 易混淆考點：**Eversense E3（植入式）** 雖然 wear time 長達 180 天，但仍需 **twice-daily SMBG** 校正。

⚠️ 早期準確度變異的兩個情境（fellow 必背）：

- **Insertion-site trauma + 局部 glucose bioavailability 下降** → 感測器**剛貼上後**準確度會暫時變差。
- <u>Pressure-induced sensor attenuation（壓力誘發訊號衰減）</u> → 在貼附部位受壓時（例如 **趴睡 / sleeping prone**）會出現假性低值。
- 現行系統已能適應這些情境，在 **成人** 無證據顯示造成傷害；但 **acute neonatal care（急性新生兒照護）** 必須對此特別警覺。

> 📌 **重點 (High-Yield)**：
> - 三種校正：**factory calibration / user (SMBG) calibration / calibration code**。
> - calibration code ≠ SMBG calibration：前者只需輸碼，後者要扎手指。
> - 剛貼上（insertion trauma）與受壓（趴睡，pressure attenuation）是兩個典型的準確度暫時失真情境。
> - 新生兒急性照護使用 CGM 須特別注意上述失真。

💡 **記憶法（校正三型）**：「**廠、碼、扎**」
> **廠**（factory，免動手）→ **碼**（code，輸個碼）→ **扎**（SMBG，扎手指）。越往後使用者負擔越重，越依賴 user 配合度。

---

## 📏 Sensor Accuracy 與 MARD

監管機關評估準確度的方式：將 interstitial fluid sensor 讀數與**同時**抽取、以 reference blood glucose analyzer 量測的血糖值比較。

🧮 **Mean Absolute Relative Difference (MARD)**：

- 定義：CGM 量測值與同步 reference 值之間的**平均絕對相對差異**（百分比）。**數字越低越準**。
- 現行 CGM 的 MARD 範圍約 **8% 至 14%**，與 SMBG 血糖機的寬廣準確度範圍相比表現良好。
- 核准用於 **nonadjunctive insulin dosing/titration** 或搭配 **AID** 的裝置，MARD 通常 **低於 10%**。
- ⚠️ 但：**尚無前瞻性臨床研究** 證明「低 MARD」是必要條件，更低 MARD 的確切臨床意義也尚未完全評估。

⏱️ **Time-lag（時間延遲）**——血液 vs 組織間液：

- blood 與 interstitial fluid 是**不同生理區室 (compartments)**，glycemic dynamics 不同。
- 血糖變化反映到 interstitial fluid 的平均 time-lag 約為 **3 至 15 分鐘**。
- 當兩區室間 glucose 的生理變化速率 **> 2.0 mg/dL/min（0.1 mmol/L/min）** 時，time-lag 可能更大。
- 臨床意涵：在血糖**快速變化**（如運動後、餐後、低血糖矯正中）時，CGM 與指尖血糖的差距會被放大。

🧭 **Consensus error grid（共識誤差網格）**：

- 另一種評估系統準確度與精密度的工具，評估 sensor 讀數誤差的**臨床意義**，依誤差落在哪個 zone 賦予不同 **風險等級**。
- 最具臨床重要性的誤差：在生理性**低血糖**狀態下，CGM 卻顯示**高值** → 導致誤打 insulin → 進一步推升 **severe hypoglycemia** 風險。

> 📌 **重點 (High-Yield)**：
> - **MARD 越低越準**；現行 CGM 約 **8–14%**，nonadjunctive/AID 用裝置通常 **< 10%**。
> - 「低 MARD 一定更好」尚無前瞻性證據支持——這是常見的陷阱題。
> - blood ↔ interstitial fluid **time-lag 3–15 分鐘**，血糖快速變化（>2.0 mg/dL/min）時更明顯。
> - **Consensus error grid** 評的是「誤差的臨床後果」，最危險情境＝低血糖卻讀成高值而誤打胰島素。

💡 **MARD 方向口訣**：「**M 越小越神準**」（MARD 數字小 = sensor 準）。

---

## 📊 Table 36.1：各 CGM 系統感測器屬性（Attributes of Glucose Sensors Used by Available CGM Systems）

| Device | Type of Sensor | Calibration | Wear Time (Days) | Wear Site | Alarms | Separate Transmitter | Warm-up Period | Scanning Needed |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Abbott FreeStyle Libre system | Transdermal | Factory calibrated | 14 | Back of upper arm | No | No | 60 min | Yes |
| Abbott FreeStyle Libre 2 system | Transdermal | Factory calibrated | 14 | Back of upper arm | Optional high and low glucose | No | 60 min | Yes |
| Abbott FreeStyle Libre 3 system | Transdermal | Factory calibrated | 14 | Back of upper arm | Optional high and low glucose | No | 60 min | No |
| Dexcom One | Transdermal | Factory-supplied calibration code | 10 | Back of arm, abdomen, buttocks (age 2–17 yr) | Optional high and low glucose | Yes | 2 hr | No |
| Dexcom G4 & G5 | Transdermal | Twice-daily SMBG test | 7 | Back of arm, abdomen, buttocks (age 2–17 yr) | High and low alerts | Yes | 2 hr | No |
| Dexcom G6 | Transdermal | Factory-supplied calibration code | 10 | Back of arm, abdomen, buttocks (age 2–17 yr) | High and low alerts; Predictive | Yes | 2 hr | No |
| Dexcom G7 | Transdermal | Factory-supplied calibration code | 10 | Back of arm, abdomen, buttocks | High and low alerts; Predictive | No | 30 min | No |
| Medtronic Guardian Connect | Transdermal | Twice-daily SMBG test | 7 | Abdomen, back | High and low alerts; Predictive | Yes | 2 hr | No |
| Medtronic Guardian 3 | Transdermal | Twice-daily SMBG test | 7 | Back of arm, abdomen, buttocks (age 7–13 yr) | High and low alerts; Predictive | Yes | 2 hr | No |
| Medtronic Guardian 4 | Transdermal | Factory calibrated | 7 | Back of arm, abdomen, buttocks | High and low alerts; Predictive | Yes | 2 hr | No |
| Medtronic Simplera | Transdermal | Factory calibrated | 7 | Back of upper arm | High and low alerts; Predictive | No | 2 hr | No |
| Roche Senseonics Eversense E3 | Implantable | Twice-daily SMBG test | 180 | Implanted under skin on the upper arm | Optional high and low glucose | Yes | 24 hr | No |

*註：表中為 T1D/T2D 臨床研究最常用的系統，市面尚有其他 CGM。SMBG = self-monitoring of blood glucose。*

📊 表格解讀：

- **Type of Sensor**：除 **Eversense E3 為 implantable（植入式）** 外，其餘皆為 **transdermal（經皮）**。植入式 = 唯一 wear time 達 **180 天** 者。
- **Calibration** 欄是最高頻考點：
  - **Factory calibrated**：FreeStyle Libre 全系列、Medtronic Guardian 4、Simplera。
  - **Factory-supplied calibration code**：Dexcom One / G6 / G7（注意：是輸碼，非 SMBG）。
  - **Twice-daily SMBG test**：Dexcom G4/G5、Medtronic Guardian Connect/3、**Eversense E3**。
- **Wear Time**：Libre 系列 **14 天**最長（transcutaneous 中）；Dexcom 系列 **10 天**；Medtronic 系列 **7 天**；Eversense **180 天**（implantable）。
- **Alarms（警報）**：
  - 最早的 **FreeStyle Libre（第一代）= No**（無警報）。
  - Libre 2/3 起加入 **optional high/low glucose** 警報。
  - Dexcom G6/G7、Medtronic 全系列具 **Predictive alerts（預測性警報）**——可在到達低/高血糖前先警示，這是 AID 與低血糖防護的關鍵。
- **Separate Transmitter（獨立發射器）**：
  - 需獨立 transmitter：Dexcom One/G4/G5/G6、Medtronic Guardian 系列、Eversense E3。
  - **不需** 獨立 transmitter（一體式 all-in-one）：**FreeStyle Libre 全系列、Dexcom G7、Medtronic Simplera**。
  - 考點對比：**Dexcom G6 需 transmitter，G7 不需**（G7 改為一體式、warm-up 也縮短）。
- **Warm-up Period（暖機時間）**：
  - FreeStyle Libre 全系列：**60 min**。
  - Dexcom One/G4/G5/G6：**2 hr**；**Dexcom G7 縮短至 30 min**（全表最短，implantable 除外）。
  - Medtronic 全系列：**2 hr**。
  - **Eversense E3：24 hr**（植入式，最長）。
- **Scanning Needed（需掃描 = isCGM）**：
  - **需掃描**：FreeStyle Libre 與 Libre 2（isCGM）。
  - **不需掃描（real-time / rtCGM，自動傳輸）**：FreeStyle Libre 3、所有 Dexcom、所有 Medtronic、Eversense E3。
  - 考點：**Libre 3 是 Libre 系列中第一個不需掃描者**，向 real-time CGM 靠攏。

💡 **比較表記憶法（Dexcom G6 → G7 的世代差異）**：

| 屬性 | Dexcom G6 | Dexcom G7 |
| --- | --- | --- |
| Warm-up | 2 hr | **30 min**（更快） |
| Separate transmitter | **需要** | **不需要**（一體式） |
| Wear time | 10 天 | 10 天（相同） |
| Calibration | calibration code | calibration code（相同） |

> 一句話記 G7 的進化：「**更快暖機、不用發射器**」（30 分鐘 + all-in-one）。

> 📌 **重點 (High-Yield)**：
> - **Eversense E3** 是唯一 implantable、唯一 180 天、warm-up 最長（24 hr），且仍需 **twice-daily SMBG** 校正。
> - **FreeStyle Libre 全系列 warm-up 最短（60 min）**；**Dexcom G7 = 30 min**（transcutaneous 最短）。
> - **isCGM（需掃描）**＝Libre 與 Libre 2；**Libre 3 起不需掃描**。
> - **Predictive alarms** 見於 Dexcom G6/G7 與 Medtronic 全系列；第一代 Libre 完全無警報。
> - 一體式（無獨立 transmitter）：Libre 全系列、**Dexcom G7**、Medtronic Simplera。

---

## ⚖️ CGM 為何是 Transformative：SMBG 與 HbA1c 的局限

患者隨時可用 fingerprick SMBG 測一個時間點的血糖，但會痛、一天難做幾次；而 HbA1c 雖是長期併發症的成熟 marker，卻**無法反映每日血糖波動**。CGM 能在所有關注時段提供**客觀**資訊。

### 🩸 The Limitations of SMBG Testing

- SMBG 提供的是**孤立的瞬間快照 (isolated snapshots)**。
- CGM 則 **minute-by-minute** 收集，給出**全日（含夜間）完整視野**，涵蓋高/低血糖期與變異時的 peaks and troughs。
- Fig. 36.2 的示範：同一天，SMBG 8 點快照可能**漏掉**高低 glycemic excursions；CGM 連續曲線則完整呈現夜間與全日波動（而且現實中沒人會一天扎 8 次手指）。

### 🧪 The Limitations of HbA1c

- HbA1c 是過去 **2–3 個月** 平均血糖控制的公認指標，1969 年首次與糖尿病連結，與 mean fasting glucose、mean daily glucose 相關。
- **UKPDS** 與 **DCCT** 證明：以 HbA1c 衡量的血糖改善可降低 retinopathy、nephropathy、neuropathy、腎衰竭等長期併發症 → HbA1c 成為 glycemic control 的客觀指標與 morbidity/mortality 的 **gold standard marker**。
- 但 HbA1c 的**致命盲點**：
  - **看不到 day-to-day 的波動**：HbA1c 完全相同的兩人，可有截然不同的 hyperglycemia/hypoglycemia 型態（Fig. 36.4），治療需求大不同。
  - 受 **non-glycemic factors（red blood cell turnover、homeostasis）** 影響 → HbA1c 可能**高估或（更常見地）低估**平均血糖。
  - CGM 證實：對於 HbA1c **高估** 平均血糖的人，可能造成 **treatment overintensification（過度強化治療）** → 增加 **hypoglycemia** 風險。

💡 **核心對比表：SMBG vs CGM vs HbA1c**

| 面向 | SMBG（fingerprick） | CGM | HbA1c |
| --- | --- | --- | --- |
| 時間解析度 | 瞬間快照 | 連續（1–5 分鐘） | 2–3 個月平均 |
| 看得到 hypoglycemia？ | 偶爾（剛好測到才行） | ✅ 完整捕捉 | ❌ 看不到 |
| 看得到 glycemic variability？ | ❌ 幾乎不行 | ✅ peaks/troughs 全現 | ❌ 看不到 |
| 夜間覆蓋 | 通常缺 | ✅ 含夜間 | n/a |
| 受非血糖因素干擾 | 否 | 否 | ✅（RBC turnover 等） |
| 長期併發症關聯 | 間接 | 間接（TIR 等指標） | ✅ gold standard |

> 📌 **重點 (High-Yield)**：
> - **HbA1c 的兩大盲點**：① 看不到 **hypoglycemia 與 glycemic variability**；② 受 **non-glycemic（RBC）因素** 影響而高估/低估。
> - HbA1c 相同 ≠ 血糖型態相同（Fig. 36.4 經典圖）。
> - HbA1c **高估** 平均血糖時，盲目降 HbA1c 會導致 overintensification → 低血糖。
> - CGM 同時補足 SMBG（無連續性）與 HbA1c（無波動/低血糖視野）的缺口。

---

## 🔺 CGM 讓多重風險因子可被管理：Triangle of Diabetes Care

HbA1c 讓我們理解 hyperglycemia 的長期後果，但 CGM 揭示：**避免 hypoglycemia** 與 **限制 glucose variability** 同等重要。三者構成 <u>"triangle of diabetes care"（糖尿病照護三角）</u>（Fig. 36.5）：

- 頂點：**Improve overall glucose levels（HbA1c）**
- 左：**Avoid hypoglycemia**
- 右：**Limit glucose variability**
- 中心：**Better outcomes for people with diabetes**

📈 為何不能只盯 HbA1c 往下壓：

- 五大里程碑試驗的 meta-analysis（**UKPDS、ACCORD、ADVANCE、VADT、PROactive**）顯示：在 T2D，intensive HbA1c 控制有 cardiovascular benefit，但**未改善整體 mortality**。
- HbA1c 與併發症/死亡的關係**並非直線**，而是 **U 形或 J 形曲線** → 「HbA1c 越低未必越好」。
- **T1D（2018，瑞典 national diabetes registry，n = 33,915）**：即使達到 optimal HbA1c **≤6.9%（52 mmol/mol）**，相較無糖尿病者（每人配對 5 名年齡、性別相符的對照），仍有 **兩倍 (twofold)** 的全因死亡或心血管死亡風險 → 達到 glycemic target 仍**掩蓋了其他增加 CV 風險的因子**。

> 📌 **重點 (High-Yield)**：
> - **Triangle of diabetes care**＝改善 HbA1c + 避免 hypoglycemia + 限制 glycemic variability。
> - 五大試驗（UKPDS/ACCORD/ADVANCE/VADT/PROactive）：T2D intensive control 有 CV 益處但**不降總死亡**。
> - HbA1c 與結局呈 **U/J 形曲線**——過低有害。
> - 瑞典 T1D 研究：HbA1c ≤6.9% 仍有 **兩倍** 死亡/CV 風險 vs 非糖尿病者。

---

## ⚠️ The Need to Manage Hypoglycemia（管理低血糖）

Hypoglycemia 是 insulin 與 insulinotropic（促胰島素）藥物治療公認的不良後果：

- **神經學後果**：cognitive function 受損、confusion、irrational behavior、drowsiness，嚴重者 **seizures 與 coma**。
- **社會/職場**：embarrassment、physical injury。
- **致死性**：acute hypoglycemia 估計佔 **40 歲以下 T1D 死亡的 up to 10%**。
- **心血管連結**（三條機轉證據鏈）：
  - 增加 **cardiac dysrhythmia（心律不整）**。
  - 增加 inflammatory responses + **endothelial-cell dysfunction** → 促 atherosclerosis。
  - 擾亂 coagulation system → **prothrombotic（促血栓）** 環境。

> 📌 **重點 (High-Yield)**：
> - Acute hypoglycemia ≈ 佔 **<40 歲 T1D 死亡的 10%**（高頻數字）。
> - 低血糖致 CV 傷害三機轉：**心律不整、內皮功能障礙/發炎、促血栓**。
> - 這正是 CGM **predictive low alerts** 與 AID 低血糖防護價值所在（呼應 Table 36.1 的 alarm 欄）。

---

## 🔁 The Need to Manage Glycemic Variability（管理血糖變異）

CGM 資料強化了 glucose variability 與 cardiovascular pathology 的連結：

- T1D 與 T2D 中，**實驗誘發的 hypo↔hyper 擺盪**，比起**持續高血糖**，造成更顯著的 **endothelial dysfunction 與 oxidative stress**。
- 任何原因住院的糖尿病患者，**glycemic swings** 與 **較高 mortality 及較長住院天數** 相關。
- T2D 中，**reactive oxygen metabolites（活性氧代謝物）** 與 glucose variability 相關：
  - 與每日 **mean amplitude of glucose excursions（MAGE）** 顯著正相關。
  - 也與**日間差異（mean differences in glucose between days）** 相關。

💡 **記憶要點**：變異本身就是傷害——「**忽高忽低比一直高更傷血管**」（swings > sustained hyperglycemia 在 endothelial/oxidative stress 上）。

> 📌 **重點 (High-Yield)**：
> - **血糖擺盪（variability）** 對 endothelial dysfunction/oxidative stress 的傷害 **大於 sustained hyperglycemia**。
> - 住院糖尿病患的 **glycemic swings** ↔ 較高死亡率與較長住院日。
> - Glucose variability 與 **reactive oxygen metabolites、MAGE** 正相關 → variability 是**獨立風險因子**。

---

## 📱 CGM 即時顯示範例（Trend Arrows，Fig. 36.6）

兩款已核准 nonadjunctive use（可直接做 insulin dosing 決策）系統的主畫面範例：

| 系統 | Current Glucose | Trend（趨勢箭頭） | 附加訊息 | 時間 |
| --- | --- | --- | --- | --- |
| **Dexcom G7** | 5.7 mmol/L | **Falling rapidly（雙箭頭向下）** | Alert：20 分鐘內將達 3.1 mmol/L | 10:30 |
| **FreeStyle Libre** | 112 mg/dL | **Rising（斜箭頭向上）** | GLUCOSE IN RANGE | 10:23 |

📊 表格解讀：

- **Trend arrow（趨勢箭頭）** 反映 **rate of change**，是 nonadjunctive dosing 的核心資訊——不只看當下值，更看「往哪走、走多快」。
- **Dexcom G7 範例**：falling rapidly = 變化 **>2.0 mg/dL/min（>0.1 mmol/L/min）**，並**預測**即將低血糖（雙箭頭向下）→ 應暫緩/減少胰島素、考慮補糖。
- **FreeStyle Libre 範例**：rising = 變化 **1.0–2.0 mg/dL/min（0.06–0.1 mmol/L/min）**，雖在範圍內但正上升 → 劑量決策需把上升趨勢計入。
- 完整 trend arrow rate of change 對照見 **Table 36.2**（本節未涵蓋）。

> 📌 **重點 (High-Yield)**：
> - Nonadjunctive dosing 要**同時看 glucose 值 + trend arrow**；雙箭頭向下＝快速下降（>2.0 mg/dL/min）需警覺低血糖。
> - 趨勢箭頭把前述 **time-lag** 與 **rate of change** 概念落實到床邊決策。

---

## 🧠 全節整合記憶卡

💡 **「CGM 三角 + 三盲點」總口訣**：
- **三角 (Triangle)**：降 HbA1c、避 hypoglycemia、限 variability。
- **HbA1c 三盲點**：① 看不到低血糖、② 看不到變異、③ 受 RBC 等非血糖因素干擾。
- **MARD 越小越準**（8–14%；nonadjunctive/AID <10%，但低 MARD 更好「無前瞻證據」）。
- **校正三型「廠/碼/扎」**；**Eversense** 是植入式特例（180 天、24 hr warm-up、仍需扎手指校正）。
