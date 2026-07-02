# Ch.36 決策支援系統、mHealth apps 與 AGP 報告判讀（Decision-Support, mHealth & AGP）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — 決策支援平台 (decision-support systems)、AI advisers、caregiver support、diabetes smartphone apps，以及 ambulatory glucose profile (AGP) 報告的解剖與系統性判讀步驟

---

## 🖥️ 一、決策支援系統：CGM 資料的視覺化與「超越視覺化」

對於使用 continuous glucose monitoring (CGM) 的糖尿病病人（無論是 standalone CGM 或屬於 automated insulin delivery (AID) 系統的一部分），**主動式管理 (proactive management)** 都需要一個 <u>資料管理平台 (data-management platform)</u>。

- 這些平台可以是：
  - **system-specific**：僅綁定單一 CGM 廠商產品。
  - **inclusive**：可整合多個 CGM 系統送來的 glucose data。
- 共同特性：
  - 全部是 <u>cloud-based</u>，可透過 web 存取。
  - 設計目的：支援 <u>shared decision making（共享決策）</u> 與治療調整。
  - 存取方式：病人或醫療團隊以 **secure log-in** 登入，並確保 data confidentiality and security。
  - 提供使用者所選期間（current 或 historical）的 glycemic status 視覺摘要。
  - 各家有 proprietary features，但**多數平台共通**提供：
    - <u>time in range (TIR) performance「bars」</u>（如 Fig. 36.8）。
    - <u>ambulatory glucose profile (AGP)</u>（Fig. 36.9）。
- 臨床應用亮點：
  - **可在排定的回診之間遠端存取 (accessed remotely between scheduled follow-up appointments)**。
  - 讓醫療人員即時檢視病人對治療調整的反應，或朝目標 (goals) 的進展。

### 💡 從「視覺化」到「AI advisers」：新興的演算法決策支援

- 新興領域：decision-support systems 能整合 **connected care devices** 的資料：
  - CGM、smart insulin pens、SMBG、insulin pumps。
- 透過 **smart apps 或 cloud-based algorithms** 產生有意義的 guidance 與 advice。
- 功能涵蓋：
  - 協助 **multiple daily injections (MDIs)** 或 pump therapy 病人做 <u>dose titration（劑量滴定）</u>。
  - 提供 dose optimization 與 behavioral modification 建議。
  - 給臨床團隊增強的 visualization 與 insulin management 建議。
- ⭐ **關鍵證據**：一項 RCT 比較「physician-guided dose alterations」與「decision-support tool 建議的劑量調整」，結果顯示演算法達 <u>noninferiority（非劣性）</u>，因而獲得該裝置的 **regulatory approval（法規核准）**。
- 其他 decision-support tools 仍在開發中。

> 📌 **重點 (High-Yield)**：
> - 決策支援平台的三大共通本質：**cloud-based、secure log-in、shared decision making**。
> - 幾乎所有平台都提供兩種共通報告：**TIR bars + AGP**。
> - 平台可在回診之間**遠端**檢視，是 telemonitoring 的具體應用。
> - AI/演算法 dose-titration 工具已有 **RCT 證明 noninferiority 並獲法規核准**——這是考點等級的里程碑。

---

## 📊 二、Table 36.4 — 用於存取與檢視 CGM glucometric data 的決策支援系統

> 此表列出臨床常用、也是 type 1 diabetes (T1D) 臨床研究中最常使用的平台；尚有其他平台存在（非窮舉）。

| Platform | SMBG Meters | CGM | Insulin Pumps | Smart Pens | Supports Multiple Brands |
| --- | :---: | :---: | :---: | :---: | :---: |
| **Glooko** | Yes | Yes | Yes | Yes | **Yes** |
| **Tidepool** | Yes | Yes | Yes | Yes | **Yes** |
| **Abbott LibreView** | Yes | Yes | No | Yes | No |
| **Medtronic Carelink** | Yes | No | Yes | No | No |
| **Dexcom Clarity** | No | Yes | No | No | No |
| **Tandem t:connect** | No | No | Yes | No | No |

*CGM, continuous glucose monitoring; SMBG, self-monitoring of blood glucose.*

### 📊 表格解讀

