# Ch.36 趨勢箭頭與胰島素劑量調整（Trend Arrows & Insulin Dosing — the "Slide Rule" Systems）

> 來源：Williams Textbook of Endocrinology, Ch.36 Digitized Approaches to Diabetes — 涵蓋 Trend arrows 與 projected glucose 概念、各 CGM 廠商 trend arrow 對應 rate of change（Table 36.2）、以 trend arrow 做 insulin dosing 的演進（"slide rule" 系統）
---

## 🩸 用 CGM 做每日決策（Making Daily Decisions Using CGM）

- CGM 對 PWD（people with diabetes）最重要的第一項好處：**改善每日 diabetes self-management 的決策品質**。
- 隨時（白天或夜間）皆可 on-demand 看到當下血糖，<u>不需 fingerprick SMBG</u>，使 CGM 使用者對自身血糖狀態更有警覺。
- 但要注意：<u>單看一個高或低的數值</u>就採取 corrective action，這個動作**可能需要、也可能不需要** —— 容易過度反應。
- CGM 真正更強大的能力在於：除了當下血糖，還同時提供 **trend arrow**，告訴你血糖變化的<u>方向 (direction)</u> 與 <u>變化速率 (rate of change)</u>（Fig. 36.6）。

> 📌 **重點 (High-Yield)**：
> - CGM 對日常決策的核心價值＝**current glucose + trend arrow**，不是只有一個 spot value。
> - 只看單一數值就行動 = 危險；必須結合「方向＋速率」的趨勢資訊。

---

## 📈 Trend Arrows 與 Projected Glucose 的概念

- CGM 以 **minute-by-minute（逐分鐘）** 收集血糖讀值。
- 每套系統會根據 <u>過去 15 分鐘</u> 儲存的讀值，計算出血糖的：
  - **方向 (direction)**：上升、下降或穩定。
  - **速率 (rate of change)**：上升/下降有多快。
- 這個資訊在 CGM reader 或 smartphone app 上以 **trend arrow** 顯示。
- 臨床意涵 — 把當下血糖配上 trend arrow，使用者可做出 informed and timely 的決策：
  - 是否需要 corrective action（**打 insulin** 或 **補 carbohydrates**），以預防不想要的血糖上升或下降。
  - 理解血糖的 context（脈絡），進而決定 **運動、進食的時機**，以及 **生病期間 (illness)** 的血糖管理。
- 「projected glucose」概念：trend arrow 等於是對「血糖將往哪走、走多快」的預測 —— 讓決策從「反應現在」進化到「預期未來」。

> 📌 **重點 (High-Yield)**：
> - Trend arrow 的演算基礎 = <u>過去 15 分鐘</u> 的讀值（考點數字！）。
> - Trend arrow 同時編碼兩件事：**方向 + 速率**。
> - 應用面：corrective insulin/carb、運動與進食時機、sick-day management。

---

## 📊 Table 36.2：各 CGM 廠商 Trend Arrow 對應的 Rate of Change 比較

> ⚠️ 這是本節最大考點：**不同廠商的箭頭，代表的 mg/dL/min 並不相同**，且箭頭的「數量與方向設計」也不同。同一個「↑」在 Abbott 與 Dexcom 代表的速率就不一樣。

