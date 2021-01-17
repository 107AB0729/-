# 資財三乙 107AB0729 林暐偵 期末報告
# CH8

# 步驟

1.執行 run_complete_detector.sh\
2.利用SKlearn的RandomForestClassifier以及FeatureHasher提取特徵\
3.以機器學習方式訓練提取特徵\
4.用預測出來的scores和test_y辨別是惡意或善意的檔案\
5.繪製ROC curve的圖

# 結果
！[ image ]（https://github.com/107AB0723/final/blob/main/Curve.png）\
利用隨機森林決策樹model提取特徵的惡意軟件，\
再用接收器操作特徵（ROC）曲線測量的是檢測器的真實陽性率（成功檢測到的惡意檔案的百分比）\
和錯誤陽性率（被錯誤標記為惡意檔案的善意檔案的百分比）的變化。\
當靈敏度設定越高得到的假陽性(被錯誤標記為惡意檔案的善意檔案)越多，但會提高檢測率 ;\
而當靈敏度設定越低，則檢測的正確率(成功檢測到的惡意檔案)越高。
