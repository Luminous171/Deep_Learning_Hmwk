# Deep_Learning_Hmwk

Part of this assignment is learning to test and refine models. As such the following three questions were analyzed:

1) What was the lowest loss model?
2) Which model displayed the best accuracy tracking?
3) How was the window size determined?

#### Question 1 and 2

The model with both the lowest loss and best accuracy tracking was the closing price predictor [closing price](https://github.com/Luminous171/Deep_Learning_Hmwk/blob/main/Starter_Code/lstm_stock_predictor_closing.ipynb). In addition to the loss metric calculated by Tensorflow, the supplemental measure of mean squared error was calculated to determine the best accuracy tracking.

| Final Model with 100 Epochs |             |      |     |            |
| --------------------------- | ----------- | ---- | --- | ---------- |
| Indicator                   | Window Size | Loss | MSE | Batch Size |
| Price                       | 3           | 2.4% |         329,765,409 | 5 |
| FNG                         | 3           | 4.3% |     1,265,817,273 | 5 |



#### Question 3

To determine the best window size. The model was run multiple times holding constant all other parameters except for window size. The best results was a window size of 3.

| Window Size | Loss | MSE                 |
| ----------- | ---- | ------------------- |
| 1           | 5.0% |         902,580,900 |
| 2           | 3.4% |         726,318,427 |
| 3           | 2.4% |         329,765,409 |
| 4           | 2.5% |         504,123,047 |
| 5           | 2.6% |         547,440,813 |
| 6           | 2.9% |         684,339,092 |
| 10          | 2.9% |         655,312,756 |