| Trend Arrow（數量與方向） | Abbott FreeStyle Libre System ᵃ | Dexcom G4/G5/G6/G7 Mobile ᵇ | Medtronic Guardian Connect / Sensor 3 / Sensor 4 ᶜ | Roche/Senseonics Eversense ᵈ |
| --- | --- | --- | --- | --- |
| ↑↑↑ | NA | NA | **>3 mg/dL**（>0.2 mmol/L）/min | NA |
| ↑↑ | NA | **>3 mg/dL**（>0.2 mmol/L）/min | 2–3 mg/dL（0.1–0.2 mmol/L）/min | NA |
| ↑ | **>2 mg/dL**（>0.1 mmol/L）/min | 2–3 mg/dL（0.1–0.2 mmol/L）/min | 1–2 mg/dL（0.05–0.1 mmol/L）/min | **>2 mg/dL**（>0.1 mmol/L）/min |
| ↗ | 1–2 mg/dL（0.05–0.1 mmol/L）/min | 1–2 mg/dL（0.05–0.1 mmol/L）/min | NA | 1–2 mg/dL（0.05–0.1 mmol/L）/min |
| → | <1 mg/dL（<0.05 mmol/L）/min | <1 mg/dL（<0.05 mmol/L）/min | NA | 0–1 mg/dL（0–0.05 mmol/L）/min |
| ↘ | 1–2 mg/dL（0.05–0.1 mmol/L）/min | 1–2 mg/dL（0.05–0.1 mmol/L）/min | NA | 1–2 mg/dL（0.05–0.1 mmol/L）/min |
| ↓ | **>2 mg/dL**（>0.1 mmol/L）/min | 2–3 mg/dL（0.1–0.2 mmol/L）/min | 1–2 mg/dL（0.05–0.1 mmol/L）/min | **>2 mg/dL**（>0.1 mmol/L）/min |
| ↓↓ | NA | **>3 mg/dL**（>0.2 mmol/L）/min | 2–3 mg/dL（0.1–0.2 mmol/L）/min | NA |
| ↓↓↓ | NA | NA | **>3 mg/dL**（>0.2 mmol/L）/min | NA |

ᵃ 所有 FreeStyle Libre 系統。ᵇ 所有 Dexcom Mobile 系統。ᶜ Medtronic Guardian Connect。ᵈ Ascensia/Eversense user guides。
> 此表為各廠商「常用 standalone CGM」之產品線，亦是 T1D / T2D 臨床研究中最常用的系統；市面上尚有其他 CGM 系統。

### 📊 表格解讀

- **欄位含義**：列＝箭頭的「數量與方向」（最多 3 個箭頭、最少 1 個）；欄＝四大廠商；格子內＝該箭頭代表的 **血糖變化速率（mg/dL per minute，括號為 mmol/L）**。
- **箭頭數量設計不同（最易混淆點）**：
  - **Abbott FreeStyle Libre**：只有 **5 種**箭頭（↑ ↗ → ↘ ↓），<u>沒有雙/三箭頭</u>。所以 Libre 的單箭頭「↑」門檻最低，僅 **>2 mg/dL/min**。
  - **Dexcom**：有 **7 種**（↑↑ ↑ ↗ → ↘ ↓ ↓↓），雙箭頭 ↑↑/↓↓ 代表 **>3 mg/dL/min**。
  - **Medtronic（Guardian）**：有 **三箭頭（↑↑↑ / ↓↓↓）** 系統，三箭頭代表 **>3 mg/dL/min**；且 Medtronic <u>沒有斜箭頭 ↗ ↘ 與水平 →</u>（表中為 NA）。
  - **Eversense**：與 Libre 類似為 5 種箭頭（↑ ↗ → ↘ ↓），水平 → 定義為 **0–1 mg/dL/min**（略不同於 Libre/Dexcom 的 <1）。
- **同一箭頭、不同速率（核心考點）**：
  - 「↑」單箭頭：Abbott=**>2**、Dexcom=**2–3**、Medtronic=**1–2**、Eversense=**>2** mg/dL/min —— 四家全不同。
  - 「最快上升」的最高階箭頭都收斂在 **>3 mg/dL/min**，但 Dexcom 用 ↑↑（雙）、Medtronic 用 ↑↑↑（三）來表達。
- **臨床意涵**：因為「<u>沒有跨廠商標準化（no standardization）</u>」，所以**胰島素劑量建議必須依各裝置的箭頭定義調整**，不能把 A 廠的演算法直接套用到 B 廠。換機種時務必重新衛教。

> 💡 **記憶法（廠商箭頭數量）**：「**Libre/Eversense 五；Dexcom 七；Medtronic 上看三箭**」
> - Libre & Eversense = 5 箭（無雙箭）
> - Dexcom = 7 箭（最高 雙箭 = >3）
> - Medtronic = 有三箭（最高 三箭 = >3，無斜箭/水平）

