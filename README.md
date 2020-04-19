# IoT_Fire-Safety (爐此安全)
## 概念
使用Flag's Block拼圖式的編譯程式來撰寫，當使用者在燉煮東西時，系統透過紅外線感測器去判斷爐前是否有人，溫度感測器判斷溫度是否過高，並利用燈光閃爍、警示聲來吸引使用者的注意。
## 電路圖
### 紅外線感測器: 偵測爐前是否有人
### 溫溼度感測器: 感測爐火溫度
### LED燈: 照明設備
### 蜂鳴器: 警報器
### LCD螢幕: 顯示溫度和警示訊息
![image](https://github.com/Chun-Ching/IoT_Fire-Safety/blob/master/%E7%88%90%E6%AD%A4%E5%AE%89%E5%85%A8%E9%9B%BB%E8%B7%AF%E5%9C%96.PNG)
## 程式碼
一開始先設定變數，每秒在LCD第一列顯示出偵測到的溫度，紅外線感應器有偵測到人，LED燈會正常發光，LCD第二列顯示SAFE，如果超過10秒沒有偵測到，LED燈開始閃爍。溫度感測過高，LCD第二列顯示WARNING，蜂鳴器發出警示聲。

![image](https://github.com/Chun-Ching/IoT_Fire-Safety/blob/master/%E7%88%90%E6%AD%A4%E5%AE%89%E5%85%A8code.PNG)
