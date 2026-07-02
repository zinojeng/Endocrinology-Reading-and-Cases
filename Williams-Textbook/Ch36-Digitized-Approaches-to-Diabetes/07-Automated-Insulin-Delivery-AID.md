# Ch.36 自動胰島素輸注 AID：證據、特殊情境與可近性（Automated Insulin Delivery）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — Automated Insulin Delivery（AID 的演算法分類、支持證據、特殊情境管理、open-source DIY 系統與 access 議題）

---

## 🤖 AID 的基本概念與系統組成

Automated insulin delivery (AID) 系統，又稱 <u>closed loop (CL)</u> 或 <u>artificial pancreas (AP)</u> 系統，是目前 insulin 治療**最成功的模式**。它不只像 PLGS 那樣「暫停 insulin 來預防 hypoglycemia」，更能**主動加碼 insulin** 來縮短 hyperglycemia 的時間（即雙向調節）。

**三大基本組件（缺一不可）：**
- <u>glucose sensor</u>（CGM）：持續提供 sensor glucose 資料
- <u>algorithm（演算法）</u>：AID 系統的「大腦 (brain)」，決定要輸注多少 insulin
- <u>insulin pump</u>：實際執行 insulin 輸注

**演算法 = AID 的靈魂**，目前主要有三大類：

| 演算法 | 機轉特性 | 核心邏輯 |
|---|---|---|
| **Model predictive control (MPC)** | 預測式 (predictive) | 使用個人化參數，在預先設定的 **time horizon** 內，**最小化** model 預測 glucose 與 target glucose 之間的差距 |
| **Proportional integral derivative (PID)** | 反應式 (reactive) | 加總三部分：與 target 的差值（**proportional**）＋ 量測與 target 之間的曲線下面積（**integral**）＋ glucose 變化率（**derivative**） |
| **Fuzzy logic controller** | 模仿臨床醫師推理 | 仿照 diabetes practitioner 的思路，納入常識性醫學知識、已知建議與臨床經驗來調節 insulin |

**兩種 target 策略：**
- <u>Treat-to-target</u>：設定**單一** glucose target
- <u>Treat-to-range</u>：設定**上下限 (lower and upper bounds)**，演算法在此範圍內調整劑量

📊 **表格解讀（演算法分類）**
- **MPC 是「預測式」、PID 是「反應式」**——這是最常考的對立點。MPC 往前看（predict 並 minimize 誤差），PID 往後看（根據已發生的偏差 P/I/D 三項加總反應）。
- PID 的三個英文字母對應三個數學項：P＝瞬時偏差、I＝累積偏差（AUC）、D＝變化趨勢，記住「P/I/D = 現在/過去累積/趨勢」。
- Fuzzy logic 的精神是「把醫師的經驗法則寫成規則」，較不依賴嚴格數學模型。
- Treat-to-target vs treat-to-range：前者一個點、後者一個帶狀區間，臨床上 range 策略給演算法較大彈性。

> 📌 **重點 (High-Yield)**：
> - AID＝sensor＋algorithm＋pump，**雙向調節**（既能暫停又能加碼），優於只會暫停的 PLGS。
> - 演算法是「大腦」：**MPC（預測式）vs PID（反應式）vs fuzzy logic（模仿醫師）**。
> - PID 三項：proportional（與 target 差值）、integral（AUC）、derivative（變化率）。

---

## 🔁 從 Full Closed Loop 到 Hybrid（混合型）的演進

- **早期研究**採用 <u>fully automated（full closed loop）</u>，完全由系統決定所有 insulin。
- 問題：full closed loop 會造成**明顯的餐後血糖飆升 (postprandial glycemic excursions)**。
- 解決：改採 <u>hybrid（混合型）</u>——**餐前 prandial insulin 仍由使用者輸入**，其餘由演算法調節。
- 目前仍持續努力朝 **fully AID** 邁進，策略包括：
  - 使用**更快速作用的 insulin analogues (faster-acting insulin analogues)**
  - 加上 **adjunctive to insulin therapies（輔助治療）**（本章後段討論）

**術語更新（consensus 建議）：**
- 傳統把 pump 劑量分為 **basal / bolus**，但在更先進的輸注方式下此分類已不再恰當。
- 新共識指引建議改用：
  - <u>User-initiated insulin delivery</u>（使用者啟動）
  - <u>Algorithm-modulated insulin delivery</u>（演算法調節）

> 📌 **重點 (High-Yield)**：
> - Full closed loop 的致命傷是**餐後血糖飆升** → 因此演變為 **hybrid（使用者仍需手動輸入餐前 insulin）**。
> - 邁向 fully AID 的兩大途徑：**faster-acting insulin analogues** ＋ **adjunctive therapies**。
> - 新術語：**user-initiated vs algorithm-modulated**，取代舊的 basal/bolus。