- **欄位含義**：
  - **SMBG Meters / CGM / Insulin Pumps / Smart Pens**：該平台是否能匯入並顯示對應裝置的資料。
  - **Supports Multiple Brands**：是否支援**跨多家廠牌**的裝置資料整合（agnostic platform）。
- **臨床意涵**：
  - <u>Glooko 與 Tidepool 是「全才型」平台</u>：四類裝置全支援、且 **multiple brands = Yes**。這代表它們是 **vendor-agnostic（不綁特定廠商）**，最適合裝置組合複雜或混用多廠牌的病人/診所。
  - <u>廠商專屬平台（vendor-specific）只支援自家生態系</u>：
    - **Abbott LibreView**：支援 SMBG、CGM、Smart Pens，但**不支援 insulin pumps**，且 multiple brands = No。
    - **Medtronic Carelink**：支援 SMBG 與 pumps，**不支援 CGM 欄位（標 No）**、不支援 smart pens。
    - **Dexcom Clarity**：**只支援 CGM**（純 CGM 報告平台）。
    - **Tandem t:connect**：**只支援 insulin pumps**。
- **易混淆點 / 考點**：
  - 「能整合多廠牌」的只有 **Glooko 與 Tidepool 兩家**——這是最容易被問的記憶點。
  - Carelink 在 CGM 欄位標 **No**，容易被誤以為支援；它的定位是 pump 廠商（Medtronic）的平台。
  - LibreView 不支援 pumps；Dexcom Clarity 不支援 pumps 也不支援 SMBG——反映各自的產品線。

### 💡 記憶法 / 比較表

- 口訣：**「Glooko、Tidepool 通吃，其餘只顧自家門」**——只有這兩家 multiple brands = Yes。
- **平台屬性比較表**：

| 屬性 | Vendor-agnostic（跨廠牌） | Vendor-specific（廠商專屬） |
| --- | --- | --- |
| 代表平台 | Glooko、Tidepool | LibreView、Carelink、Clarity、t:connect |
| 裝置支援 | 四類 (SMBG/CGM/pump/pen) 多為全包 | 僅綁自家產品線 |
| Multiple brands | Yes | No |
| 適用情境 | 混用多廠牌、診所統一檢視 | 病人/診所單一廠牌生態系 |

> 📌 **重點 (High-Yield)**：
> - **Glooko + Tidepool = 唯二支援 multiple brands 的全才型平台。**
> - Dexcom **Clarity** = 純 CGM；Tandem **t:connect** = 純 pump；Medtronic **Carelink** CGM 欄位是 **No**。
> - Abbott **LibreView** 支援 CGM/SMBG/pen 但**不支援 pump**。

---

## 👨‍👩‍👧 三、為 caregivers 提供支援（Caregiver Support / Follow apps）

- 部分可下載的 apps 允許使用者**邀請家人與照護者 (caregivers)** 一同存取其 glucose data。
- 功能：
  - 照護者可在**自己的 smartphone** 上**遠端**監看病人的 continuous glucose readings。
  - 可接收 **high / low glucose 的 alerts**。
- 臨床價值：
  - 對父母與照護者而言是 invaluable tools，即使無法陪在身邊也能獲得 **reassurance（安心感）** 與 glucose feedback。
- ⚠️ **使用關鍵 / 注意事項**：
  - 必須**事先設定清楚的期待 (clear expectations)**：跟蹤資料的人**會如何反應 alerts 與 alarms**。
  - 在 **adolescence（青春期）** 尤其重要——青少年在爭取 **autonomy（自主性）** 的階段，過度監看與警報反應可能造成衝突。

> 📌 **重點 (High-Yield)**：
> - Follow/caregiver app 讓照護者遠端接收 high/low alerts，提供 reassurance。
> - **青少年自主性 (autonomy)** 是必考的情境衝突點——需事先約定誰看資料、如何回應警報。

---

## 📱 四、Mobile Health (mHealth) 與糖尿病 smartphone apps 的興起

### 🔢 市場概況（November 2022 搜尋數據，忠於原文）

