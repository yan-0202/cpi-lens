# 美國 CPI：計算方法、2026 年權重與來源查核

資料截止：2026-10-15。簡報分析 2026 年 9 月資料，發布日期為 2026-10-14。「下月」指 2026 年 10 月觀察值。

## 官方入口

- [BLS 最新 CPI 發布](https://www.bls.gov/news.release/cpi.nr0.htm)：滾動更新，引用時請記錄資料月份。
- [BLS 官方分類圖表](https://www.bls.gov/charts/consumer-price-index/consumer-price-index-by-category.htm)：顯示分類年增率，並非權重圖。
- [2026 年起始權重表：Table 1，2024 Weights](https://www.bls.gov/cpi/tables/relative-importance/2025.htm)：2025 年 12 月相對重要性。
- [2026 年新舊權重比較](https://www.bls.gov/cpi/tables/relative-importance/weight-update-comparison-2026.htm)：確認 2026 年採 2024 年支出資料。
- [權重與相對重要性的解釋](https://www.bls.gov/cpi/tables/relative-importance/)。
- [CPI 計算方法](https://www.bls.gov/opub/hom/cpi/calculation.htm)。

## CPI 如何計算

CPI 衡量消費者購買商品與服務的價格變動。本次統一使用 CPI-U、全美城市平均。不能把 CPI-W 或不同區域的權重混進同一張全國 CPI-U 圖。

編製分兩層：多數基本分類使用幾何平均計算價格相對變化，部分分類採不同公式；再以消費支出權重，透過修正 Laspeyres 架構加總。因此，「所有物價漲幅做簡單平均」並非 CPI。

- 月增率＝（本月指數／上月指數－1）×100%。分析短期動能通常採季調數列。
- 年增率＝（本月指數／去年同月指數－1）×100%。新聞稿主要採未季調數列。
- 分項貢獻的教學近似：前期分項相對重要性／100 × 分項漲幅。結果為百分點；實務應使用相容的期間、分類與季調口徑，不宜拿年初權重乘上所有已四捨五入的月增率，宣稱精確重建官方總指數。
- 同層、不重疊分類才可加總。能源分散在住宅、交通等大類；核心指數與能源、食品的分類方式又不同，不能把這些分類全部放在一張圓餅圖相加。

「2024 年支出權重」是支出參考期；「2025 年 12 月相對重要性」是價格更新到該月後的占比；「2026 年」是採用新權重編製指數的年度。三者並不矛盾。年度支出權重更新後，各月相對重要性仍隨相對價格移動。詳見上述 BLS 方法與權重說明。

## 2026 年起始權重：課堂 Table 1 的八大支出類別

使用 CPI-U，單位為占全項目百分比；非 2026 年全年平均，也非 9 月當期占比。由課堂 `cpi-relative-importance.md` 與 BLS Table 1 逐項比對。原始圖像未能從課堂 Markdown 清楚辨識，故以附件可辨識的八大支出分類為準，並補充官方圖表的常用分析分類。

| 中文分類 | BLS 分類 | 權重 |
|---|---|---:|
| 食品與飲料 | Food and beverages | 14.539% |
| 住宅 | Housing | 44.469% |
| 服飾 | Apparel | 2.368% |
| 交通運輸 | Transportation | 16.316% |
| 醫療保健 | Medical care | 8.423% |
| 娛樂 | Recreation | 5.137% |
| 教育與通訊 | Education and communication | 5.846% |
| 其他商品與服務 | Other goods and services | 2.902% |
| 合計 | All items | 100.000% |

來源：[BLS Table 1](https://www.bls.gov/cpi/tables/relative-importance/2025.htm)。簡報權重長條圖為依官方數據重繪，並非 BLS 原圖截圖。

## 官方分類圖表的主要群組對照

以下採同一份起始權重。縮排或父子關係代表包含，不能重複加總。

| 分析分類 | 權重 |
|---|---:|
| 食品 Food | 13.698% |
| └ 在家食品 Food at home | 8.325% |
| └ 外食 Food away from home | 5.373% |
| 能源 Energy | 6.383% |
| └ 能源商品 Energy commodities | 3.120% |
| 　 └ 汽油 Gasoline | 2.895% |
| └ 能源服務 Energy services | 3.262% |
| 核心：扣除食品與能源 | 79.919% |
| └ 核心商品 | 19.176% |
| └ 扣除能源的服務 | 60.744% |
| 居住服務 Shelter（服務子項） | 35.625% |
| └ 主要住宅租金 | 7.840% |
| └ 屋主設算租金 OER of residences | 26.204% |
| 醫療服務 | 6.935% |
| 交通服務 | 6.315% |

細項公布到小數三位，可能出現 0.001 百分點的四捨五入加總差異。食品不包含酒精飲料；食品與飲料則包含。OER 是住宅提供的居住服務估計租金，不是房價或房貸利息。資料來源同上。

## 三頁分析及證據強度

### 1. 與市場預期有哪些落差

| 指標 | 前值 | 本次公布 | 比較預期 | 差異 |
|---|---:|---:|---:|---:|
| 整體月增 | 0.4% | 0.6% | 0.6% | 0.0 百分點 |
| 整體年增 | 3.4% | 3.7% | 3.6% | +0.1 百分點 |
| 核心月增 | 0.3% | 0.3% | 0.2% | +0.1 百分點 |
| 核心年增 | 2.4% | 2.6% | 2.5%* | +0.1 百分點 |

實際值以 [BLS 新聞稿](https://www.bls.gov/news.release/cpi.nr0.htm) 為準，並與 [BLS 分類圖表](https://www.bls.gov/charts/consumer-price-index/consumer-price-index-by-category.htm) 的年增率、[Reuters 報導](https://www.marketscreener.com/news/us-consumer-prices-accelerate-in-september-on-costlier-gasoline-core-cpi-firmer-ce785dd2df88f027) 交叉核對。

整體月增及年增預期來自 [Reuters 市場反應報導](https://www.investing.com/news/economic-indicators/hot-september-cpi-sends-ratehike-bets-soaring-4949438)；核心月增預期來自上述 Reuters 主報導。

*核心年增預期 2.5% 來自 [ETF.net 轉述 CNBC](https://etf.net/news/september-cpi-is-the-last-inflation-reading-before-the-fed-meets-2026-10-14)，與課堂資料一致；CNBC 原頁本次讀取失敗，因此僅完成二手來源與課堂資料比對，未完成原始調查直接驗證。ETF.net 同時列出 FactSet 核心年增預期為 2.4%、整體月增預期為 0.5%。不同調查不是同一套共識，簡報已加註，不將 2.5% 誤稱為 Reuters 預測。

核心月增沒有出現預期中的降溫，是較清楚的意外。年增與月增的季調口徑及四捨五入不同，整體月增符合預期、年增高於預期可以同時成立。

### 2. 落差的主要可能原因

汽油是本次總體上漲的主要來源；但整體月增本來就預期偏高，不能把汽油實現漲幅直接等同預測誤差。居住服務與其他商品、服務共同支撐核心，與核心降溫不如預期的方向一致。Reuters 的分項解讀與 BLS 敘述相符。

我們沒有取得市場對每個細項的發布前預測，所以無法嚴格分解「核心 +0.1 百分點預測誤差」各自來自哪一項。此處是實現值構成與可能機制分析，不是已識別的因果估計。

課堂 OCR 將 OER 與 Shelter 混用；已依官方權重表修正。能源向運輸、食品的成本傳導屬可能機制，不能僅憑一個月 CPI 證明完整因果關係。

### 3. 對下個月 CPI 的影響

若油價漲幅回落，總體月增可能放緩；若油價持平，直接能源增量減弱，核心的居住及服務項目更重要；若油價繼續上漲，則存在直接推升與後續成本轉嫁風險。這些是條件情境，未設定機率，也未建立數值預測模型。

年增率還受去年同月基期影響。課堂提到的 3.6%–3.8% 區間、固定 1–2 個月傳導時滯缺少可重現模型或足夠證據，因此未沿用。原油現貨、零售汽油與 BLS 季調汽油指數的變化不應直接互換。

市場解讀：核心持續偏強可能支撐較高利率並壓抑估值；能源單獨回落未必代表全面降溫。聯準會通膨目標對應 PCE，CPI 不可直接視為同一指標。下次發布時間取自 BLS 公告。

