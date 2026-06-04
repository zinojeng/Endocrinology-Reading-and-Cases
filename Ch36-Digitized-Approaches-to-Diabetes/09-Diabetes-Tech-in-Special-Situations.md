# Ch.36 特殊情境中的糖尿病科技：住院、ICU、NICU/PICU、孕期與未來方向（Diabetes Technologies in Special Situations）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — 住院 / 重症 / 新生兒 / 兒科 ICU / 孕期之 CGM、insulin pump、AID 應用，及本章 Future Directions
---

## 🏥 住院病人血糖控制的科技應用（Glycemic Control in Hospitalized Patients）

### 為什麼住院血糖管理很重要

- 在**非重症住院病人**中，每 4 人就有 1 人（**1/4, 25%**）有 diabetes。
- 另有約 **25%** 住院病人因下列原因出現 hyperglycemia，但**未必有 diabetes 病史**：
  - 導致住院的疾病本身（如 infections）。
  - 住院中的處置（如 surgeries、parenteral nutrition）。
- 在 critically ill 病人、neonates、infants、adults 中，即使**沒有 preexisting diabetes**，hyperglycemia 的頻率更高。
- **臨床意義**：diabetes 與 hyperglycemia 都與下列結果相關：
  - <u>住院時間延長</u>（prolonged hospitalization）。
  - <u>併發症增加</u>。
  - <u>死亡率上升</u>。
- 因此 CGM、insulin pumps、AID systems、bedside algorithms 在住院情境受到越來越多關注，潛在好處包括改善短期與長期臨床預後、並降低住院成本。

### ⚠️ 住院情境帶來的特殊挑戰（Fig. 36.12 核心概念）

住院本身使血糖科技的應用變得困難，主因是**insulin requirements 高度變異**且 hyperglycemia 機轉異質（例如 sepsis、neurologic compromise 的成人，或 neonatal care）：

- **Insulin sensitivity / requirements 大幅波動**，原因：
  - 未受抑制且不規則的 hepatic glucose production。
  - 周邊組織 glucose uptake 下降。
  - 藥物誘發的 insulin resistance（drug-induced insulin resistance）。
- 臨床醫師必須持續評估病情並調整 insulin regimen：
  - 對住院前已用 insulin 者 → 動態調整。
  - 對先前 insulin-naïve 者 → 評估是否需新起始 insulin（可能只在住院期間需要，也可能延續至出院）。
- 其他障礙：
  - 營養供給方式改變（parenteral nutrition vs. enteral nutrition）。
  - 長時間 immobilization 可能影響 glucose sensor 準確度。
  - 醫療單位**不熟悉**新科技，採用負擔大。

> 💡 **記憶法 — Fig. 36.12「住院科技 5 大挑戰」(NICU 為例)**：
> 用 **「TVA-AT」** 記 → **T**argets（functional vs operational 血糖目標）、**V**ariability（↑血糖變異 / ↓insulin sensitivity）、**A**ccuracy（CGM 準確度）、**A**lgorithms（需專屬演算法）、**T**raining（人員訓練）。

### 📊 住院血糖目標（Glycemic Targets）

| 族群 | 建議 / 常用目標 | mmol/L | 來源 / 備註 |
|---|---|---|---|
| 非重症成人（有或無 diabetes 病史） | **100–180 mg/dL** | 5.6–10.0 | Endocrine Society 建議之 operational target |
| Preterm neonates（臨床試驗常用） | **72–144 mg/dL** | 4–8 | 基於實務考量，缺乏「functional measure」定義臨床有意義閾值 |
| Neonates / 兒科住院病人 | 無共識 | — | 依 clinical scenario 調整，最佳目標仍有爭議 |

📊 **表格解讀**：

- **operational vs functional target**：preterm 的 72–144 mg/dL 是「operational（操作型）」目標——只是試驗實務上採用，並非根據「哪個 glucose threshold 真正對應臨床結果」的 functional 證據而定。這是 Fig. 36.12 中「functional vs operational glycemic targets」的核心。
- **雙向風險（考點）**：
  - Hyperglycemia → ↑morbidity、↑mortality、住院延長。
  - **Tight glycemic control**（不論 IV 或 SC insulin）→ ↑hypoglycemia 風險；而 hypoglycemia 在 ICU 情境**會進一步增加 mortality**。
