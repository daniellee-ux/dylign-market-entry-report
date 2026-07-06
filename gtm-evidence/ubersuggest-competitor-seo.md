# Ubersuggest — 競品 SEO / 自然流量實測 + Dylign SEO 策略

> GTM 證據數據 · 判斷競品靠什麼渠道獲客、SEO 空間是否可競爭，並據此擬定 Dylign SEO 策略。

## 一、怎麼取得的（方法與可複現性）

- **工具**：Ubersuggest（app.neilpatel.com）→ Traffic Analyzer → Overview，逐個輸入競品域名。
- **帳號**：用戶自己的 Ubersuggest 登入帳號，透過 Claude 的 Chrome 擴充功能操作已登入的真實瀏覽器。
- **設定**：Language/Country = English / United States（locId 2840）。**抓取日期 2026-07-06**。
- **分析 6 個域名**：avery.com、stickermule.com、onlinelabels.com、bluelabelpackaging.com、noissue.co、sttark.com。
- **只讀**；**精度限制**：Ubersuggest 流量/關鍵字是第三方估算（非 GA 真值），量級可信、精確值參考。

## 二、六域對照（美國自然流量）

| 域名 | 定位 | 自然流量/月 | 付費 | DA | 自然關鍵字 | 流量引擎 |
|---|---|---|---|---|---|---|
| **avery.com** | 標籤模板/耗材巨頭 | **1,800,000** | **0** | 65 | 130,980 | **免費模板帝國**(/templates 187k、templates avery 135k、5160、名片模板) |
| **onlinelabels.com** | 空白標籤/模板站 | **297,132** | 23(0.01%) | 59 | 30,358 | **免費工具**(營養標籤產生器 48k、條碼產生器 17k)+ 空白/定制標籤 |
| **stickermule.com** | 通用貼紙領導 | 239,270 | 166(0.07%) | 77 | 31,229 | 通用貼紙詞 + 品牌 + 對比長文 |
| **bluelabelpackaging.com** | B2B 精釀/食品標籤 | 31,964 | 0 | 32 | 2,822 | 精釀內容 + **品牌混淆詞灌水**(「blue label label」74k) |
| **noissue.co** | eco 包裝(貼近 Dylign ICP) | 21,692 | 5(0.02%) | 41 | 7,116 | 產品線廣度(食品包裝紙/棉紙/咖啡袋)+ 品牌 |
| **sttark.com** | B2B 精品標籤 | 2,297 | 0 | 36 | 2,373 | 盒子/紙箱資訊長文 + 品牌 |

## 三、各家靠什麼詞/頁拿流量（重點）

- **OnlineLabels（最關鍵）**：頂頁 = **免費營養標籤產生器 /tools/nutrition-label-generator 48,664 訪問**(超過它的 /custom-labels 商業頁 35,043)、**免費條碼產生器 17,378**。頂詞:nutrient facts label(27,100)、nutrition information label maker(5,400·pos1)、making a nutrition label——**它的 SEO 護城河是「食品品牌需要的免費工具」，再導流到賣標籤。**
- **Sticker Mule**：customise stickers(90,500·pos2)、sticker makers、custom packages——**全通用貼紙/品牌詞，零食品標籤詞**。
- **Sttark**：盒子/紙箱長文(carton define、folding cartons)+ 品牌，美國自然詞僅 1,009，幾乎不排 custom label 商業詞。
- **Blue Label**：「blue label label」74k(pos1·約 16,864 訪問)幾乎確定是品牌混淆(Johnnie Walker 等)非買標籤意圖；真實流量靠 growler/beer/barcode 教育內容。
- **noissue**：food wrapping paper(1,900·pos1)、產品線頁 + 品牌 + 「what is a hang tag」；標籤詞非其強項。

## 四、六個域名收斂出的鐵律

