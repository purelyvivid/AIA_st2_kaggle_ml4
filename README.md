# AIA_taiwan_southern_2nd
臺灣人工智慧學校(AIA)南部分校技術班第二期

## Kaggle 競賽 - 透過training data預測最後30筆外匯收盤價
https://www.kaggle.com/c/aia-st2-forex-predict-overview

### DL framework
Tensorflow 2.0

### Data 
~70000筆訓練資料
預測30筆接下來的收盤表現

### Metric
MSE Error of 收盤價('Close')

### Method & Result
1. LSTM, mse_error: ~0.0006
2. 1dCNN, mse_error: ~0.0010
3. Seq2Seq, mse_error: ~0.0012

### Remark
- 簡單起見, 三種方法都只用了收盤價('Close'), 但不代表其他欄位沒有參考價值
- 雖然LSTM錯誤率最低, 但不代表最適合用來預測股市, 只是此資料集剛好如此而已
- Seq2Seq模型太過複雜, 不適合此任務, 只是寫來當作tf2練習