- **易混淆**：成人非重症目標（100–180）vs preterm（72–144）數值不同，務必分清族群。

### IV insulin 的限制

- 雖然急需在「不增加 hypoglycemia」前提下治療住院 hyperglycemia，但 **IV insulin delivery** 受限於：
  - 增加醫護人員負擔。
  - 需頻繁血糖檢測以 titrate insulin drip。
  - 頻繁操作 IV line → infection 風險。
- 在 critically ill neonates / pediatric 病人更關鍵：**minimize blood drawn（減少抽血量）**在 NICU 與 PICU 至為重要。

> 📌 **重點 (High-Yield)**：
> - 非重症住院成人血糖 operational target = **100–180 mg/dL (5.6–10.0 mmol/L)**（Endocrine Society）。
> - Preterm neonate 試驗常用 target = **72–144 mg/dL (4–8 mmol/L)**，屬 operational 而非 functional。
> - Tight control 在 ICU 會增加 hypoglycemia，而 hypoglycemia **本身增加 mortality**——這是「為何別過度壓血糖」的關鍵論述。
> - NICU/PICU 的核心限制之一是「**減少抽血量**」，這正是 CGM/bedside advisor 的切入點。

---

## 🩸 NICU 的糖尿病科技：CGM 與 Bedside Advisors

### 新生兒血糖的生理背景

- 出生後所有 infant 因 placenta 連續供糖中斷，會有**短暫 glucose 下降**。
- **Preterm infant** 風險更高，因為：
  - 缺乏 glycogen stores（通常在 **third trimester** 才累積）。
  - gluconeogenesis 不足。
- 結果：**>50%** 早產兒在出生後最初幾天出現 hypoglycemia 或 hyperglycemia，**不論母親是否有 gestational/pregestational diabetes**。

### 兩種不同機轉（重要區分）

| 族群 | 主要血糖問題機轉 | 對應介入 |
|---|---|---|
| **Preterm（早產兒）** | glucose 攝取大量依賴 IV 供給 → 需精準調控 | CGM + dedicated algorithm 維持目標血糖 |
| **Late preterm / term（晚期早產 / 足月）** | 主要為**母體孕期 hyperglycemia**所致 neonatal hypoglycemia | 早期 nutrition、預防性 **glucose gel** + CGM 早期偵測 hypoglycemia |

📊 **表格解讀**：

- **preterm 是「供給依賴型」**：因外源 IV 葡萄糖供應，血糖易上下波動 → CGM 驅動 algorithm 調整 infusion。
- **term/late preterm 是「母源型」**：母親孕期高血糖造成胎兒高胰島素，出生後易低血糖 → 重點在早期餵食 / glucose gel，CGM 用於**早期偵測**。
- **神經發育考點**：glucose 是 neonatal developing brain 的主要燃料，hypo 與 hyper 都可能嚴重影響 preterm 神經發育。
  - 曾有 neonatal hypoglycemia 的新生兒，**fourth-grade（四年級）literacy 測驗分數與熟練度低 20%**。
  - hypo 與 hyper 都可能影響 preterm 的 long-term neurodevelopment。

### CGM 在 NICU 的證據與實作

- 現況：CGM **尚非** standard neonatal care，但多個試驗顯示其**安全且有效**協助達成 tight neonatal glycemic control。
- 準確度：**older generation 裝置**在 preterm neonates 已具足夠準確度可驅動治療決策（**MARD <14%**）。
- **Term neonates** 的 CGM 證據仍有限。
- 試驗族群：very preterm、extremely preterm，出生體重 **<1000 g**。
- 放置位置：通常置於**大腿外側（lateral side of thigh）**，依製造商指示使用，可校正或不校正。

### Bedside Advisor 的概念（Fig. 36.13）

對照「standard of care」vs「CGM bedside advisor」：