1. ~~**付費全部 ≈ 0（6/6，含 1.8m 流量的巨頭 Avery）**。這品類靠自然/內容贏，不靠廣告——連最大玩家都零廣告。~~ ⚠️ **此條已被廣告庫實測推翻（見 `meta-google-ad-scan.md`）。** Ubersuggest 的「付費關鍵字數」只抽樣搜尋詞、漏掉展示/影片/購物/PMax，嚴重低估。實測：**六家全部投 Google 廣告**（~23–3,000 條創意），四家還投 Meta。**正確口徑：付費搜尋是本品類基本盤（table stakes），不是「沒人投」；差異在渠道組合與 CTA 風格跟著商業模式走（DTC＝Google+Meta 直購 / B2B＝只 Google 詢價）。** 判斷誰投廣告要用廣告庫，別用 Ubersuggest 付費關鍵字數。
2. **沒有人靠 SEO 佔住「custom 食品/飲料 label」商業詞**。贏家都靠:免費工具(OnlineLabels)、通用詞(SM)、旁支內容(Sttark 盒子/Blue Label 精釀)、產品廣度(noissue)、或品牌/混淆詞。
3. **這空間 SEO 槓桿最高的資產 = 食品品牌需要的「免費工具」**。OnlineLabels 的營養標籤產生器單頁 48k/月、條碼產生器 17k/月，都贏過它自己的商業頁。**這正好等於 Dylign 差異化裡的「食品合規字段模板」——它既是產品功能，也是第一獲客引擎。**
4. **DA 可競爭**。相關標籤玩家 DA 32–59(SM 77 例外);Dylign 從零用「工具+內容+反鏈」飛輪，12–24 月達 DA 30–40 是現實的。

---

## 五、Dylign SEO 策略（evidence-based，可執行）

### 不打不可能贏的地方
- 通用貼紙詞 → Sticker Mule DA 77,放棄。
- 通用「label / online label」→ OnlineLabels DA 59,放棄。
- **通用「label template / avery 模板」→ Avery DA 65、1.8m/月的免費模板帝國,放棄。**

### 支柱 1 — 免費「食品合規」工具（最高槓桿,但要挑對格）
免費工具/模板是本品類 SEO 最強引擎(Avery 1.8m、OnlineLabels 48k 都證明了)。**但要分格:通用模板(名片/地址標/Avery 5160)已被 Avery 壟斷,不能碰;開放的是「食品合規」這一格**——Avery 是通用辦公模板,不做食品合規;OnlineLabels 只搶了「營養標籤」一個工具。Dylign 應建一套**食品合規工具**,Avery 不在、OnlineLabels 只點了一個:
- **營養成分標籤產生器(FDA 格式)** ← OnlineLabels 實證單頁 48k/月(已有人做,但空間仍大)
- 過敏原/成分標籤產生器、cottage food 各州標籤要求檢查器(**無人做**)
- **條碼/UPC 產生器** ← 實證 17k/月
- 按容器的標籤尺寸/刀線指南(瓶/罐/杯)
- 這就是報告「食品合規字段模板」——一物三用:產品功能 + 第一 SEO 引擎 + 對既有客戶的獲客鉤子。Dylign 的整合優勢(免費合規工具 + 直接接單印刷)比 OnlineLabels(賣空白標籤)、Avery(通用模板)、ReciPal(只出檔不印,收 $29–129/月)都完整。

### 支柱 2 — 圍繞食品標籤的教育型長文（已驗證的內容打法）
照抄「die-cut vs kiss-cut」「growlers vs crowlers」的教育長文模式,但瞄準食品:
- 「如何寫 FDA 合規食品標籤」
- 「醬料/飲料瓶標:BOPP vs 紙標怎麼選」
- 「熱醬瓶標尺寸指南」「防水標籤怎麼選」
- 精釀:啤酒/康普茶/冷萃標籤指南。

### 支柱 3 — 商業長尾產品頁（無強佔位者）
針對 Keyword Planner 那批食品標籤商業詞(custom sauce/beer/jar/bottle labels、food label printing)——量小但競爭低、意圖高,每詞一個優化落地頁。

### 支柱 4 — 現實預期與節奏
- 相關對手 DA 32–41,Dylign 12–24 月達 DA 30–40 現實可行。
- 付費搜尋只當種子(接受 CAC $100–250)先買早期流量,SEO(工具+內容)複利起來後主導獲客。
- **關鍵順序**:先上 1–2 個免費工具(營養標籤/條碼)搶 SEO 頭部,同步鋪教育內容與商業長尾頁。

## 六、可補強
- 尚未拉:StickerYou、Vistaprint、Vograce、GS-JJ、Avery(可再各花一次)。Avery 值得補——它可能靠免費模板佔住「label template」資訊詞,驗證「免費工具」打法的天花板。
- 廣告素材面(Meta / Google Transparency / TikTok Creative Center)未做,屬同一 GTM 工作流下一輪。
