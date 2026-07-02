# Ch.36 胰島素輸注硬體：從 connected pens 到 hybrid closed-loop（Insulin Delivery: Connected Pens → Pumps → SAP → LGS/PLGS → HCL）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — 本節涵蓋 Insulin delivery 總論、connected/smart insulin pens、insulin pumps (CSII)、sensor-augmented pump (SAP)、low glucose suspend (LGS)、predictive low glucose suspend (PLGS)，以及 hybrid closed-loop (HCL) 的概念與 automation 演進階梯。

---

## 💉 Insulin Delivery 總論：與 glucose monitoring 並行演進

- 過去數十年，**輸注治療劑量胰島素**的科技與 glucose monitoring 科技**並行（in parallel）**快速演進（見 Fig. 36.1）。
- 這些進展同時為**兒童與成人**胰島素治療者帶來兩大好處：
  - <u>達成血糖目標 (glycemic targets)</u>。
  - <u>改善生活品質 (quality of life)</u>。
- 演進的整體邏輯（本節主軸，務必記住這條「**自動化階梯**」）：

```
MDI / connected pen → insulin pump (CSII) → SAP → LGS → PLGS → HCL → (closed-loop)
   手動                 手動但更精準          顯示但仍手動  反應式暫停  預測式暫停  自動基礎+手動餐前  全自動
```

> 📌 **重點 (High-Yield)**：
> - Insulin delivery 與 glucose monitoring 是**兩條平行的科技軸**，最終匯流成 AID（automated insulin delivery）。
> - 自動化是**逐級遞進**：每一級都建立在前一級的硬體基礎上——pump 是後續所有進階科技的 <u>backbone</u>。

---

## 🖊️ Connected Insulin Pens（Smart Pens，智慧筆）

### 定義與基本價值

- 「**Smart**」或 **connected** insulin pens / caps（筆或筆蓋）＝**胰島素注射裝置 + 配對的 smartphone app**。
- 可搭配 **CGM** 或 **fingerstick（指尖血糖）** 讀值使用。
- 最基本價值：給「**記不得自己是否打過、打了多少胰島素**」的病人使用。

### 可預設與計算的參數（offload 計算負擔）

- 裝置可預設下列因子協助**劑量決策**，大幅減輕病人的計算負擔：
  - correction factor（校正因子）
  - target glucose（目標血糖）
  - duration of insulin action（胰島素作用時間）
  - carbohydrate ratio（碳水比值，醣類胰島素比）
- 部分裝置可用**較質性的 meal announcement**：以「**餐點大小 (meal size)**」取代精確的碳水計算 (discrete carbohydrate count)。

### 防 stacking（堆疊）→ 降低低血糖

- <u>Stacking</u>＝**短時間內、前一劑仍有作用 (active) 時又補打多劑胰島素**。
- 透過在裝置中設定 **duration of insulin action**，可估算 insulin-on-board → 減少 stacking → **降低低血糖風險**。

### 額外功能

- memory function：記錄**注射時機**，部分可記錄**注射劑量**。
- 長效胰島素施打**提醒 (reminder)**。
- temperature tracking（溫度追蹤）。
- 筆內**剩餘胰島素量**指示。

### 實證（數字忠於原文）

- **觀察性研究**：成人搭配 CGM 使用 smart pen → **TIR 增加約 2 小時/天**；同時：
  - hyperglycemia（>180 mg/dL，10.0 mmol/L）減少。
  - hypoglycemia（<70 mg/dL，3.9 mmol/L）減少。
- 兒童 real-world 觀察性研究亦有類似發現。
- 機轉推測：使用 smart pen 後**漏打 bolus（omitted boluses）變少**。
- 文獻回顧：在 **8 篇有報告偏好的研究**中，smart pen **優於**替代輸注方式（病人偏好）。
- cost-effectiveness：connected pen 可能具成本效益，因預期可**降低風險、延緩併發症發生**。

### 臨床定位

- 雖然進階科技使用增加，**許多人仍以 insulin injection 為偏好的輸注方式**。
- 2010–2018 三大國際 registry：pump 使用率上升，但 2018 年 **pump 使用頻率介於 41%–73%** 之間（仍有大量 MDI 族群）。
- 因此 smart pen 是**為 MDI 族群提供更精準胰島素治療**的有用資源：利用 dosing calculator，並依注射史與血糖型態優化劑量。