- 在 Google Play 與 Apple App Store 搜尋（2022 年 11 月）共找到 **85 個 diabetes mHealth apps**：
  - 多數由 diabetes technology 公司提供，協助使用其專屬 **SMBG meters、CGM systems、insulin pumps** 的病人。
  - 這些「device-manufacturer apps」已通過 **regulatory assessment**，確保 system accuracy 與 data privacy 合規。
- 另有 **56 個來自 independent providers**，聚焦於糖尿病健康與日常管理：
  - 最常見功能：**blood-sugar diaries（血糖日記）** 或 **healthy eating / meal planning（健康飲食/餐食規劃）**，偶爾兩者兼具。
  - 較少見：聚焦於 physical activity 或 diabetes communities 的 apps。

### 📦 Box 36.1 — Digital Health 重要定義（用 diabetes technology 舉例）

| 名詞 | 定義要點 | Diabetes 範例 |
| --- | --- | --- |
| **Telemedicine** | 以科技在**遠距**提供醫療；可 synchronous 或 asynchronous。涵蓋 telemonitoring、tele-expertise、tele-assistance、televisit、teleconsultation、tele-education | — |
| **Telemonitoring** | 以資通訊技術在地理上分隔的人之間**監測、傳輸、分享**病人健康狀態資訊 | **用 CGM 系統監測 glycemic metrics 即為 telemonitoring 範例** |
| **mHealth** | eHealth 的子分支，以 **mobile devices** 直接支援醫療與公衛實務，含 mobile health applications | **讀取/回報 glucose-sensor data 的 smartphone apps** |

#### 📊 表格解讀

- **層級關係**：mHealth ⊂ eHealth；telemonitoring 是 telemedicine 的一種應用範疇。
- **臨床意涵**：CGM 是 **telemonitoring 的典型範例**；CGM 讀數的 smartphone app 是 **mHealth 的典型範例**——同一個 CGM 生態系同時體現兩個概念。
- **易混淆點**：Telemedicine 強調「遠距提供醫療」，可同步或非同步；Telemonitoring 強調「監測+傳輸+分享資料」。考試常以「CGM 屬於哪一類」設題，答案取向 **telemonitoring / mHealth**。

### 📲 採用態度與證據

- **青少年 T1D**：對 mHealth apps 接受度高，包括聚焦 nutrition、physical activity、glucose logging/monitoring、insulin bolusing、insulin delivery 的 apps。
- **2022 年調查**（310 位 T1D 青少年與成人）：**80% 受訪者願意分享 real-time glucose data** 以換取量身定制的支援（含 text messaging 與 email）。
- **T2D**：同樣支持 mHealth，符合其對 **independence 與 convenience** 的偏好；接受含提醒與強化訊息的 text messages。

### ⚖️ 法規、品質保證與 digiceuticals

- ⚠️ **核心隱憂**：mHealth 開發的品質保證——資訊的 **accuracy 與 safety** 監管不足。
- **FDA**：設有核准軟體 apps 的 registration and listing database（含 diabetes）；但出版時**僅列出由 diabetes hardware 廠商提供的 apps**。
- **歐洲 CE mark**：少數 apps 取得，但**並非必要要求**。
- **Digiceuticals（數位處方藥）**：
  - 在美國開始被應用的概念。
  - 定義：**經臨床驗證 (clinically validated)** 的 mHealth apps，**只能在 physician prescription（醫師處方）後取得**，包含 diabetes-specific apps。
- **EASD + ADA Diabetes Technology Working Group** 的共識建議：
  - 呼籲法規機構對 mHealth 技術加強 oversight。
  - 對醫療人員的三項簡單 call to action：
    1. **熟悉**數位健康 apps 的優缺點 (be knowledgeable)。
    2. **支持並指導**病人使用 apps 來強化糖尿病管理與生活型態調整。
    3. **運用健康資料**改善照護品質與健康結果。
  - 實務相關性：mHealth 的成效在 **younger vs older** 病人、以及行動科技近用程度不同者之間有差異——醫療人員最適合提供脈絡化建議。

### ⭐ 使用者智慧與整體結論