| 項目 | Standard of care | CGM bedside advisor |
|---|---|---|
| 血糖資料來源 | Blood Glucose Meter，**3–4 次/天** | CGM sensor，**24/7 連續資料** |
| 警示 | 無 | Hypo/Hyper alerts 送至 laptop/bedside algorithm |
| 調整方式 | Healthcare provider **週期性**調整 glucose/insulin infusion | algorithm 提示，provider **即時（real-time）**調整 infusion |

📊 **表格解讀**：

- bedside advisor 的精髓 = **real-time CGM 值餵入 control algorithm → 引導 glucose 與 insulin infusion 的即時調整**。
- 試驗結果（兩個 pivotal trials）：
  - 相較 standard of care，**time in target glucose range ↑約 10%**。
  - **無 time in hypoglycemia**（hypoglycemia 定義為 glucose <47 mg/dL（2.6 mmol/L））。
  - 大樣本、無 adverse events → 支持未來將 CGM 納入 neonatal care 的臨床實務改變。

### ⚠️ Preterm CGM 的技術限制（Fig. 36.14 / Table）

| 限制 | 機轉 | 臨床後果 |
|---|---|---|
| **Time lag（時間延遲）** | 血糖**下降**時 → ⇑ positive error；血糖**上升**時 → ⇑ negative error | 真值與量測值不一致，影響決策 |
| **Drift（漂移）** | sensor 表面 corrosion 或 biofilm，同一血糖濃度產生不同電流 | sensor 不穩定，讀值偏移 |
| **Compression artifacts（壓迫偽影）** | 對 sensor 部位壓迫 | 造成「false」hypoglycemia（假性低血糖） |

📊 **表格解讀**：

- 三種限制對應 Fig. 36.14 的三組曲線（BW 1130 g / 1080 g / 1360 g 案例）。
- 另有藥物干擾：**acetaminophen、vitamin C、alcohol、tetracycline** 可干擾 sensor glucose 讀值。
- **重要結論（考點）**：這些限制在臨床試驗中**並未成為主要障礙**——理論限制存在，但實證上可接受。
- **方向記憶（易混淆）**：
  - 血糖**掉**的時候 CGM 偏**高**（positive error）→ 可能延誤治療 hypo。
  - 血糖**升**的時候 CGM 偏**低**（negative error）。
  - compression → 假性 hypo（不是真的低）。

> 💡 **記憶法 — Time lag 方向**：「**降高升低**」——血糖下降時 sensor 顯示偏高、上升時偏低（因組織間液落後血液）。

> 📌 **重點 (High-Yield)**：
> - >50% preterm 在出生數天內出現 hypo 或 hyper，與母親 diabetes 史無關。
> - preterm 低血糖機轉 = glycogen 不足（third trimester 才累積）+ gluconeogenesis 不足。
> - CGM 在 preterm 的準確度 **MARD <14%**（older generation 即可驅動治療），sensor 放**大腿外側**，試驗族群 BW **<1000 g**。
> - Bedside advisor 使 time in target **↑約 10%**，無 time in hypoglycemia（hypo 定義 <47 mg/dL / 2.6 mmol/L）。
> - CGM 三大技術限制：**Time lag（降高升低）、Drift、Compression（假性 hypo）**。

---

## 🩸 PICU 的糖尿病科技：CGM 與 Bedside Advisors

### SPECS Trial（Safe Pediatric Euglycemia in Cardiac Surgery）

- 最早研究之一：用 CGM 引導 **PICU 心臟術後兒童**的血糖採樣頻率。
- 設計：**bedside glucose meter** 的資料餵入 control algorithm → 引導 **IV insulin delivery**。
- 結果：
  - tight glycemic range **80–110 mg/dL（4.4–6.1 mmol/L）**的 time in range 增加。
  - **對 primary outcome（healthcare-associated infections）無影響**。
- 縱貫分析（longitudinal analysis）：
  - 經歷 **moderate to severe hypoglycemia** 者：
    - moderate 定義 **<50 mg/dL（2.7 mmol/L）**。
    - severe 定義 **<40 mg/dL（2.2 mmol/L）**。
  - 這些孩童在 **Bayley-III** cognitive 與 motor 領域分數**較低**（vs 無 mild hypoglycemia 者）。