> 📌 **重點 (High-Yield)**：
> - Smart pen 的核心賣點＝**記錄 + 計算 + 防 stacking**，特別適合 <u>MDI 族群</u>（不想/不用 pump 者）。
> - 觀察性證據：成人 + CGM → **TIR ↑ 約 2 小時/天**，雙向減少高低血糖，機轉是「**少漏打 bolus**」。
> - meal size 取代 carb count 是降低使用門檻的設計（質性 vs 量化）。

---

## 🔁 Insulin Pumps（CSII，連續皮下胰島素輸注）

### 歷史與硬體優勢

- 自 **1970 年代晚期**小型研究首度證實 CSII 可改善血糖以來，pump 治療大幅演進。
- 相較 MDI，pump 能**精準輸送更小劑量**：依廠牌不同，目前可達 **0.001–0.05 units**。
- **Basal insulin profile**（取代長效 basal analogue）：
  - 預設**隨時間變動**的基礎輸注速率（units/hour）。
  - <u>temporary basal rate（暫時基礎率）</u>可即時調整：
    - **減量** → 用於敏感度上升（如**運動 exercise**）。
    - **增量** → 用於需求上升（如**生病 illness**）。

### Bolus calculator 與防 stacking

- 多數現代 pump 內建 bolus calculator，可儲存：
  - insulin-to-carbohydrate ratio（醣類比）
  - correction factor / insulin sensitivity factor（可隨時段變化）
- 可設定 duration of insulin action → 估算 **insulin-on-board** → **防 stacking** → 減少過量校正劑 → 降低低血糖。
- 輸注套件 (infusion set) 目前**每 3 天更換一次**：因此一天內多次 bolus（進食/校正）**不需逐次注射**（不同於 MDI）。
- 結論：**pump 是許多進階糖尿病科技的 backbone（骨幹）**。

### 📈 Pump 改善血糖與生活品質的實證

| 面向 | 證據重點（忠於原文） |
| --- | --- |
| HbA₁c / 血糖 | 臨床試驗 + real-world registry 均顯示 pump → 血糖改善、HbA₁c 較低 |
| 嚴重低血糖 | pump → severe hypoglycemia（需他人協助才能恢復）發生率較低 |
| DKA | trial + registry 顯示 pump 使用者 DKA 率較低 |
| DKA（丹麥研究） | pump 組 HbA₁c 較低、DKA 發生率**相似**；但**取決於樣本量**——若單一診所追蹤 **>250 名 pump 使用者**，pump 組 DKA 率較低 |
| 微血管併發症 | 青少年前瞻研究：pump 組 **peripheral nerve abnormality 與 retinopathy 率較低**，即使兩組 HbA₁c 相似（**8.7% vs 8.6%**）；已校正 socioeconomic bias 與糖尿病病程 |
| 長期效果 | 長期使用 pump 可維持血糖改善 |

#### 📊 表格解讀

- **「相似 HbA₁c 仍有微血管獲益」是高分考點**：pump 組在 HbA₁c 幾乎相同（8.7% vs 8.6%）下，神經與視網膜病變仍較少 → 暗示 pump 帶來的好處**不只反映在 HbA₁c**（如 glycemic variability、低血糖暴露減少）。該研究還**控制了社經與病程**，因果論述較強。
- **DKA 的「樣本量依賴」易混淆**：丹麥研究整體看 DKA 率「相似」，但這個結論會被**診所經驗（>250 pump 使用者）**翻轉成「pump 組較低」→ 提示**團隊熟練度/規模**影響安全性結果，不要死記「pump 一定降 DKA」。
- registry（DPV、T1DX、SWEET）＝real-world 證據來源，補足 RCT 不足，並顯示臨床上 pump 使用**逐年增加**。

### 適用族群（幾乎無禁區）