> 💡 **記憶法（速率分級, mg/dL/min）**：以 Dexcom/Medtronic 的「1–2 → 2–3 → >3」三段最直觀；對照 mmol/L 即 **0.05–0.1 → 0.1–0.2 → >0.2**。口訣：「**一、二、三 mg/dL ↔ 零點一、零點二 mmol/L**」。

> 📌 **重點 (High-Yield)**：
> - <u>跨廠商「無標準化」</u>是核心觀念 —— 箭頭數量、方向、速率對應全都不同。
> - 記住三個臨界：**>3、2–3、1–2 mg/dL/min**（對應 >0.2、0.1–0.2、0.05–0.1 mmol/L）。
> - Dexcom 最快＝**↑↑**（雙）；Medtronic 最快＝**↑↑↑**（三）；Abbott/Eversense 最快只到單箭 **↑（>2）**。

---

## 💉 把 Trend Arrow 納入胰島素劑量決策（Insulin Dosing with Trend Arrows）

- 多款 CGM 已獲衛生主管機關核可可用於 **insulin dosing 決策**，<u>不需 confirmatory SMBG</u>（即所謂 non-adjunctive use）。
- 治療決策必須同時考量：
  - **方向 (direction of trend arrow)**
  - **不同的速率 (rates of change)**
- 重申關鍵限制：**不同 CGM 在箭頭方向與速率上沒有標準化** → 胰島素劑量建議必須針對各裝置調整。
- 目前已有數個針對 T1D「如何依 trend arrow 調整 insulin」的發表建議（見下文 slide rule 演進）。

> 📌 **重點 (High-Yield)**：
> - CGM 可作 non-adjunctive（免確認性指尖血）劑量決策。
> - 劑量決策＝**方向 + 速率**雙要素；且須<u>按裝置別客製化</u>。

---

## 🔁 "Slide Rule" 系統的演進（Evolution of Trend-Arrow Insulin Dosing）

### 階段一：百分比調整（JDRF / DirecNet 時代）

- 在 **JDRF** 與 **DirecNet** 的 CGM 研究中，建議：依 trend arrow 與當下血糖，把 regular insulin dose：
  - **±10%**：血糖上升 (rising) 或下降 (falling)。
  - **±20%**：血糖<u>快速</u>上升 (rising rapidly) 或快速下降 (falling rapidly)。
- ⚠️ 問題（real-world 失真）：後續 patient-reported data 顯示
  - 上升箭頭 → 病人自行把劑量增加 **>100%**（遠超建議）。
  - 下降箭頭 → 自行把劑量減少 **up to 50%**。
  - → 顯示「百分比法」在真實世界容易被誇大執行，安全性堪憂。

### 階段二：固定數值加減（adjusted glucose 法）

- 改良為：依 trend arrow，把一個**固定的血糖數值**加到或減去當下血糖，得到「校正後血糖」再算劑量。
- ⚠️ 缺點：
  - 增加 CGM 使用者負擔，需要 **mathematical skills / numeracy**。
  - 即使簡化版，仍<u>未納入臨床因素</u>，如個別 insulin regimen 或 insulin sensitivity。

### 階段三：Slide Rule（查表加減固定胰島素量）

- 為盡可能納入多種因素，發展出多套 **"slide rule"** 查表法：
  - **Laffel et al** 與 **Aleppo et al**：依 **箭頭方向 + 速率**，查表加減一個**固定的胰島素單位數**；並依不同 **insulin sensitivity** 分層，<u>兒童與成人分開計算</u>（Fig. 36.7A）。此法較易依個別 insulin therapy 調整，並獲 **Endocrine Society** 推薦。
  - **Ziegler et al**：類似的 slide rule，但**加入 current glucose range** 作為查表變數（Fig. 36.7B）。
  - **Bruttomesso et al**：在 Ziegler 基礎上進一步修改，**增加 current glucose range 的數量** 與 **成人 insulin sensitivity 的分級數**。

### 💡 三階段演進比較表