- **結論**：critically ill children 的 glycemic targets 仍有爭議。

📊 **數值解讀**：

- SPECS 的 tight target（80–110 mg/dL）比成人非重症（100–180）**更嚴格**，這也是為何 hypoglycemia 風險浮現。
- 核心教訓：即使把 time in range 拉高，**hypoglycemia 會傷害神經發育（Bayley-III ↓）**，故不可一味追求嚴格控制。

> 📌 **重點 (High-Yield)**：
> - SPECS：PICU 心臟術後，CGM/algorithm 引導 IV insulin → tight range **80–110 mg/dL** 的 TIR ↑，但**未改善 healthcare-associated infections（primary outcome 陰性）**。
> - moderate/severe hypoglycemia（<50 / <40 mg/dL）→ Bayley-III cognitive & motor 分數較低。
> - 兒科重症的最佳血糖目標**尚無共識**。

---

## 💉 非重症住院病人（有或無 diabetes）的糖尿病科技

### CGM 在非重症住院成人

- 對**已用 insulin** 治療的 diabetes 非重症住院成人：**建議使用 real-time CGM**，但需搭配 **confirmatory bedside point-of-care (POC)** 血糖測試來調整 insulin（優於單用 POC）。
- CGM 的好處：
  - 減少 hyperglycemia（>180 mg/dL / 10.0 mmol/L）的時間。
  - 增加 hypoglycemia（<70 mg/dL / 3.9 mmol/L）的偵測。
- **注意干擾因子**（影響 sensor 讀值）：
  - 藥物：acetaminophen、vitamin C、alcohol、tetracycline。
  - hypoperfusion（低灌流）。
  - 其他損及 CGM 準確度的因素。

### Insulin Pump 在住院期間（ADA / AACE 立場）

- 對使用 insulin pump 的病人，**ADA 與 AACE 主張住院期間維持 pump 和/或 CGM**，條件是：
  - 病人**生理與心智上有能力**繼續使用。
  - 具備必要 supplies。
  - 醫院有**熟悉糖尿病科技的人員**可協助管理。
- **初始評估**是否可續用 pump，需考量：
  - 住院型態（長度、critical vs noncritical unit）。
  - 病人狀態（self-manage 能力）。
  - 將接受的處置類型。
- **孕婦 with diabetes 用 pump 入院待產（labor）**：**AACE Clinical Practice Guideline 建議維持 pump therapy**。
- **最終決定**取決於是否有熟悉裝置的醫護人員；否則應考慮轉為 **basal-bolus MDI regimen**。

### 💡 比較表：住院血糖科技決策

| 情境 | 建議 |
|---|---|
| 非重症、insulin-treated、有 diabetes | real-time CGM **+ POC 確認** 調 insulin |
| 已用 pump、能自我管理、有 supplies、醫院有專業人員 | **維持 pump ± CGM**（ADA/AACE） |
| 孕婦用 pump 入院待產 | **維持 pump**（AACE） |
| 醫院**無**熟悉裝置人員 | 轉 **basal-bolus MDI** |

📊 **表格解讀**：

- 共同關鍵字 = **「醫院是否有熟悉科技的人員」**——這是 pump 能否續用的決定性條件（易考）。
- CGM 在住院仍需 **POC 確認**，不可單獨依 CGM 調 insulin（與門診情境不同）。

> 📌 **重點 (High-Yield)**：
> - 非重症 insulin-treated 住院成人：建議 real-time CGM，但須以 **POC 確認**後再調 insulin。
> - 續用 pump 的三條件：病人有能力、有 supplies、**醫院人員熟悉科技**；否則轉 basal-bolus MDI。
> - 孕婦用 pump 入院待產 → AACE 建議**維持 pump**。
> - CGM 干擾因子記憶：藥物（acetaminophen / vit C / alcohol / tetracycline）+ hypoperfusion。

---

## 🔁 住院病人使用 AID（AID in People Who Are Hospitalized）

### 非重症 + 腸道/靜脈營養（enteral/parenteral nutrition）