---

## 📊 支持 AID 的證據（The Evidence）

過去數年 AID 試驗的資料量**呈指數成長 (exponentially grown)**，據此一個國際共識小組已撰寫 AID 系統的臨床實務指引。

**RCT 與單臂研究 (single-arm studies) 的一致發現：**
- **從幼兒 (toddlers) 到老年族群 (geriatric population)**，AID 系統**一致地**提升 <u>%TIR</u>（70–180 mg/dL，3.9–10.0 mmol/L）。
- TIR 上升的同時伴隨：
  - mean glucose 下降
  - time in hyperglycemia 下降
  - HbA₁c 下降
  - time in hypoglycemia **不變或下降**（不會惡化低血糖）

**具體數據：**

| 比較項目 | TIR 改善幅度 | 換算每日時間 |
|---|---|---|
| AID vs 傳統 pump / SAP / PLGS / 第一代 AID（RCT） | **10%–15%** | **每天多 2.0–3.5 小時** in range |
| AID vs 啟用前 baseline（single-arm） | 類似改善 | — |

📊 **表格解讀（療效數據）**
- **10%–15% TIR ≈ 每天多 2.0–3.5 小時** 在目標範圍——這是必背的換算（TIR 1%≈14.4 分鐘）。
- 對照組涵蓋廣：傳統 pump、SAP（sensor-augmented pump）、PLGS、甚至第一代 AID，AID 都更優，顯示新一代系統的進步。
- Single-arm 研究（與自身 baseline 比）也得到相似 TIR 改善，**證據一致性高**。
- 注意：低血糖時間「不變或下降」，代表 AID 能**同時改善高血糖與不增加低血糖**，打破傳統「降 HbA₁c 必增低血糖」的取捨。

**臨床脈絡——TIR 與併發症的連結 (DCCT post hoc analysis)：**
- DCCT 資料 post hoc 分析顯示：**每降低 10% time in target range**，與下列風險增加相關：
  - retinopathy progression：hazard rate **64%**
  - microalbuminuria 發生：hazard rate **40%**
- ⚠️ 注意限制：此分析只能用**白天 7-point SMBG** 來計算 TIR，故**可能低估**真正的差異。

> 📌 **重點 (High-Yield)**：
> - AID 在**所有年齡層**一致提升 TIR：RCT 顯示 **+10%–15%（每天多 2–3.5 小時）**。
> - 「降高血糖、不增低血糖」是 AID 最大賣點。
> - DCCT post hoc：**TIR 每低 10%**，retinopathy progression HR **64%**、microalbuminuria HR **40%**（但因僅用白天 7-point SMBG，可能**低估**）。

---

## 🏥 從 Real-World 資料看 AID（含 system-mandated exits 問題）

**整合進臨床照護的時間軸：**
- 此技術**首次整合進臨床照護是 2017 年**（第一個商業核准的 AID 系統）。

**第一代系統的痛點—— system-mandated exits（系統強制退出）：**
- 觸發強制退出的情境：
  - sensor 未以 fingerstick glucose 校正
  - insulin delivery 達到預設的**最大輸注時段**
  - 反之，insulin 暫停**過久**
- 後果：
  - 早期單中心報告**約 30% 使用者流失 (attrition)**，多歸因於對強制退出的挫折感。
  - 一份 80 名使用者的前瞻真實世界調查（**30% 為 18 歲以下**）：雖肯定有獲得適當訓練，但**超過一半因 alarms 而睡眠中斷**，且 **40% 認為強制退出頻率是個問題**。
- 改善方向：**factory-calibrated sensors**（工廠校正，免 fingerstick）＋ 減少 system-mandated exits → 新一代系統**增加 time in automation**、降低負擔，提升配戴與持續使用率。

**Real-world 大型資料（為何重要）：**
- RCT 收案者通常**無法反映真實多元的糖尿病族群**，且 protocol 規定的聯繫頻率在臨床難以複製。

| Real-world 分析 | 樣本數 | 關鍵結果 |
|---|---|---|
| 某 AID 系統中央伺服器分析 | **9451** 名（**17% 為 T2D**） | median time in automation **94%**；median TIR 由 baseline **63.6%** → 12 個月 **73.6%**（與該技術 RCT 結果吻合） |
| 另一 AID 系統雲端上傳（early adopters） | **4120** 名 | 中位配戴 2 個月後 mean GMI **6.8%**、TIR **76%** |
| 依年齡分層分析 | ≤15 歲 **n=3211** vs >15 歲 **n=8874** | **兩組皆有 75% 的人**達共識指引 TIR **>70%** 的目標 |