- **幼兒 (very young children)**：證實有益 → **ISPAD 建議**：若有 pump 且臨床團隊有專業，**學齡前 (preschoolers) 即可使用 pump**。
- **年長成人 (older adults)**：可成功使用。
- **病程不限**：診斷後**剛起步**即可成功導入。
- **糖尿病型別不限**：**T2D** 亦有實用性。
- **起始 HbA₁c 不限**：**起始 HbA₁c 最高者，獲益最大**。
- 總結：凡**能從強化胰島素治療獲益者**，都應考慮 pump。

> 📌 **重點 (High-Yield)**：
> - Pump 硬體三大優勢：**微量精準（0.001–0.05 U）、可變 basal profile（含 temp basal）、bolus calculator 防 stacking**。
> - ISPAD 建議**學齡前幼兒**可用 pump（前提：有裝置 + 團隊專業）。
> - 「**起始 HbA₁c 最高者獲益最大**」＋「**相似 HbA₁c 仍減少微血管病變**」＝兩個招牌考點。
> - Pump 是後續 SAP/LGS/PLGS/HCL 的 **backbone**。

### ⚠️ Pump 治療的額外考量與不良反應

- **外接裝置 (external device)**：對部分病人是「慢性病的具體提醒」→ 心理負擔。
  - **intraperitoneal pumps（腹腔內 pump）**仍在研究中，可能克服此問題。
- **Attrition（中止率）**：約 **4%–20%**。
  - **成人**：發生 severe hypoglycemia 與停用 pump 相關。
  - **青少年**：停用者多為**女性、青少年、憂鬱症狀較高**者。
- **不良事件（相當常見）**：
  - 最常見＝**pump malfunction 與/或 infusion set 失效**。
  - Teflon vs steel catheter：**7 天磨耗期 infusion set 失效率無差異**；但 **15% Teflon catheter 在置入時打折 (kinked)**，需更換。
  - 必須衛教 **ketoacidosis 風險**（infusion set 部分阻塞、移位、pump 故障）→ 需有 **sick-day plan + 24/7 廠商與醫師管道**。
- **Lipodystrophy（脂肪失養，兩型）**：

| 類型 | 定義 | 發生率 | 處置/關聯 |
| --- | --- | --- | --- |
| **Lipohypertrophy（脂肪肥厚）** | 局部脂肪堆積 | **20%–近一半** | 預防：輪替 infusion set/注射部位；偵測後避開該區待恢復 |
| **Lipoatrophy（脂肪萎縮）** | 先前部位脂肪流失 | **2%–6%**（合併多重自體免疫病者較高） | **局部類固醇注射有效** |

  - 兩者均屬 lipodystrophy，與**血糖變異度↑、HbA₁c 不佳**相關。
- **皮膚問題（黏著劑相關）**：
  - 直接檢查研究：**14%** 青少年有局部濕疹樣反應 (eczematous)。
  - 線上問卷：**89%** pump 使用者曾有皮膚問題；其中 **77% 搔癢、50% 傷口、近半數非特異性濕疹**。
  - 已有呼籲：需更了解黏著劑與 wear time 對皮膚的影響。

#### 📊 表格解讀（lipodystrophy）

- **方向相反、處置相反**：lipo**hyper**trophy（肥厚，常見）靠**輪替部位**預防；lipo**atrophy**（萎縮，較少見）用**局部類固醇**治療——別記反。
- lipoatrophy 與**多重自體免疫疾病**相關（免疫機轉色彩），lipohypertrophy 則偏局部反覆注射的機械/代謝效應。
- 兩者都會**惡化血糖變異與 HbA₁c**，所以是「技術相關但會回頭影響血糖」的雙向問題。

> 💡 **記憶法（兩型脂肪病變）**：
> - **Hyper = 多 = 多堆積 (堆肥)**，靠「**換地方 (rotate)**」解決。
> - **Atrophy = 萎縮 = 少**，靠「**打類固醇 (steroid)**」長回來。
> - 口訣：「**肥厚輪替、萎縮類固醇**」。

> 📌 **重點 (High-Yield)**：
> - Pump 最常見不良事件＝**infusion set 失效 / pump malfunction** → 衛教重點是 **DKA 預防（sick-day plan、24/7 支援）**。
> - **Teflon catheter 15% 置入時打折**是具體數字考點。
> - 停用 pump 風險族群：成人＝**severe hypo**；青少年＝**女性 + 憂鬱症狀**。

