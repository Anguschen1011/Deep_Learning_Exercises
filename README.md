#### 資訊工程學系(1121)
# 1121_人工智慧導論(B4CS020017A)
### Python 深度學習
---
透過深度學習判斷圖片人物是否為 Santa
---
經過測試，在Google Colab中執行此訓練的系統 RAM可接受的圖片大小為256\*256，所以在讀取圖片後在256*256的空白畫布貼上依照比例縮放的.jpg圖片。

之後，將縮放後的資料 reshape 成四維張量並進行正規化，並將y_Train和y_Test進行 One-Hot 編碼。接著，建立 Sequential 模型並加入卷積層、池化層、Dropout 和全連接層，將kernel_size改為(3, 3)和model.add(Dense())改為(2, activation='softmax')。

最後，在訓練模型train_history = model.fit()中，調整以下參數validation_split=0.15, epochs=20, batch_size=32, verbose=1。

- expand.ipynb for epoch = 20
- expand(50).ipynb for epoch = 50