- Google Play 與 Apple App Store 的 **star-rating 系統**讓使用者回饋 app 的效用，凸顯好用/有問題的 apps。
- 一項對 T1D/T2D 熱門 app 使用調查結論：使用糖尿病 apps 自我管理與 **self-care behavior 正相關**，可支持生活型態與血糖監測的改變。
- 整體：telemedicine 與 mHealth apps 對糖尿病病人是公認的助益；使用者的健康與數位素養 (health and digital literacy) **並非隱含問題**——事實上，數位科技反而能**促進 diabetes health literacy**。

> 📌 **重點 (High-Yield)**：
> - 2022/11 搜尋：**85 個廠商相關 + 56 個 independent** apps；最常見 independent 功能 = 血糖日記 / 飲食規劃。
> - **80% T1D 受訪者願分享 real-time glucose data** 換取個人化支援。
> - **Digiceuticals**＝臨床驗證、**需醫師處方**才能取得的 mHealth app。
> - FDA database 出版時**僅列硬體廠商的 apps**；CE mark 非必要。
> - 數位科技可**提升**而非削弱 health literacy。

---

## 📈 五、Ambulatory Glucose Profile (AGP)——檢視 CGM 資料的圖形化工具

AGP 是總結並視覺化密集 CGM 資料的 **公認標準方法 (accepted standard method)**，是理解每日/每週血糖樣態的演進中工具，設計目的同樣是支援 **shared decision making 與治療調整**。其有效運用建立在 **四個獨立元件 (four separate components)** 上。

### 🧩 元件 1：Data Capture（資料擷取）

- 條件：**連續 14 天 CGM 配戴 + ≥70% data capture**。
- 意義：此資料量足以滿意地代表「最多 90 天 glucose data 才會看到的 patterns and trends」——即 **HbA1c 所反映的時間範圍**。
- 臨床價值：因此可在**數週**內（而非數月）回顧 medication 或 lifestyle 的調整成效。

### 🚦 元件 2：Time in Ranges（報告期間的各範圍時間）

- 視覺摘要 CGM 使用者達成標準化 TIR、TBR、TAR 目標的程度（international consensus；見 Table 36.3、Fig. 36.8）。
- **一致 color-coding** 共識，可優化安全性與臨床判讀：
  - 🟢 **Green** = 理想血糖範圍 (desired)。
  - 🔴 **Red** = 第一優先處理 (first priority for attention)，即低血糖端。
  - 🟡🟠 **Yellow / Orange** = 高血糖樣態，應作為 medication 或 behavioral 調整的焦點，目標是把它們移回 green。

### 🌀 元件 3：The Modal Day（眾數日／典型一日）的視覺構成

14 天 AGP 的大量資料，被顯示成「彷彿所有讀數都發生在**單一 24 小時**」——即 **modal day**。modal day 由四個關鍵特徵構成（Fig. 36.9）：

1. **Target glucose range**：通常 **70–180 mg/dL (3.9–10.0 mmol/L)**（懷孕例外），以 **green** 著色。
2. **Median line（中位數線，50%）**：較深的實線，描繪 modal day 每一時點的中位數血糖；顯示平均血糖是否落在 green target 內、以及典型一日內的振盪程度。
3. **25th–75th percentile band（IQR，四分位距）**：較深的陰影帶，涵蓋最接近中位數的 **50% 讀數**及其 day-to-day 變異。
   - 反映**多數日子都會出現的每日趨勢**，主要指出 meals 與 medication（常為 insulin）如何影響血糖。
   - **IQR band 越寬 = day-to-day 變異越大**。
4. **5th–95th percentile range**：最淺的陰影帶，代表**僅在某些日子出現**的較不頻繁變異，可反映 behavior 與 lifestyle 因素對血糖的影響。

⚠️ **重要**：位於 5th–95th percentile **之外**的最高與最低各 5% 讀數**不顯示**於 AGP。這些是 rarely-occurring outliers，不應影響臨床判斷。

### 📊 表格解讀（Fig. 36.9 範例 AGP 報告數據重建）

下表為原文 Fig. 36.9「Sam test patient」範例報告（14 days: Aug 8–21, 2021；Time CGM active: 100%）：

**Time in Ranges（type 1/type 2 目標）**