---

## 🩸 Sensor-Augmented Pump (SAP)：銜接血糖與輸注的第一步

- SAP＝**把 sensor glucose 資料**顯示於 smartphone/dedicated reader 或**直接顯示在 pump 上**。
- **關鍵限制**：治療決策**仍由使用者承擔 (onus on the user)**。
  - 例：sensor 發出高血糖警報 → **仍需病人自己動手**打 correction bolus。
- 定位：SAP **提供自動化的基礎 (foundation)**——是「**顯示但不自動**」的階段，後續整合系統建立其上。

### 實證

- **2008 第一個 RCT**（SAP vs pump）：兩組 HbA₁c 下降相似；但**對照組（pump + SMBG）低血糖暴露增加**。
  - SAP 組若 **sensor 使用 >60% 時間** → HbA₁c 下降。
- **STAR-3 study**（SAP vs MDI+SMBG，1 年，T1D、裝置初學者 device naïve）：
  - SAP → HbA₁c 下降，但**由 sensor 配戴頻率所中介 (mediated)**。
  - **青少年 cohort sensor 使用最低、達標最少**。
- real-world（162 名 T1D 轉 SAP）：**3 個月**改善血糖，**維持 2 年**。
- cost-effectiveness：SAP 優於傳統 pump（依 QALY 與臨床獲益）——但**取決於持續配戴 sensor**。

> 📌 **重點 (High-Yield)**：
> - SAP 的精神＝「**sensor 顯示資料，但人來做決定**」（仍是 open-loop）。
> - **貫穿 SAP 所有證據的主旋律＝「sensor wear 是成敗關鍵」**：2008 RCT 的 >60%、STAR-3 的中介效應、青少年使用率低達標差，全都指向「戴得夠久才有效」。

---

## ⬇️ Low Glucose Suspend (LGS)：反應式暫停

- 在能顯示血糖後，下一步＝**用 sensor 資料直接影響輸注**。
- 設計邏輯：**暫停 (suspend) 輸注比加碼 (ramp up) 輸注風險更低** → 自動化從「暫停」起步最安全。
- 機轉（Fig. 36.10A）：當 **sensor glucose 達到預設低血糖閾值**時，**暫停 basal insulin**（＝**反應式 reactive**，事件發生後才動作）。

### 實證

- **ASPIRE in-home study**（RCT，T1D，16–70 歲）：
  - real-world 使用 → **低血糖範圍的 sensor 讀值減少**。
  - **HbA₁c 無惡化**。
  - 夜間 insulin interruption → **暫停後 2 小時血糖穩定**。
- 另一 RCT（**impaired awareness of hypoglycemia 族群**）：LGS → 降低 severe（hypoglycemic seizure/coma）與 moderate（需協助治療）低血糖。
  - **對照組 6 個月內 6 次 severe hypo；LGS 組 0 次**。
- real-world（伺服器上傳資料）佐證 RCT 結果。

### ⚠️ 「sensor 讀值不準會不會導致高血糖/DKA？」的疑慮

- 核准前疑慮：若 sensor 讀**低**但實際血糖正常/偏高，暫停胰島素 → 可能高血糖甚至 DKA。
- 實驗（預設 2 小時 insulin interruption 夜 vs 正常輸注夜）：
  - interruption 後**空腹血糖約高 50 mg/dL（2.8 mmol/L）**。
  - **血 β-hydroxybutyrate 數值上略高，但未達統計顯著、也無臨床顯著意義**。
  - 結論：**「sensor 不準導致 interruption」的擔憂被排除 (allayed)**。
- cost-effective 族群：高低血糖風險、disabling/impaired awareness hypoglycemia、fear of hypoglycemia 者。

> 📌 **重點 (High-Yield)**：
> - LGS ＝**reactive（事件發生後）暫停 basal**；自動化從「暫停」起步是因為**暫停最安全**。
> - 招牌數字：impaired awareness 族群 RCT，**對照組 6 次 vs LGS 組 0 次 severe hypo**。
> - 「2 小時暫停只讓空腹血糖高約 50 mg/dL、酮體無顯著差異」→ **安全性疑慮被消除**，是核准的關鍵論述。