📊 **表格解讀（real-world 證據）**
- 9451 人分析的 **94% time in automation** 說明新系統「黏著度」高；TIR 63.6→73.6% **與 RCT 吻合**，代表 RCT 結果可外推到真實世界。
- 4120 人 early adopters 僅 2 個月就達 **GMI 6.8%、TIR 76%**，顯示上手快、效果迅速。
- 年齡分層分析證明**兒童與成人都能達標**（各 75% 達 TIR>70%），破除「小孩做不到」的迷思。
- 趨勢：下一代 AID 的臨床試驗將更能準確預測真實世界的使用經驗。

> 📌 **重點 (High-Yield)**：
> - AID 臨床整合**始於 2017**；第一代痛點＝**system-mandated exits**（約 **30% attrition**、alarms 致睡眠中斷、40% 覺得強制退出煩人）。
> - 解方＝**factory-calibrated sensor ＋ 減少強制退出 → 增加 time in automation**。
> - Real-world：9451 人 time in automation **94%**、TIR 63.6→73.6%；分齡分析兩組皆 **75% 達 TIR>70%**。

---

## 🩸 AID 的特殊情境管理（Special Situations）

### 🤒 病日管理 (Sick-day management)
- 與任何 insulin pump 一樣：**規律檢查 ketones**、**更換 infusion set**。
- ⚠️ 關鍵觀念：AID 由 **sensor glucose 驅動**，而 ketosis 代表 insulin 不足 → 若出現 ketosis，**建議退出 automation、回到 open loop**。
- 退出後可：
  - 給予 **correction dose**
  - 利用 **temporary basal rates** 加碼（例如 **200% basal rate ＝ 比平常多 +100%**），**不受當下 glucose 限制**。
- Ketosis 緩解後可恢復 automation，但**不能早於演算法設定的 insulin duration of action（即 2–4 小時）**，以避免**algorithmic 與 user-initiated insulin 疊加 (stacking)**。

### 💊 類固醇治療 (Steroids)
- 是否維持 automation **取決於所用系統**。
- 部分系統可允許**更積極的 insulin 輸注**：
  - 可設定多種 **alternate insulin profiles**
  - 特定 **"boost" mode** 讓使用者**暫時增加**輸注
- 指引需個別化：依**個人、所用系統、類固醇的效價與劑量**而定。

### 🔪 小手術前 (Minor procedures)
- AID 在術前**非常有幫助**——glucose-driven 輸注可提高處於可接受範圍的機率。
- 若擔心 hypoglycemia，可使用：
  - **temporary glucose target（暫時拉高目標）**
  - **exercise / activity mode**
  - 兩者皆能**降低 insulin on board (IOB)**、減少低血糖風險。

💡 **記憶法（特殊情境三大策略）**：
- 「**酮體往上、低血糖往下**」——有 ketosis 要**退出 automation 並加碼**（200% basal）；怕低血糖則用 **activity mode / 暫時拉高目標** 來**減 IOB**。
- 恢復 automation 的時機 = **等一個 insulin duration of action（2–4 小時）**，避免 stacking。

> 📌 **重點 (High-Yield)**：
> - **Sick day + ketosis → 退出 automation、open loop、correction dose、temp basal（如 200%＝+100%）**；恢復需等 **2–4 小時（insulin DOA）防 stacking**。
> - **Steroids → 視系統而定**，可用 alternate profiles 或 **boost mode** 加碼。
> - **小手術前 → AID 有利**；怕低血糖用 **temp target / activity mode** 降 IOB。

---

## 🛠️ Open-Source AID（DIY 系統）的洞見

**背景與動機：**
- 一群糖尿病患者與家屬意識到**臨床試驗與法規核准的延遲 (inherent delays)**，決定自己動手。
- <u>Do-it-yourself (DIY)</u> 路線：線上 tech-savvy 的糖尿病社群在商業產品核准**之前**，就自行開發出**遠端監測 glucose 並調整 insulin 輸注**的方法。

**療效證據：**

| 研究設計 | 樣本 | 結果 |
|---|---|---|
| 前瞻觀察性試驗 (real-world prospective observational) | **>550** 名使用者 | DIY AID **提升 %TIR**、**降低嚴重低血糖事件** → 可安全有效使用 |
| RCT（open-source AID vs 僅用 CGM 對照組） | — | DIY 組 TIR **增加 10%**，組間差 **14%（>3 小時/天）** |

**安全性 / 中止率：**
- RCT 中 AID 組因 **connectivity issues** 中止者約 **5%**；觀察性研究中止比例相近。

