# Product-co-purchasing-graph
The best model is Spec+MLP+CS.


#### Detailed Hyperparameter:

```python
Namespace(device=0, dropout=0.5, epochs=200, hidden_channels=512, lr=0.01, num_layers=3, runs=10, use_cached=True, use_embed=True)

num_layers = 3
hidden_dim = 512
dropout = 0.5
lr = 0.01
runs = 10
epochs = 200
num_correction_layers = 50
correction_alpha = 1.0
num_smoothing_layers = 50
smoothing_alpha = 0.8
scale = 15.
A1 = 'DAD'
A2 = 'DA'
```

#### Result:

```bash
Train: 0.9452, Val: 0.9127, Test: 0.8405
All runs:
Highest Train: 94.57 ± 0.04
Highest Valid: 91.24 ± 0.04
  Final Train: 94.57 ± 0.04
   Final Test: 84.10 ± 0.06
```

| Model                | Test Accuracy   | Valid Accuracy  | Parameters |
| -------------------- | --------------- | --------------- | ---------- |
| Spec+MLP+C&S         | 0.8410 ± 0.0006 | 0.9124 ± 0.0004 | 340527     |
