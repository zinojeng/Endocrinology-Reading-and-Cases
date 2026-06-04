# Ch.36 Digitized Approaches to Diabetes Diagnostics and Therapeutics — Fellow 精讀筆記

> 來源：**Williams Textbook of Endocrinology, Ch.36**（Battelino, Sherr, Galderisi, Dovč）
> 原始 PDF 經 **LlamaParse** 解析（見 [`_source/Ch36-raw-llamaparse.md`](_source/Ch36-raw-llamaparse.md)），再重整為 endocrinology fellow 適用的精讀筆記：條列式、繁中解說 + 英文專名、附**記憶法 / 口訣 / 比較表 / 表格解讀**，重點以**粗體**與 <u>底線</u> 標示。
> 🇹🇼🇬🇧 逐段英中對照：[`_source/Ch36-bilingual-EN-ZH.md`](_source/Ch36-bilingual-EN-ZH.md)

---

## 🗺️ 本章一句話

> 糖尿病科技 = **監測 (monitoring)** 與 **輸注 (insulin delivery)** 兩條主線，各自演進後在 **automated insulin delivery (AID)** 匯流。監測由 SMBG → **CGM**（用 **TIR/TBR/TAR** 取代單一 HbA1c）；輸注由 vial/syringe → pen → connected pen → **CSII pump** → SAP → **LGS → PLGS → hybrid closed-loop (HCL)**。

## 📚 分節索引

| # | 檔案 | 主題 | 核心表格 |
|---|------|------|----------|
| 00 | [Overview & Key Points](00-Overview-and-Key-Points.md) | 總論、10 條 Key Points、章節學習地圖、兩大支柱演進史 | 演進史表、KEY POINTS 三群表 |
| 01 | [CGM Sensors, Calibration & Accuracy](01-CGM-Sensors-Calibration-Accuracy.md) | 三種校正、MARD、time-lag；SMBG 與 HbA1c 的局限；triangle of diabetes care | **Table 36.1** 感測器屬性 |
| 02 | [Trend Arrows & Insulin Dosing](02-Trend-Arrows-Insulin-Dosing.md) | 趨勢箭頭、projected glucose、"slide rule" 劑量調整三部曲 | **Table 36.2** 各廠箭頭速率 |
| 03 | [CGM Metrics: TIR/TBR/TAR](03-CGM-Metrics-TIR-TBR-TAR.md) | TIR/TBR/TAR、TITR、%CV、各族群目標（老年、孕期） | **Table 36.3** 共識目標（最高分考點） |
| 04 | [Decision-Support & AGP Report](04-Decision-Support-and-AGP-Report.md) | 決策支援平台、mHealth apps、AGP 四元件與系統性判讀五步 | **Table 36.4**、Box 36.1/36.2 |
| 05 | [CGM Outcome Evidence & Telemedicine](05-CGM-Outcome-Evidence-and-Telemedicine.md) | CGM vs SMBG 招牌試驗、T1D/T2D 結果、telemonitoring、EMR 整合 | **Table 36.5 (+cont'd)** |
| 06 | [Insulin Delivery: Pumps → HCL](06-Insulin-Delivery-Pumps-to-Hybrid-Closed-Loop.md) | smart pen、CSII、SAP、LGS/PLGS/HCL 自動化階梯、lipodystrophy | 自動化階梯比較表 |
| 07 | [Automated Insulin Delivery (AID)](07-Automated-Insulin-Delivery-AID.md) | MPC/PID/fuzzy 演算法、hybrid 原理、特殊情境、open-source、access | 演算法比較表、療效表 |
| 08 | [Future Developments](08-Future-Developments-Insulin-Delivery.md) | 吸入/腹腔內 insulin、pramlintide/GLP-1/SGLT-i、bihormonal、長效輸注組、運動、月經 | 三大輔助藥比較表 |
| 09 | [Special Situations](09-Diabetes-Tech-in-Special-Situations.md) | 住院/ICU、NICU/PICU、preterm CGM 限制、住院 AID、孕期 AID、未來方向 | 住院目標表、NICU/PICU 證據表 |

---

## ⭐ High-Yield 速記（跨節濃縮）

**監測（01–05）**
- **MARD** 越低越準，現行 CGM 約 **8–14%**；blood↔interstitial **time-lag 3–15 min**（變化越快越大）。
- **HbA1c 兩大盲點**：看不到 **hypoglycemia** 與 **glycemic variability**；高估時導致 overintensification。
- **Table 36.3 一般成人目標必背**：<u>TIR >70%、TBR <4%（<54 為 <1%）、TAR <25%（>250 為 <5%）、%CV ≤36%</u>。
- **孕期 T1D「7-4-1」**：範圍 **63–140 mg/dL**，<u>TIR >70%、<63 為 <4%、<54 為 <1%</u>。
- **老年/高低血糖風險**：放寬為 <u>TIR >50%、TBR(<70) <1%</u>，安全（TBR）優先於達標（TAR）。
- **AGP 系統性判讀五步**口訣「**擷低高變糖**」：Data capture → TBR → TAR → %CV → GMI vs HbA1c。
- **招牌試驗**：DIAMOND、REPLACE、IMPACT、MOBILE、COMISAIR、RELIEF。

**輸注（06–09）**
- **自動化階梯**：MDI/pen → pump → SAP（加眼）→ **LGS（reactive）→ PLGS（proactive）→ HCL（雙向，自動 basal + 手動 meal bolus）→ AID**。
- **LGS vs PLGS**：已低才停 vs 預測快低先停；兩者皆**只能單向暫停 basal**。
- **AID 演算法**：**MPC**（預測）/ **PID**（反應）/ **fuzzy logic**（仿醫師）；目標 treat-to-target vs treat-to-range。
- **AID 療效**：TIR **+10–15%**（每天多 2.0–3.5 小時），降高血糖且**不增低血糖**；baseline HbA1c 最高者獲益最大。
- **Lipohypertrophy（輪替部位）vs Lipoatrophy（局部類固醇）**——口訣「肥厚輪替、萎縮類固醇」。
- **住院非重症目標 100–180 mg/dL**；preterm NICU 試驗常用 72–144 mg/dL（operational ≠ functional）。

> 📌 **一張圖記住自動化光譜（Fig. 36.11）**：SAP 58% < PLGS 60% < **AID 71%** TIR——automation 越多，TIR 越高。

---

*內容忠於原文、數字未外推。臨床決策請以最新指引與原文為準。*