| Range | Glucose Level | % | Goal |
| --- | --- | :---: | --- |
| Very high | > 250 mg/dL | 20% | < 5% |
| High | 181–250 mg/dL | 24% | （High+Very high 合計 < 25%） |
| Target (TIR) | 70–180 mg/dL | **46%** | **> 70%**（每 +5% 即臨床有益） |
| Low | 54–69 mg/dL | 5% | < 4% |
| Very Low | < 54 mg/dL | 5% | < 1%（每 1% ≈ 15 分鐘） |

**Glucose Metrics**

| Metric | Value | Goal |
| --- | --- | --- |
| Average glucose | 175 mg/dL | < 154 mg/dL |
| Glucose management indicator (GMI) | 7.5% | < 7% |
| Glucose variability (%CV) | 45.5% | ≤ 36% |

**Modal Day — Median (50%) 曲線（mg/dL）**

| Time | 12am | 3am | 6am | 9am | 12pm | 3pm | 6pm | 9pm | 12am |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Median | 220 | 150 | 100 | 150 | 200 | 180 | 180 | 190 | 230 |

- **欄位含義**：TIR 表用 5 個範圍 + 各自 % + consensus goal；metrics 表給 average glucose、GMI、%CV 與其目標；modal day 表是中位數線每 3 小時的取樣。
- **臨床意涵（以此範例判讀）**：
  - **TIR 46% < 70%**（未達標）；**TAR（>180）= 44%、TBR（<70）= 10%** 皆超標。
  - **Average glucose 175 > 154**、**GMI 7.5% > 7%**、**%CV 45.5% > 36%**——血糖高且**變異大**。
  - Modal day 顯示**清晨 6am 最低 (100)**、**午夜前後最高 (220–230)**——夜間/睡前高血糖樣態。
- **易混淆點 / 考點**：
  - 「Each 5% increase in TIR is clinically beneficial」「Each 1% time in range ≈ 15 minutes」是常考的轉換語句。
  - GMI 與 average glucose 的目標（<7% / <154 mg/dL）要與 %CV ≤36% 一起記。
  - Daily glucose profiles（最底部 14 條 sparkline，midnight-to-midnight）讓變異能對應到**特定星期幾的日常活動**。

### 📅 元件 4：Daily Glucose Profiles（每日血糖剖面）

- 位於 AGP 報告**最底部**，顯示 14 天內**每一天的個別 glucose trace**（每條為 midnight-to-midnight）。
- 用途：判斷 AGP 中的變異能否以**不同每日活動的脈絡**來解讀。
  - 例：是否某些固定發生於某星期幾的活動，造成特定的血糖控制變化？

> 📌 **重點 (High-Yield)**：
> - AGP 四元件：**Data capture → Time in ranges → Modal day → Daily profiles**。
> - **14 天 + ≥70% capture** ≈ 代表最多 90 天樣態（= HbA1c 的時間尺度）。
> - Modal day 四特徵：**green target、median line、IQR (25–75) band、5th–95th band**；**band 越寬＝變異越大**。
> - **最高/最低各 5%（5th–95th 之外）的 outliers 不顯示**——避免被罕見極端值誤導。

---

## 🔎 六、系統性判讀 AGP 報告的步驟法（Box 36.2）

AGP 可用一套 **systematic stepwise process** 找出血糖控制趨勢以利臨床決策（無正式共識，但 Box 36.2 提供結構）。

| 步驟 | 內容 | 目標/門檻 |
| --- | --- | --- |
| **Step 1：Check Data Capture** | 確認 14 連續天中擷取 **>70%** 資料（反映 CGM 使用 adherence） | >70% over 14 days |
| **Step 2：Investigate TBR（< 70 mg/dL）** | <4% → 達標可往下；**≥4% 需追查原因**，尤其 ≥1% 低於 **54 mg/dL (3.0 mmol/L)**。高風險者 consensus 建議 **<1%** 低於 70 mg/dL | <4%（高風險 <1%） |
| **Step 3：Investigate TAR（> 180 mg/dL）** | <25% → 達標；**≥25% 需追查**，尤其 ≥5% 高於 **250 mg/dL (13.9 mmol/L)** | <25% |
| **Step 4：Investigate Glucose Variability（%CV）** | 目標 **≤36%**（>36% 低血糖風險顯著上升）。>36% 時，找 AGP 中 **IQR band 與 5th–95th band 變寬**之處 | CV ≤ 36% |
| **Step 5：Review GMI vs recent HbA1c** | 比較 GMI 與最近 HbA1c，判斷 glycator 類型；若為 **high glycator**，治療強化**僅依 GMI** | 見下方 glycator 說明 |

