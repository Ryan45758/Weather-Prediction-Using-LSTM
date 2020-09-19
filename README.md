# Weather-Prediction
### 目的:分析台中市龍井區近8年來天氣資料，來預測龍井區未來天氣
### 步驟:<br>
手動蒐集CSV檔 → 匯入資料 → 合併資料 → 資料前處理 <br>
→ 匯出資料 → 切分資料 → 載入模型 → 訓練模型 <br>
→ 保存模型 → 觀看準確度 → 畫圖 → 修正與改善。<br>
### 1. 蒐集資料:From https://e-service.cwb.gov.tw/HistoryDataQuery/index.jsp 下載台中市龍井區近8年來天氣資料<br>
![](https://i.ibb.co/qdxVjqV/1.png)<br>
### 2. 下載完後，遍歷所有檔案並新增我們所需的特徵，春夏秋冬<br>
![](https://i.ibb.co/x7PmJd3/2020-09-19-135516.png)
### 3. 最後將所有資料合併成一個檔案Weather.csv<br>
### 4. 接著對資料進行前處理，刪除不要的特徵，因為很多欄位為空，因該觀測站無安裝該欄位所需sensor故無資料<br>
