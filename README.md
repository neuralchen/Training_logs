# Training_logs
 
# Mobilenet V2

### Mobilenet V2 Setting:

- batch size: 4 * 64
- epochs: 150
- LR decay strategy cosine, 5 epochs warm up, initial learning rate 0.05
- weight decay 0.00004
- 0.1 label smoothing
- ImageNet

### MobileNetV2 with a spectrum of width multipliers
| Architecture      | # Parameters | MFLOPs | Top-1 / Top-5 Accuracy (%) |
| ----------------- | ------------ | ------ | -------------------------- |
| MobileNetV2 1.0 | 3.504M | 300.79 | 72.192 / 90.534 |
| MobileNetV2 1.0 (retrain) | 3.504M | 300.79 | 72.252 / 90.622 |
| MobileNetV2 1.0 Depth Embedding | 3.504M | 300.79 | 72.652 / 90.578 |
| MobileNetV2 0.75 | 2.636M | 209.08 | 69.952 / 88.986 |
| MobileNetV2 0.75 Depth Embedding | 2.636M | 209.08 | 70.164 / 89.054 |
| MobileNetV2 0.5 | 1.968M | 97.14 | 64.592 / 85.392 |
| MobileNetV2 0.5 Depth Embedding | 1.968M | 97.14 | 65.74 / 86.004 |
| MobileNetV2 0.35 | 1.677M |     59.29 | 60.092 / 82.172  |
| MobileNetV2 0.35 Depth Embedding | 1.677M |     59.29 | 62.470 / 83.828  |
| MobileNetV2 0.25 | 1.519M |     37.21 | 52.352 / 75.932  |
| MobileNetV2 0.1 | 1.356M | 12.92 | 34.896 / 56.564 |
| MobileNetV2 0.1 Depth Embedding | 1.356M | 12.92 | 43.772 / 67.946 |
| MobileNetV2 0.1 Depth Embedding (第一层加入宽度乘子) | 1.356M | 12.92 | 42.396 / 66.592 |
# ResNet

### ResNet Setting:

- batch size: 4 * 64
- epochs: 100
- LR decay strategy cosine, 5 epochs warm up, initial learning rate 0.1
- weight decay 1e-4
- 0.1 label smoothing
- ImageNet


### ResNet
| Architecture      | # Parameters | GFLOPs | Top-1 / Top-5 Accuracy (%) |
| ----------------- | ------------ | ------ | -------------------------- |
| Resnet50 | 25.56 M | 4.12 G | 75.20 / 92.52 |
| Resnet50 Depth Embedding | 25.56 M | 4.12 G | - / - |
| Resnet34 | 21.80 M | 3.68 G | 73.31 / 91.40 |
| Resnet34 Depth Embedding | 21.80 M | 3.68 G | 74.620 / 92.122 |