### 🧮 Step 5 深入：GMI、HbA1c 與「glycator」概念

- **GMI (glucose management indicator)**：14 天 AGP 期間的 **glucose exposure** 指標，由 CGM 平均血糖計算，以 DCCT 或 IFCC 標準化單位報告（% 或 mmol/mol，如同 HbA1c）。
- **為何重要**：HbA1c 只是長期血糖暴露的 surrogate，會受多種**非血糖因素 (nonglycemic factors)** 影響，未必只反映平均血糖；GMI 則**僅根據平均血糖**估計長期暴露。
- **Glycator 分類與處置**：

| 類型 | GMI vs HbA1c | 處置原則 | 機轉/陷阱 |
| --- | --- | --- | --- |
| Low / average glycator | GMI **高於或相當於** HbA1c | 治療強化可依 GMI **或** HbA1c | 若 HbA1c 反而**低於** GMI，須考慮 **high RBC turnover（如 occult blood loss）假性壓低 HbA1c** |
| **High glycator** | GMI **明顯低於** 近期 HbA1c | 治療強化**只用 GMI 值** | 若**僅憑 HbA1c** 強化 → **低血糖風險** |

- GMI 與 HbA1c 所測平均血糖的關係，會因 **ethnic / racial 等多種因素**而不同。

### 💡 記憶法 / 口訣

- **AGP 判讀五步口訣：「擷低高變糖」**
  1. **擷** = 擷取 Data capture (>70%/14天)
  2. **低** = TBR（<70，目標 <4%；54 是危險線）
  3. **高** = TAR（>180，目標 <25%；250 是危險線）
  4. **變** = Variability（%CV ≤36%）
  5. **糖** = GMI vs HbA1c（glycator）
- **先看低、再看高**：Step 2（TBR）排在 Step 3（TAR）**之前**——「**降低低血糖是糖尿病指引的核心 (at the heart of guidelines)**」，安全優先。
- **Glycator 口訣**：「**High glycator → trust GMI**」——HbA1c 被高估，盲目依 HbA1c 強化會招致低血糖。

> 📌 **重點 (High-Yield)**：
> - 五步順序固定：**Data capture → TBR → TAR → Variability → GMI**；**TBR（安全）優先於 TAR**。
> - 關鍵門檻：TBR <4%（高風險 <1%；危險線 54 mg/dL ≥1%）、TAR <25%（危險線 250 mg/dL ≥5%）、**%CV ≤36%**。
> - **High glycator**（GMI < HbA1c）：治療強化**只依 GMI**，否則有**低血糖風險**。
> - **HbA1c < GMI** 時要想到 **high RBC turnover / occult blood loss** 假性壓低 HbA1c。
> - %CV >36% 時，於 AGP 找 **IQR band 與 5th–95th band 變寬** 的時段。

---

## 🧠 全章節速記總表（Cheat Sheet）

| 主題 | 必記一句話 |
| --- | --- |
| 跨廠牌平台 | **Glooko + Tidepool** 唯二 multiple brands = Yes |
| 純單功能平台 | Clarity=純CGM、t:connect=純pump、Carelink CGM欄=No |
| Caregiver app | 遠端 high/low alerts；**青少年 autonomy** 是衝突點 |
| mHealth 數據 | 85 廠商 + 56 independent（2022/11）；80% 願分享 real-time data |
| Digiceuticals | 臨床驗證 + **需醫師處方** |
| AGP 四元件 | Data capture → Time in ranges → Modal day → Daily profiles |
| AGP 門檻 | TIR >70%、TBR <4%、TAR <25%、%CV ≤36%、GMI <7% |
| AGP 五步 | **擷低高變糖**（TBR 先於 TAR） |
| Glycator | High glycator (GMI<HbA1c) → 強化只依 **GMI** |