| 階段 | 方法 | 核心變數 | 主要缺點 |
| --- | --- | --- | --- |
| 一 | **百分比**（JDRF/DirecNet） | 箭頭 → ±10%/±20% | real-world 被誇大（升 >100%、降 up to 50%）；未個別化 |
| 二 | **固定數值加減血糖** | 箭頭 → 校正當下血糖 | 需算數能力；未納 regimen / ISF |
| 三 | **Slide rule 查表加減固定 insulin** | 箭頭方向 + 速率 + **ISF**（Ziegler 再加 current glucose） | 對「上升血糖」傾向**高估**追加劑量 |

> 💡 **記憶口訣（演進三部曲）**：「**先用 %，再校正血糖，最後查表加 ISF**」（Percent → Add/Subtract glucose → Slide-rule with ISF）。

### 📊 Slide Rule 計算器（Fig. 36.7）重點

- Fig. 36.7 為依 **CGM trend arrow 方向 + 速率** 做胰島素劑量調整的 slide-rule calculators（**ISF = insulin sensitivity factor**）。
- **Endocrine Society 版（Fig. 36.7A，Laffel/Aleppo）**：用 **rate of change + ISF** 決定 insulin 調整量；**當箭頭穩定（→）時，不需調整胰島素**。
- **修改版（Fig. 36.7B，Ziegler）**：把 **ISF 與 current glucose** 結合，找出所需的胰島素調整量。
- 表中以 ISF 分層（如 **<25 / 25–49 / 50–74 / ≥75 mg/dL**）對應不同箭頭，給出 **+/−固定單位**（例如 ↑ 在 ISF<25 約 +3.5 U；↓↓ 在 ISF<25 約 −4.5 U；穩定箭頭則 0）。

### ⚖️ Slide Rule 系統的整體評價（考點）

- 採用程度不一（variably adopted）。
- 在 modeling scenarios 中：
  - **血糖下降（downward arrows）時：所有方法都被評為 effective。** ✅
  - **血糖上升（rising glucose）時：傾向 overestimate（高估）追加劑量** → 可能後續需要 corrective action（指反向校正，恐致低血糖風險）。
- ⚠️ 重要 caveat：**到目前為止，尚無 clinical study 評估各模型的個別或比較價值**（皆為 modeling 證據，非 RCT）。

> 📌 **重點 (High-Yield)**：
> - 演進三部曲：**% → 加減固定血糖 → slide rule 查表（+ISF）**。
> - 百分比法在 real-world 被誇大：升箭 → >100%、降箭 → up to 50%。
> - Laffel/Aleppo 法（兒童 vs 成人分表、依 ISF）獲 **Endocrine Society** 背書；Ziegler/Bruttomesso 再加 current glucose 變數。
> - Slide rule **對下降血糖有效、對上升血糖高估劑量**；<u>目前缺乏 head-to-head 臨床試驗</u>。
> - 「↗→↘」穩定/輕微變化時，slide rule 一般**不調整劑量**。

---

## ⭐ 本節總整理（One-page Summary）

- **Trend arrow = 過去 15 分鐘** 演算出的「方向 + 速率」，是 CGM 優於 spot SMBG 的關鍵。
- **Table 36.2 核心**：四大廠商箭頭定義不同 → 速率臨界 **1–2 / 2–3 / >3 mg/dL/min**（=0.05–0.1 / 0.1–0.2 / >0.2 mmol/L）；Libre/Eversense 5 箭、Dexcom 7 箭（雙箭最快）、Medtronic 有三箭（無斜箭/水平）。
- **無跨廠商標準化** → 劑量建議須按裝置客製，換機要重新衛教。
- **Slide rule** 三階段演進，Endocrine Society 推薦 ISF-based 查表；對**降糖有效、升糖高估**，且**尚無臨床試驗**驗證。

> 📌 **最終 High-Yield 速記**：
> - 數字記：**15 分鐘**（演算窗）、**>3 / 2–3 / 1–2 mg/dL/min**（速率三段）、百分比法被誇大成 **>100% / 50%**。
> - 概念記：**no standardization**、**Endocrine Society 推 ISF slide rule**、**升糖高估、降糖有效、無 RCT**。
