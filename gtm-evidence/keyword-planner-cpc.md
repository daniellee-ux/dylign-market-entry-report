# Google Keyword Planner — 關鍵字 CPC / 搜量實測

> GTM 證據數據 · 用於收窄 CAC 估算的 CPC 分子,並判斷付費搜尋的可承接量。

## 一、怎麼取得的(方法與可複現性)

- **工具**:Google Keyword Planner(ads.google.com/aw/keywordplanner)。
- **帳號**:用戶自己的 Google Ads 帳號 **324-430-2868**,透過 Claude 的 Chrome 擴充功能操作用戶**已登入**的真實瀏覽器(Playwright 用不了,因為它是全新無登入 session)。
- **路徑**:Keyword Planner →「Get search volume and forecasts」→ 貼入下方 15 個關鍵字(逗號分隔)→ Get started → 生成 plan。
- **關鍵設定(重要)**:預設地區是 **Taiwan**,已手動改成 **United States**(移除 Taiwan、加入 United States country,並 Save)——否則搜量/CPC 全錯。
- **抓取日期**:2026-07-06(plan 標題 "Plan from Jul 6, 2026")。
- **數據時間範圍**:Jun 2025 – May 2026(KP 預設近 12 個月)。
- **欄位**:Avg. monthly searches / Competition / Top of page bid (low range) / Top of page bid (high range)。
- **只讀不動**:全程只用規劃/預測工具查數,未建立廣告、未出價、未花錢、未改帳號設定。

### 換算與精度限制(誠實標註)
- 帳號幣別是 **TWD**,所以 KP 顯示的是 **NT$**;下表 USD 按 **≈32 TWD/USD** 換算(±幾 %,不影響量級)。
- Top of page bid 是 **Google 的模型區間(low≈低分位、high≈高分位)**,**不是保證實付 CPC**;實際 CPC 通常落在 low 與 high 之間、偏低中段。
- 搜量是**粗分桶**(10–100 / 100–1k / 1k–10k / 10k–100k)——此帳號未投放,拿不到精確整數。
- **CPC 只是 CAC 的分子;分母(轉化率)仍是假設,必須靠原型實測。** `CAC = CPC ÷ 轉化率`。

## 二、數據(美國地區,2026-07-06 抓)

| 關鍵字 | 月搜量(US) | 競爭 | CPC 低 NT$ | CPC 高 NT$ | CPC 低 US$ | CPC 高 US$ |
|---|---|---|---|---|---|---|
| custom stickers | 10k–100k | High | 50.93 | 262.84 | $1.59 | $8.21 |
| custom bottle labels | 1k–10k | High | 48.98 | 210.33 | $1.53 | $6.57 |
| custom labels | 1k–10k | High | 65.17 | 463.31 | $2.04 | $14.48 |
| label printing | 1k–10k | High | 61.34 | 481.67 | $1.92 | $15.05 |
| custom beer labels | 100–1k | High | 53.09 | 251.04 | $1.66 | $7.85 |
| custom food labels | 100–1k | High | 44.62 | 362.26 | $1.39 | $11.32 |
| custom jar labels | 100–1k | High | 48.27 | 208.09 | $1.51 | $6.50 |
| custom product labels | 100–1k | High | 87.99 | 392.81 | $2.75 | $12.28 |
| custom roll labels | 100–1k | High | 189.51 | 1,358.32 | $5.92 | $42.45 |
| food label printing | 100–1k | High | 45.99 | 294.18 | $1.44 | $9.19 |
| custom sauce labels | 10–100 | Medium | 110.51 | 351.29 | $3.45 | $10.98 |
| custom labels no minimum | 10–100 | High | 79.87 | 316.56 | $2.50 | $9.89 |
| waterproof labels custom | 10–100 | High | 82.98 | 407.82 | $2.59 | $12.74 |
| small batch label printing | 10–100 | High | 111.88 | 411.74 | $3.50 | $12.87 |
| short run labels | 10–100 | High | 165.58 | 886.90 | $5.17 | $27.72 |

## 三、結論(進費米模型 + GTM)

**① CAC:冷啟動付費搜尋 CAC ≈ $100–250(基準 ~$150–200),不是先前樂觀的 $70。**
- 目標食品/飲料標籤詞 CPC 低檔 ~$1.4–3.5、有效 CPC ~$3–6;配轉化 1.5–3% → `$3–6 ÷ 1.5–3% ≈ $100–250`。
- 若搶 B2B 卷標詞(custom roll labels CPC 高達 $42、short run labels $28),CAC 可破 $400。

**② GTM:高意圖食品標籤詞的「量」很薄——付費搜尋單靠自己撐不起來。**
- 有量的是廣詞(custom stickers 10k–100k、custom labels / label printing 1k–10k),但不精準、更貴、競爭 High。
- 精準食品詞(sauce / beer / jar / food labels)多為 100–1k 甚至 10–100 月搜。
- 實證印證舊報告「細分頭部詞月搜僅 30–420」——**量要靠 SEO 長尾 + 其他渠道 + Dylign 對既有客戶的 cross-sell,不能只靠付費搜尋。**

## 三·五、二輪 CPC 擴容——非食品/跨場景（2026-07-06，Ubersuggest 估值）

> 一輪(§二)為 Google Keyword Planner 的食品/廣詞 CPC。二輪把目標詞擴到**非食品垂直 + 工具 + 能力詞**,CPC 取自 Ubersuggest(登入帳號,US locId 2840)。完整搜量/SD/判讀見 `seo-keyword-strategy.md` §三·七。

| 關鍵字 | 月搜 | SD | CPC | 類別 |
|---|---|---|---|---|
| candle labels | 2,900 | 26 | $3.57 | 非食品垂直 |
| soap labels | 880 | 21 | $2.23 | 非食品垂直 |
| cosmetic labels | 320 | 22 | $7.93 | 非食品垂直 |
| essential oil labels | 170 | 25 | $4.77 | 非食品垂直 |
| custom bottle labels | 1,300 | 27 | $5.51 | 飲料外側標 |
| beer labels | 1,300 | 26 | $6.51 | 飲料外側標 |
| jar labels | 1,000 | 34 | $3.93 | 跨垂直 |
| waterproof labels | 2,400 | 31 | $6.48 | 能力鉤子 |
| product labels | 2,900 | 41 | $9.07 | 廣商業 |
| roll labels | 590 | 27 | **$30.38** | B2B 機貼（CPC 異常高） |
| barcode generator | 368,000 | 39 | $4.19 | 工具磁鐵 |
| barcode generator free online | 27,100 | 13 | $2.27 | 工具磁鐵 |
| custom labels no minimum | 20 | 34 | **$10.78** | 定位詞（轉化用） |

**進 CAC 模型的口徑修正:**
- **非食品目標詞有效 CPC ~$2.2–7.9**(candle/soap 最便宜),與一輪食品詞同量級——**混合 CAC(≈$100–250)結論不變**;但 soap/candle 這種「低 SD＋低 CPC」的詞,是**壓低 CAC 的最佳入口**。
- **roll labels $30.38、custom labels no minimum $10.78** ＝高意圖高價詞:只做**小預算精準 PPC**,不冷啟走量。
- **barcode generator**($4.19、PD 5＝付費競爭低)＋免費工具引流,把獲客成本壓到接近零——直接改善混合 CAC(同 §三 結論②)。

## 四、可補強(若要更硬)
- 換一個**曾投放過的 Google Ads 帳號**可拿到精確搜量(非分桶)與更窄的 CPC 區間。
- 轉化率:上線後用首月實投測(判死線 H3),得到真 CAC = 實付 CPC ÷ 實測轉化。