**指引立場（重要！）：**
- ⚠️ DIY 裝置**未取得法規核准**，HCP 推薦時應**謹慎**。
- ✅ 但共識指引強調：**當病人選擇使用 DIY AID 系統時，提供者應給予支持 (support them)**。

📊 **表格解讀（DIY 證據）**
- >550 人觀察性與 RCT 雙重證據都顯示 DIY「**升 TIR、降嚴重低血糖**」，效果不輸商用系統（TIR +10%，組間差 14%）。
- 主要失敗原因是**連線問題（connectivity）**而非血糖控制不佳，約 5%。
- 考點：指引態度是「**不主動推薦、但若病人已選擇則支持**」——這種「謹慎但支持」的立場常被考。

> 📌 **重點 (High-Yield)**：
> - DIY/open-source AID 證據（>550 人觀察 ＋ RCT）：**升 %TIR、降 severe hypoglycemia**；RCT TIR **+10%、組間差 14%（>3 小時/天）**。
> - 中止主因＝**connectivity issues（約 5%）**。
> - 指引立場：**未核准 → 謹慎；但病人選用 → 應支持**。

---

## 🌍 AID 的可近性（Access for All）

**過去的問題——選擇偏誤 (selection bias)：**
- 科技裝置的取得常被**對「理想候選人」的偏誤**所阻礙。
- 一份 192 名 providers 的調查顯示：判定誰「適合 pump」的標準很**主觀**，考量因素包括：
  - fingerstick 檢測頻率
  - 每年回診次數
  - 是否達 target HbA₁c
  - 確診糖尿病的時間長短
- 這類主觀標準可能正好**對應到已被報導的裝置取得差距 (disparities)**。

**新證據翻轉舊觀念：**
- RCT 與真實世界觀察資料皆顯示：<u>baseline HbA₁c / GMI 最高</u>的人，反而獲得**最大的改善**：
  - time above range 降幅最大
  - GMI 降幅最大
  - time in target range 增幅最大
- ⭐ 結論：**「控制差」不該是排除標準，反而是最該用 AID 的族群**。

**指引與證據的共同方向：**
- 臨床醫師應**廣泛地考慮對所有糖尿病患者使用 AID**。
- 此立場獲多個學會共識指引支持，並有近期 RCT 的彙整資料佐證：**更多 automation → 更高 %TIR**（Fig. 36.11）。

💡 **比較表（Access 的舊觀念 vs 新證據）**

| 面向 | 舊觀念（selection bias） | 新證據 |
|---|---|---|
| 誰適合 AID/pump | 自我管理好、HbA₁c 已達標、常回診者 | **所有需要 insulin 的人**都該考慮 |
| 高 baseline HbA₁c 者 | 被視為「不適合」 | **獲益最大**（TAR↓、GMI↓、TIR↑ 幅度最大） |
| 判定標準 | 主觀、易造成 disparities | 應**廣泛納入**，破除差距 |

> 📌 **重點 (High-Yield)**：
> - 過去 access 受 **selection bias** 限制（192 providers 調查標準主觀）→ 造成 device 取得 **disparities**。
> - 翻轉觀念：**baseline HbA₁c/GMI 最高者 AID 獲益最大** → 不該被排除。
> - 指引一致：**對所有需 insulin 者廣泛考慮 AID**；**更多 automation = 更高 TIR**（Fig. 36.11）。

---

## ⭐ 全節總整理（One-Page Recap）

- **AID＝sensor＋algorithm（大腦）＋pump**，雙向調節，是目前最成功的 insulin 治療模式。
- 演算法：**MPC（預測）/ PID（反應，P+I+D）/ fuzzy logic（仿醫師）**；目標策略 treat-to-target vs treat-to-range。
- Full closed loop **餐後血糖飆升** → 演變成 **hybrid**（餐前手動）；新術語 **user-initiated vs algorithm-modulated**。
- 證據：全年齡層 TIR **+10–15%（每天多 2–3.5 小時）**，降高血糖不增低血糖；DCCT 連結 TIR↓10% → retinopathy HR 64%、microalbuminuria HR 40%。
- Real-world：自 2017 整合臨床；第一代痛點 **system-mandated exits**（30% attrition）→ 新一代 factory-calibrated、time in automation 94%。
- 特殊情境：**ketosis 退出加碼、steroids 視系統 boost、術前用 activity mode 降 IOB**。
- DIY/open-source：升 TIR 降 severe hypo，**未核准但病人選用應支持**。
- Access：**baseline 越差獲益越大 → 對所有人廣泛考慮 AID**。
