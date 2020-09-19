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
### 4. 因為很多欄位為空，因該觀測站無安裝該欄位所需sensor故無資料<br>
![](https://i.ibb.co/pZb0xq4/2020-09-19-140452.png)
### 5. 接著對資料進行前處理，刪除不需要的特徵<br>
![](https://i.ibb.co/GVjJ8Fn/2020-09-19-140835.png)
### 6. 移除缺失值
![](https://i.ibb.co/gJz04Fr/2020-09-19-141020.png)
### 7. 擴增資料特徵，將資料擴增為當天的前七天資料，並移除缺失值
![](https://i.ibb.co/MkvjbyQ/2020-09-19-141148.png)
### 8.將資料切分為訓練資料與測試資料，前13行為測試資料13行之後為預測訓練資料
![](https://i.ibb.co/0Jc81vy/2020-09-19-141524.png)