- 一個 RCT（非重症、hyperglycemia、接受 enteral/parenteral nutrition、一般內科病房）：
  - 使用 **AID with faster-acting insulin aspart**。
  - time in target **100–180 mg/dL（5.5–10.0 mmol/L）↑超過 30%**（vs 傳統 SC insulin）。
  - **<50% 參與者**有入院前 diabetes 診斷。
  - **但 AID 未顯著減少 time in hypoglycemia** → 未來需以 hypoglycemia 為 primary outcome 的更大型研究。

### 非重症 T2D

- **Fully automated AID without meal announcements（全自動、無需宣告進食）**：
  - 安全地使 target range **100–180 mg/dL** 的 time in range **↑約 25%**，等於**每天多 6 小時**。
  - **未增加 total daily insulin dose**（vs MDI 傳統治療）。
  - **不擾亂病房 workflow**，病人接受度高（這些病人入院前未用過此系統）。
- **限制**：樣本量小、僅在**兩個 hospital sites** 進行 → 需更大型 multicenter trials。

📊 **數值對照（住院 AID 兩大證據）**：

| 研究情境 | AID 類型 | TIR 改善 | 重要附註 |
|---|---|---|---|
| 非重症 + EN/PN | faster-acting insulin aspart AID | **>30%** | <50% 有 diabetes 史；未顯著降 hypoglycemia |
| 非重症 T2D | fully automated, no meal announcement | **~25%（每天 +6 hr）** | 未增 total daily insulin；不擾 workflow；僅 2 院 |

📊 **表格解讀**：

- 兩研究都顯示 AID 在住院能**有效提升 TIR**，但**證據規模有限**（樣本小、site 少）。
- 重要對比：EN/PN 那組「未顯著降 hypo」，提醒 AID 的 hypoglycemia 益處尚待驗證。
- T2D 那組亮點：**未增加總胰島素劑量卻多 6 小時 TIR**——代表更聰明的分配而非更多 insulin。

> 📌 **重點 (High-Yield)**：
> - 住院 AID（EN/PN 情境）TIR **↑>30%**，但**未顯著減少 hypoglycemia**。
> - 住院 T2D 全自動 AID（無 meal announcement）TIR **↑~25%（每日 +6 hr）**，**不增總胰島素**、不擾 workflow。
> - 共同弱點：sample size 小、僅 2 個 hospital sites → 需 multicenter 驗證。

---

## 🤰 孕期使用 AID（AID in Pregnancy）

### 孕期血糖目標

- 孕期 diabetes 婦女建議 near-normal target **63–140 mg/dL（3.5–7.8 mmol/L）**，以防胎兒與產後 hyperglycemia 相關併發症。
- **T1D 孕婦的挑戰**：insulin requirements 全孕期大幅波動，interday glucose variability 高。
- **T1D 的治療目標（pregnancy TIR, TIRp，見 Table 36.3 與 Fig. 36.8）**：
  - **TIRp 63–140 mg/dL（3.5–7.8 mmol/L）>70%** 時間。
  - **<4%** time below 63 mg/dL（3.5 mmol/L）。
  - **<1%** time below 54 mg/dL（3.0 mmol/L）。
- **T2D 與 gestational diabetes 的 evidence-based 孕期目標尚未確立**。

### AID 在孕期的證據

- AID 已在孕婦測試並**證實安全**。
- 一個 **4 週 randomized crossover** 研究：
  - AID 使 tight range **63–140 mg/dL** 的 time **↑約 15%**。
  - **夜間（overnight）**使用時達成 **>70% time in target**（vs SAP therapy）。
- **Extension phase（延長期，最長 14 週）**：time in target **維持**。
- **Ongoing multicenter trial**：測試 AID 於 T1D 婦女，HbA1c 介於 **6.5%（48 mmol/mol）至 10%（86 mmol/mol）**；另有更多試驗進行中。

📊 **數值解讀**：

- 孕期 target（63–140 mg/dL）比一般非孕成人（70–180）**更嚴格、更低**——這是孕期特有，務必記住。
- AID 在孕期最大亮點 = **overnight 控制**達 >70% target，且延長期可維持。
- 注意：**SAP（sensor-augmented pump）= 對照組**，AID 優於 SAP。