---

## ⏬ Predictive Low Glucose Suspend (PLGS)：預測式暫停

- 從**反應式 (reactive)** → **主動式 (proactive)**：在**事件發生前**就中斷輸注以**預防低血糖**（Fig. 36.10B）。
- 早期研究：演算法放在床邊**筆電**上執行，證實此法可行。

### 安全性（酮症）議題

- 早期研究比較 PLGS 組 vs SAP 對照組**晨間酮症 (ketosis) 率** → **無差異**。
- 兒科研究：**4–9 歲**晨間酮症次數 > **10–14 歲**。
- 但更早研究顯示：**不論輸注方式**，幼童 ketonemia（>0.2 mmol/L）本就比青少年多（**4–7 歲 vs 14–19 歲**），且多見於**空腹期**。
- 解讀：幼童酮症較多**反映年齡生理差異，而非輸注方式** → **PLGS 不需強制驗酮**，只需比照一般 pump 使用者（持續性高血糖或生病時驗酮）。

### 兩種 PLGS 系統（不同演算法/sensor）— 核心比較

| 參數 | **系統 A** | **系統 B** |
| --- | --- | --- |
| 觸發暫停條件 | 預測 **30 分鐘內**血糖將達「**使用者設定低限 + 20 mg/dL（1.1 mmol/L）**」 | 預測 **30 分鐘內**血糖將低於**固定閾值 80 mg/dL（4.4 mmol/L）**，或 sensor 讀值 **<70 mg/dL（3.9 mmol/L）** |
| 最短暫停 | **30 分鐘** | **5 分鐘** |
| 最長暫停 | **120 分鐘（2 小時）** | **2 小時** |
| 恢復輸注 | 低血糖恢復後恢復（在 30–120 分鐘區間） | sensor 值**偵測到回升即恢復** |

#### 📊 表格解讀（兩種 PLGS）

- **觸發邏輯不同**：系統 A 是「**相對於使用者低限 + 20 mg/dL**」（個人化、浮動）；系統 B 是「**固定 80 mg/dL 閾值**或 <70 即停」（絕對閾值）。考試易混淆——記住 **A = 浮動、B = 固定**。
- **最短暫停差很多**：A 最短 **30 分鐘**（停就停較久），B 最短 **5 分鐘**（更靈活、見回升即放行）→ B 設計上更傾向「**最小化暫停時間以減少反彈高血糖**」。
- 兩者最長暫停都是 **2 小時**。

### 各系統實證

- **系統 A**：
  - 14–75 歲：夜間以增加 basal 誘發低血糖 → **多數情況成功避免低血糖**。
  - 兒童（以運動誘發低血糖）：**80% 成功預防低血糖**。
  - 2 個 RCT 均顯示低血糖減少；但其中一研究 PLGS **伴隨 >140 mg/dL（7.8 mmol/L）時間上升**（換取代價）。
- **系統 B（PROLOG RCT，6 週）**：相較 SAP 對照組，**<70 mg/dL（3.9 mmol/L）時間減少 31%**。

### 整體證據與生活面

- real-world 觀察資料支持 RCT 結果。
- 轉 PLGS → **裝置滿意度上升、糖尿病對生活影響下降**（成人 T1D 與未成年照顧者皆然）。
- 橫斷面分析：兩種 PLGS 系統導入臨床皆有益。
- meta-analysis（夜間使用）：低血糖風險**降低 8.8%**。
- meta-analysis（5 個 RCT）：**PLGS 優於 SAP**。
- **治療低血糖的碳水量需減少**：近期 PLGS 試驗中位數**僅需 9.9 克碳水**即可處理低血糖事件。

> 📌 **記憶法**：PLGS 是「**先知 (Predict)**」——在血糖**還沒掉到**閾值前就先暫停；LGS 是「**消防員 (React)**」——失火（已低）才出動。

