# Shopee-Tracker
此專案利用爬蟲概念爬取指定蝦皮商家之所有商品庫存並輸出。

## 需求
- Python >= 3.9

## 使用方式

開啟 `main.py` 並修改 `shopid` 至指定商家之 id，

以 [海底撈官方旗艦店](https://shopee.tw/shop/237300461) 為例子。

到賣場網頁複製網頁網址之shopid `https://shopee.tw/shop/237300461`  ->  `237300461`

修改完成後執行以下

```
python3 main.py
```

## DEMO

以[海底撈官方旗艦店](https://shopee.tw/shop/237300461) 為例子之輸出。

```
賣場總商品數: 40
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【多種口味湯底】 四川麻辣火鍋 限量下殺優惠
當前折扣| 4.4
子商品  | 番茄湯底有效期至2022/9/21     | 價格   98.0$ | 庫存 156
子商品  | 酸辣番茄湯底4入贈送麻辣魚皮1包| 價格  389.0$ | 庫存 91
子商品  | 清油湯底有效期至2022/11/23    | 價格   98.0$ | 庫存 150
子商品  | 麻辣香鍋-筷手小廚效期2023/1/23| 價格   98.0$ | 庫存 174
子商品  | 菌湯湯底 3入有效期至2022/9/12 | 價格  199.0$ | 庫存 76
子商品  | 清湯湯底 3入有效期至2022/8/23 | 價格  199.0$ | 庫存 85
子商品  | 清油湯底 3入有效期2022/11/23  | 價格  270.0$ | 庫存 76
子商品  | 清油湯底4入贈送麻辣魚皮1包    | 價格  389.0$ | 庫存 83
子商品  | 菌湯湯底有效期至2022/9/12     | 價格   98.0$ | 庫存 192
子商品  | 番茄+清油+清湯+上湯三鮮湯底送魚皮1包| 價格  389.0$ | 庫存 91
子商品  | 清湯湯底4入贈送麻辣魚皮1包    | 價格  389.0$ | 庫存 95
子商品  | 上湯三鮮湯底4入贈送麻辣魚皮1包| 價格  389.0$ | 庫存 90
子商品  | 菌湯湯底4入贈送麻辣魚皮1包    | 價格  389.0$ | 庫存 97
子商品  | 清油湯底+清湯湯底+菌湯湯底    | 價格  270.0$ | 庫存 92
子商品  | 麻辣香鍋(筷手小廚)4入贈送麻辣魚皮1包| 價格  389.0$ | 庫存 84
子商品  | 酸辣番茄+清湯+菌湯+麻辣香鍋送魚皮1包| 價格  389.0$ | 庫存 94
子商品  | 酸辣番茄湯底有效期至2022/10/26| 價格   98.0$ | 庫存 192
子商品  | 清湯湯底有效期至2022/8/23     | 價格   98.0$ | 庫存 173
子商品  | 番茄湯底4入贈送麻辣魚皮1包    | 價格  389.0$ | 庫存 83
子商品  | 上湯三鮮湯底有效期至2022/10/26| 價格   98.0$ | 庫存 179
子商品  | 超便宜限搶價(口味隨機)        | 價格  150.0$ | 庫存  0
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【酸辣牛肉冬粉/番茄牛肉冬粉/什錦冬粉（酸辣）】 即沖即食 懶人必備
當前折扣| 5
子商品  | 超便宜限搶價 (口味隨機)       | 價格  150.0$ | 庫存  0
子商品  | 酸辣牛肉冬粉有效期至2022/9/6  | 價格   85.0$ | 庫存 248
子商品  | 番茄牛肉冬粉有效期至2022/11/5 | 價格   85.0$ | 庫存 244
子商品  | 什錦冬粉-酸辣有效期2022/12/25 | 價格   75.0$ | 庫存 218
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【香辣粉】 四川麻辣火鍋 海底撈特製蘸料
當前折扣| 6.4
子商品  |                               | 價格  109.0$ | 庫存 130
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【自煮火鍋（麻辣嫩牛/番茄牛肉）】買三送一（贈送麻辣魚皮一包）
當前折扣| 6.3
子商品  | 麻辣嫩牛自煮鍋*2盒 2022/11/5  | 價格  370.0$ | 庫存 129
子商品  | 番茄嫩牛自煮鍋*2盒 2022/11/4  | 價格  370.0$ | 庫存 119
子商品  | 麻辣嫩牛/番茄嫩牛*各1         | 價格  370.0$ | 庫存 39
子商品  | 麻辣嫩牛自煮鍋有效期至2022/11/5| 價格  189.0$ | 庫存 212
子商品  | 番茄嫩牛自煮鍋有效期至2022/11/4| 價格  189.0$ | 庫存 179
子商品  | 超便宜限搶價 (口味隨機)       | 價格  300.0$ | 庫存  0
子商品  | 麻辣嫩牛自煮鍋*3盒買三送一（贈送魚皮）| 價格  569.0$ | 庫存 168
子商品  | 番茄嫩牛自煮鍋*3盒買三送一（贈送魚皮）| 價格  569.0$ | 庫存 133
----------------------------------------------------------------------------------------------------
商品    | 海底撈【麻辣魚皮/番茄蝦餅/麻辣蝦薯條】 嘎嘣脆~美味獨家 限時買五送一
當前折扣| 5
子商品  | 麻辣蝦薯條有效期至2023/6/10   | 價格   79.0$ | 庫存 41
子商品  | 麻辣魚皮有效期至2022/10/11    | 價格   79.0$ | 庫存 328
子商品  | 超便宜限搶價 (口味隨機)       | 價格  159.0$ | 庫存  0
子商品  | 番茄蝦餅（買五送一）贈送魚皮一包| 價格  380.0$ | 庫存 71
子商品  | 麻辣蝦薯條（買五送一）贈送魚皮一包| 價格  380.0$ | 庫存  0
子商品  | 麻辣魚皮（買五送一）贈送魚皮一包| 價格  380.0$ | 庫存 211
子商品  | 番茄蝦餅有效期至2023/3/21     | 價格   79.0$ | 庫存 432
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【原味/香辣沾醬】  四川麻辣火鍋 海底撈特色菜醬料【滿額免運快速到貨】
當前折扣| 4.7
子商品  | 原味沾醬 效期至2022/09/08     | 價格   32.0$ | 庫存 10
子商品  | 香辣沾醬 效期至2022/09/08     | 價格   32.0$ | 庫存 34
----------------------------------------------------------------------------------------------------
商品    | 海底撈  椒麻青豆花生  特色小吃 （單包）
當前折扣| 7.7
子商品  |                               | 價格   30.0$ | 庫存 282
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【麻辣血旺煲/番茄蔬菜煲/火腿豚骨煲/酸菜白肉煲】 料理簡單 廚房必備~
當前折扣| 6.3
子商品  | 火腿豚骨煲有效期至2023/2/28   | 價格  300.0$ | 庫存 179
子商品  | 麻辣血旺煲有效期至2023/2/23   | 價格  300.0$ | 庫存 94
子商品  | 番茄蔬菜煲 有效期至2022/9/3   | 價格  300.0$ | 庫存  0
子商品  | 麻辣血旺煲*4包效期至2023/2/23 | 價格  756.0$ | 庫存 90
子商品  | 番茄蔬菜煲*4包效期至2022/9/3  | 價格 1200.0$ | 庫存  0
子商品  | 酸菜白肉煲有效期至2023/3/6    | 價格  300.0$ | 庫存 150
子商品  | 火腿豚骨煲*4包效期至2023/2/28 | 價格  756.0$ | 庫存 100
子商品  | 酸菜白肉煲*4包效期至2023/3/6  | 價格  756.0$ | 庫存 90
----------------------------------------------------------------------------------------------------
商品    | 海底撈【豆皮】火鍋料【滿額免運快速到貨】
當前折扣| 9.2
子商品  |                               | 價格   36.0$ | 庫存 70
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【酸辣牛肉冬粉/番茄牛肉冬粉/酸辣什錦冬粉  12入裝】 買六杯送一包麻辣魚皮
當前折扣| 5.9
子商品  | 酸辣牛肉冬粉買六送一（贈送魚皮一包）| 價格  499.0$ | 庫存 227
子商品  | 番茄牛肉冬粉買六送一（贈送魚皮一包）| 價格  499.0$ | 庫存 197
子商品  | 酸辣什錦冬粉2022/12/25（箱）    | 價格  890.0$ | 庫存 470
子商品  | 酸辣牛肉冬粉2022/09/06（箱）    | 價格  990.0$ | 庫存 460
子商品  | 番茄牛肉冬粉2022/11/05（箱）    | 價格  990.0$ | 庫存 436
子商品  | 什錦酸辣冬粉買六送一（贈送魚皮一包）| 價格  499.0$ | 庫存 457
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【自煮火鍋套餐（麻辣嫩牛/番茄牛肉）】
當前折扣| 6.3
子商品  | 麻辣嫩牛自煮鍋有效期至2022/11/5| 價格  189.0$ | 庫存 219
子商品  | 番茄嫩牛自煮鍋有效期至2022/11/4| 價格  189.0$ | 庫存 50
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【撈派巴沙魚片】四川火鍋 海底撈特色菜【滿額免運快速到貨】
當前折扣| 8
子商品  |                               | 價格  144.0$ | 庫存 72
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【上湯三鮮湯底】 四川麻辣火鍋 海底撈特製湯底【滿額免運快速到貨】
當前折扣| 6.5
子商品  |                               | 價格   98.0$ | 庫存 48
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【芝士蝦丸】 四川麻辣火鍋 海底撈特色菜 【滿額免運快速到貨】
當前折扣| 7.1
子商品  |                               | 價格   99.0$ | 庫存 33
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【蝦皮限定超值福箱】 選擇組合種類多《下單即送麻辣魚皮》
當前折扣| 5.2
子商品  | 番茄湯底x1,麻辣嫩牛自煮鍋x1+番茄牛肉冬粉x2| 價格  388.0$ | 庫存 107
子商品  | 麻辣香鍋x1,麻辣嫩牛自煮鍋x1+酸辣牛肉冬粉x2| 價格  388.0$ | 庫存 99
子商品  | 清湯湯底x1,麻辣嫩牛自煮鍋x1+番茄牛肉冬粉x2| 價格  388.0$ | 庫存 117
子商品  | 上湯三鮮湯底x1,麻辣嫩牛自煮鍋x1+番茄牛肉冬粉x2| 價格  388.0$ | 庫存 109
子商品  | 番茄湯底x1,麻辣嫩牛自煮鍋x1+酸辣牛肉冬粉x2| 價格  388.0$ | 庫存 117
子商品  | 番茄湯底x1,麻辣自煮鍋x1+牛肉冬粉(酸辣番茄各1)| 價格  388.0$ | 庫存 107
子商品  | 麻辣香鍋x1,麻辣自煮鍋x1+牛肉冬粉(酸辣番茄各1)| 價格  388.0$ | 庫存 96
子商品  | 菌湯湯底x1,麻辣嫩牛自煮鍋x1+酸辣牛肉冬粉x2| 價格  388.0$ | 庫存 112
子商品  | 菌湯湯底x1,麻辣嫩牛自煮鍋x1+番茄牛肉冬粉x2| 價格  388.0$ | 庫存 116
子商品  | 菌湯湯底x1,麻辣自煮鍋x1+牛肉冬粉(酸辣番茄各1)| 價格  388.0$ | 庫存 113
子商品  | 清湯湯底x1,麻辣自煮鍋x1+牛肉冬粉(酸辣番茄各1)| 價格  388.0$ | 庫存 116
子商品  | 清湯湯底x1,麻辣嫩牛自煮鍋x1+酸辣牛肉冬粉x2| 價格  388.0$ | 庫存 112
子商品  | 麻辣香鍋x1,麻辣嫩牛自煮鍋x1+番茄牛肉冬粉x2| 價格  388.0$ | 庫存 111
子商品  | 上湯三鮮湯底x1,麻辣嫩牛自煮鍋x1+酸辣牛肉冬粉x2| 價格  388.0$ | 庫存 115
子商品  | 上湯三鮮湯底x1,麻辣自煮鍋x1+牛肉冬粉(酸辣番茄各1)| 價格  388.0$ | 庫存 96
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【撈派滑牛肉】 四川火鍋 海底撈特色菜【滿額免運快速到貨】
當前折扣| 7.6
子商品  | 件                            | 價格  168.0$ | 庫存 363
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【清油湯底】 四川麻辣火鍋 海底撈火鍋湯底【滿額免運快速到貨】
當前折扣| 6.5
子商品  |                               | 價格   98.0$ | 庫存 54
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【番茄鍋底 】四川麻辣火鍋 火鍋湯底
當前折扣| 6.6
子商品  |                               | 價格   99.0$ | 庫存 31
----------------------------------------------------------------------------------------------------
商品    | 海底撈【爆漿起司牛丸/麻辣牛丸】任選8入裝 蝦皮吃貨節獨家
當前折扣| 5.6
子商品  | 爆漿起司牛丸                  | 價格  169.0$ | 庫存 54
子商品  | 麻辣牛丸                      | 價格  169.0$ | 庫存 91
----------------------------------------------------------------------------------------------------
商品    | 筷手小廚 【宮保雞丁/魚香肉絲/麻婆豆腐】美味即時調理
當前折扣| 5.4
子商品  | 麻婆豆腐 有效期至2022/9/6     | 價格   38.0$ | 庫存  4
子商品  | 宮保雞丁 有效期至2022/9/6     | 價格   70.0$ | 庫存  0
子商品  | 魚香肉絲 有效期至2022/9/6     | 價格   38.0$ | 庫存 10
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【秘製去骨雞腿肉】 四川火鍋 海底撈特色菜 【滿額免運快速到貨】
當前折扣| 7.2
子商品  |                               | 價格  129.0$ | 庫存 114
----------------------------------------------------------------------------------------------------
商品    | 海底撈【川味/原味小酥肉】特色菜【滿額免運快速到貨】
當前折扣| 9.1
子商品  | 川味小酥肉                    | 價格  108.0$ | 庫存 158
子商品  | 原味小酥肉                    | 價格  119.0$ | 庫存 96
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【熔岩蝦球】 四川麻辣火鍋 海底撈炸物小吃【滿額免運快速到貨】
當前折扣| 7.9
子商品  |                               | 價格  118.0$ | 庫存 25
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【菌湯湯底】 四川麻辣火鍋 海底撈特製湯底【滿額免運快速到貨】有效期至2022/9/12
當前折扣| 4.5
子商品  |                               | 價格   68.0$ | 庫存 87
----------------------------------------------------------------------------------------------------
商品    | 海底撈  椒麻青豆花生  （組合裝）
當前折扣| 9
子商品  | 椒麻青豆花生5包組             | 價格  158.0$ | 庫存 140
子商品  | 椒麻青豆花生10包組（買十送一）  | 價格  315.0$ | 庫存 82
----------------------------------------------------------------------------------------------------
商品    | 海底撈【鈴鈴捲】火鍋料【滿額免運快速到貨】
當前折扣| 7.4
子商品  |                               | 價格   95.0$ | 庫存  3
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【清湯湯底(110g/包)】有效期至2022/8/23
當前折扣| 4.5
子商品  |                               | 價格   68.0$ | 庫存 143
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【燕麥雙椒/紅蔥黃豆】拌飯醬~即食即用
當前折扣| 5.3
子商品  | 燕麥雙椒-拌飯醬有效期至2022/9/5| 價格   80.0$ | 庫存 42
子商品  | 紅蔥黃豆-拌飯醬有效期至2022/9/4| 價格   80.0$ | 庫存 123
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【底料禮盒】 四川麻辣火鍋 海底撈火鍋湯底【6件組】
當前折扣| 6.7
子商品  |                               | 價格  599.0$ | 庫存 96
----------------------------------------------------------------------------------------------------
商品    | 海底撈【半殼扇貝】海鮮【滿額免運快速到貨】
當前折扣| 8
子商品  |                               | 價格  168.0$ | 庫存 10
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【黑糖芝士珍珠/楊枝甘露】冰沙~即飲甜品（6入組）
當前折扣| 8.5
子商品  | 黑糖芝士珍珠冰沙(六入組)      | 價格  390.0$ | 庫存 286
子商品  | 楊枝甘露冰沙(六入組)          | 價格  390.0$ | 庫存 243
----------------------------------------------------------------------------------------------------
商品    | 海底撈【番茄蝦餅】美味獨家
當前折扣| 6.1
子商品  |                               | 價格   79.0$ | 庫存 153
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【酸辣什錦冬粉】 懶人即食
當前折扣| 5.4
子商品  |                               | 價格   79.0$ | 庫存 170
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【精裝-麻辣清油火鍋】四川麻辣火鍋 火鍋湯底
當前折扣| 3.9
子商品  |                               | 價格   98.0$ | 庫存 26
----------------------------------------------------------------------------------------------------
商品    | 【海底撈】麻辣血旺寬粉
當前折扣| 5.8
子商品  |                               | 價格  145.0$ | 庫存 749
----------------------------------------------------------------------------------------------------
商品    | 【海底撈】麻辣乾拌麵
當前折扣| 6.6
子商品  |                               | 價格  166.0$ | 庫存 1029
----------------------------------------------------------------------------------------------------
商品    | 海底撈 【麻辣水煮魚調味料】四川麻辣 水煮美味
當前折扣| 6.3
子商品  |                               | 價格   98.0$ | 庫存 63
----------------------------------------------------------------------------------------------------
商品    | 【海底撈】麻辣小龍蝦900g
當前折扣| 6
子商品  |                               | 價格  399.0$ | 庫存 411
----------------------------------------------------------------------------------------------------
商品    | 海底撈超值組合【中元澎湃箱】
當前折扣| 6.7
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 97
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 98
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 95
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 95
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 98
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 98
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 96
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,番茄自煮鍋+紅蔥黃豆拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 99
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 99
子商品  | 清湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 99
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 98
子商品  | 清油湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 番茄湯底1+蝦薯條1+魚皮1+血旺寬粉1,番茄自煮鍋+紅蔥黃豆拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 100
子商品  | 上湯三鮮湯底+蝦薯條+魚皮+血旺寬粉,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 99
子商品  | 麻辣香鍋1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+番茄牛肉粉2| 價格  666.0$ | 庫存 100
子商品  | 菌湯湯底1+蝦薯條1+魚皮1+血旺寬粉1,麻辣自煮鍋+燕麥雙椒拌飯醬+酸辣番茄各1| 價格  666.0$ | 庫存 99
----------------------------------------------------------------------------------------------------
商品    | 《下單即送麻辣魚皮》海底撈 【限定超值福袋】 選擇組合種類多
當前折扣| 6.1
子商品  | 什錦酸辣冬粉,番茄牛肉自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,番茄牛肉自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,番茄底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,菌湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,麻辣香鍋底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,清油底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,上湯三鮮底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,番茄牛肉自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,清湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,清湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,菌湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,麻辣香鍋底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 199
子商品  | 酸辣牛肉冬粉,清油底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,菌湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,香辣粉*1+番茄蝦餅*2| 價格  369.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,麻辣香鍋底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,麻辣嫩牛自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 199
子商品  | 酸辣牛肉冬粉,菌湯底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,清湯底料**2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,上湯三鮮底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,香辣粉*1+番茄蝦餅*2| 價格  369.0$ | 庫存 199
子商品  | 番茄牛肉冬粉,菌湯底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,精裝清油1+水煮魚1+酸辣番茄1+花生6| 價格  499.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,清油底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,上湯三鮮底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,麻辣香鍋底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,清湯底料**2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,麻辣嫩牛自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,麻辣香鍋底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,菌湯底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,清油底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,上湯三鮮底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,精裝清油1+水煮魚1+酸辣番茄1+花生6| 價格  499.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,番茄底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,麻辣嫩牛自煮鍋*1+麻辣蝦薯條*2| 價格  479.0$ | 庫存 199
子商品  | 什錦酸辣冬粉,清油底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,清湯底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,番茄底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,番茄底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,精裝清油1+水煮魚1+酸辣番茄1+花生6| 價格  499.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,上湯三鮮底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,清油底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,香辣粉*1+番茄蝦餅*2| 價格  369.0$ | 庫存 198
子商品  | 番茄牛肉冬粉,番茄底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,上湯三鮮底料*2+紅蔥黃豆拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 什錦酸辣冬粉,清湯底料**2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 酸辣牛肉冬粉,番茄底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
子商品  | 番茄牛肉冬粉,麻辣香鍋底料*2+燕麥雙椒拌飯醬*2| 價格  539.0$ | 庫存 200
```
