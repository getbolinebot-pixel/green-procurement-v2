# 綠色採購 V2 新網頁｜完整重新部署包

## 目的
這是一個獨立新版本，可部署成第二個網址，保留原本舊版網址不動。

建議命名：
- GitHub repository：green-procurement-v2
- Vercel project：green-procurement-v2

## Google Sheet 自動同步
目前已設定：
https://opensheet.elk.sh/1e7FELtxhGBKPZ4RJxgcG_KbV_qGTxKs_/Sheet1

Google Sheet 第一列欄位請用：
category, amount, note

也可用中文欄位：
品項, 金額, 備註

## 燈號邏輯
扣除「高鐵交通 / 高鐵」後：
- 低於 100,000：紅燈
- 100,000 ~ 249,999：黃燈
- 250,000 以上：綠燈
- 另顯示距年度 400,000 目標差距

## 部署新網頁
1. GitHub 建立新 repository：green-procurement-v2
2. 上傳本資料夾全部檔案
3. Vercel → Add New → Project
4. 選 green-procurement-v2
5. Deploy

完成後，原本 green-procurement.vercel.app 仍會保留。