> 💡 **記憶法 — 孕期 T1D「7-4-1」三目標**：
> - **7**0% 以上 TIRp（63–140 mg/dL）。
> - **<4%** below 63 mg/dL。
> - **<1%** below 54 mg/dL。

> 📌 **重點 (High-Yield)**：
> - 孕期 diabetes target = **63–140 mg/dL（3.5–7.8 mmol/L）**，T1D 目標「**7-4-1**」（>70% TIRp、<4% <63、<1% <54）。
> - T2D / GDM 的孕期 evidence-based 目標**尚未確立**。
> - 4 週 crossover：AID 使 tight-range time **↑~15%**，**overnight >70% target**（優於 SAP），14 週延長期維持。
> - Ongoing trial 收 T1D HbA1c **6.5%–10%**。

---

## ⭐ Future Directions（本章未來方向）

### 核心理念

- 數位科技已**轉變現代 diabetes 管理**，協助病人與醫護更有效決策，降低長期併發症與疾病負擔。
- 最終極展現 = **AID systems 在 T1D 的廣泛導入**，有效**取代胰臟在 glucose homeostasis 的功能**。
- **未來目標**：使 AID 成為 T1D 的 **standard of care**；並協助所有用 insulin 的 diabetes 婦女順利規劃 pregnancy、產下健康嬰兒。

### CGM 的擴展

- 目標：使 wearable CGM 成為 **T2D 的 standard of care**（如今已是 T1D 標準）。
  - 包含**未使用 insulin** 的 T2D。
  - 包含 pregestational T2D 孕期。
  - 對用 insulin 的 T2D，亦應善用 **smart pens** 記錄與監測 insulin 劑量。
- **CGM-derived metrics 將作為 diabetes 藥物試驗的 primary / secondary outcomes**。
  - 進而使 **U.S. FDA 與 European Medical Agency** 將 CGM-derived metrics 納入新藥 labeling。

### 技術與系統演進

- 預期 insulin delivery devices、glucose sensors、AI 演算法持續改良。
- 特別期待：
  - **Noninvasive sensing（非侵入式感測）**。
  - **Long-term implantable sensors（長期植入式感測器）**，可同時測 glucose、ketones 及其他代謝參數，持續數年。
- 新 diabetes 藥物、formulations、combination formulations 也將專為搭配 diabetes 科技而開發。

### 資料整合與 EMR

- 互聯科技帶來好處也帶來挑戰：**資料標準化與整合**的未滿足需求，含對日益增多的 patient-centered diabetes mHealth apps 的監管。
- 終極目標：建立**完全整合的 EMR**，反映病人完整健康狀態，包括 up-to-date glucometric profile → 促成 specialist 與 primary care 間無縫銜接。
- 結合廣泛實證與 EMR 高密度資料 → **algorithm-based AI** 可協助辨識核心治療調整選項。
- 數位化已創造改變 diabetes 照護的契機（對病人、醫療服務、regulators、payers），但也需要在**態度、教育、科技、服務設計**上的 paradigm shift。

> 💡 **記憶法 — Future Directions「四大主軸」**：
> **「A-C-S-E」** → **A**ID 成 T1D standard、**C**GM 成 T2D standard（含 metrics 入藥物 labeling）、**S**ensors 進化（noninvasive / implantable，測 glucose+ketones）、**E**MR 整合 + AI 決策。

> 📌 **重點 (High-Yield)**：
> - 終極目標：**AID = T1D standard of care**；**wearable CGM = T2D standard of care**（含非 insulin T2D 與孕期）。
> - **CGM-derived metrics** 將進入藥物試驗 outcomes 與 **FDA / EMA 的新藥 labeling**。
> - 期待 **noninvasive 與 long-term implantable sensors**（可同時測 glucose、ketones、其他代謝參數，持續數年）。
> - 終極願景：**fully inclusive EMR + AI** 驅動治療調整，達成 specialist 與 primary care 無縫銜接。
