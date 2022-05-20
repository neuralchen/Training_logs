# Training_logs
 
##Mobilenet V2

#Setting:

- batch size: 4 * 64
- epoch: 150
- LR decay strategy cosine 5 epoch warmup
- weight decay 0.00004
- 0.1 lable smoothing

### MobileNetV2 with a spectrum of width multipliers
| Architecture      | # Parameters | MFLOPs | Top-1 / Top-5 Accuracy (%) |
| ----------------- | ------------ | ------ | -------------------------- |
| MobileNetV2 1.0 | 3.504M | 300.79 | 72.192 / 90.534 |
| MobileNetV2 1.0 (retrain) | 3.504M | 300.79 | 72.252 / 90.622 |
| MobileNetV2 1.0 Depth Embedding | 3.504M | 300.79 | 72.652 / 90.578 |
| MobileNetV2 0.75 | 2.636M | 209.08 | 69.952 / 88.986 |
| MobileNetV2 0.5 | 1.968M | 97.14 | 64.592 / 85.392 |
| MobileNetV2 0.5 Depth Embedding | 1.968M | 97.14 | 64.592 / 85.392 |
| MobileNetV2 0.35 | 1.677M |     59.29 | 60.092 / 82.172  |
| MobileNetV2 0.35 Depth Embedding | 1.677M |     59.29 | 62.470 / 83.828  |
| MobileNetV2 0.25 | 1.519M |     37.21 | 52.352 / 75.932  |
| MobileNetV2 0.1 | 1.356M | 12.92 | 34.896 / 56.564 |