> 📌 **重點 (High-Yield)**：
> - PLGS = **proactive/predictive**（事前），LGS = **reactive**（事後）。
> - **PLGS 不需強制驗酮**：幼童晨間酮症較多是**年齡生理**而非輸注方式所致。
> - 招牌數字：**PROLOG（系統 B）→ <70 mg/dL 時間 ↓31%**；meta-analysis **PLGS 優於 SAP**、夜間低血糖風險 ↓8.8%。
> - PLGS 暫停後**治療低血糖只需約 9.9 g 碳水**（傳統 15 g rule 需下修）。
> - 代價：某些 PLGS 研究見 **>140 mg/dL 時間上升**（防低血糖換來輕微高血糖）。

---

## 🤖 Hybrid Closed-Loop (HCL)：概念

- 機轉（Fig. 36.10C）：**sensor glucose → 演算法 → 透過 pump 調整輸注**，但**餐前 bolus 仍需病人手動輸入 (mealtime bolus input)**。
- 「**Hybrid（混成）**」一詞的由來：
  - **自動 (automated)** 的部分＝**basal**（演算法自動調整，Fig. 36.10C 中 automated basal 在 **min 0 ~ max 0.2 units** 間浮動）。
  - **手動 (manual)** 的部分＝**meal/餐前 bolus**（仍靠人）。
- 與前幾級的本質差異：
  - LGS/PLGS **只會「暫停」**輸注（單向，往下調）。
  - HCL **會主動「增減」basal**（雙向自動調控）→ 是真正的 closed-loop 雛形（但非全自動）。

### 🪜 自動化階梯總比較（核心考點：SAP → LGS → PLGS → HCL）

| 系統 | 對 sensor 資料的反應 | basal 動作 | 觸發/邏輯 | 仍需手動 | 性質 |
| --- | --- | --- | --- | --- | --- |
| **SAP** | 僅**顯示** | 無自動調整 | 高血糖警報需人處理 | basal、bolus、所有校正 | open-loop（顯示） |
| **LGS** | 影響輸注 | **暫停 basal** | 血糖**已達**低閾值（reactive 反應式） | 餐前 bolus、校正 | 單向（往下，事後） |
| **PLGS** | 影響輸注 | **暫停 basal** | **預測**短時間內將低（proactive 預測式） | 餐前 bolus、校正 | 單向（往下，事前） |
| **HCL** | 演算法調控 | **自動增/減 basal**（雙向） | 演算法持續調整 | **餐前 bolus（必須手動）** | hybrid closed-loop |

#### 📊 表格解讀（自動化階梯）

- **遞進主軸＝「自動化的程度」**：SAP（看）→ LGS（已低就停）→ PLGS（快低就停）→ HCL（自動上下調 basal）。
- **LGS vs PLGS 的唯一關鍵差異＝時機 (timing)**：reactive（事件後）vs proactive（預測、事件前）；**兩者都只「暫停」、都不「增加」basal**。
- **PLGS vs HCL 的關鍵差異＝方向性 (directionality)**：PLGS 只能往下（暫停）；**HCL 能雙向自動調 basal**——這是跨入 closed-loop 的分水嶺。
- **HCL 仍是「hybrid」而非全自動**：因為 **meal bolus 仍要人按**——這是最常被考的「為什麼叫 hybrid」。

> 💡 **記憶口訣（自動化階梯）**：
> 「**看 → 停（已低）→ 早停（快低）→ 自動調**」
> 對應 **SAP → LGS → PLGS → HCL**。
> 再加一句：「**LGS/PLGS 只會踩煞車（暫停），HCL 才會踩油門也踩煞車（增減 basal）；但 HCL 連方向盤的『吃飯那一下（meal bolus）』還是要人握。**」

> 📌 **重點 (High-Yield)**：
> - **HCL ＝ 自動 basal + 手動 meal bolus**（所以叫 hybrid，非 fully closed-loop）。
> - **LGS 與 PLGS 都只能「暫停 basal」（單向）**；HCL 是**第一個能雙向自動增減 basal** 的層級。
> - 區辨三句話：LGS = **已低才停**；PLGS = **快低就先停**；HCL = **自動調 basal、餐前仍手動**。
> - Fig. 36.10 三張圖（A=LGS、B=PLGS、C=HCL）是本章自動化演進的視覺骨幹，務必記得對應關係。
