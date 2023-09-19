## Modelling Experiments

| Model | Dataset | Processing | Model Parameters | No. of Epochs | Metric | Score | Inference Time |
| ------ |----------|-------------------|------------|-------------|-----------|------------|-----------|
| Vanilla ConvNet | FER 2013 | None | ~10 million| 60 | Val Accuracy | 0.764 | NA | ~2000 sec |
| LSTM | FER 2013 | Rescaling, Resize, Load&Label | 140,679 | 50 | Test(Val) Accuracy | 0.431 | NA |
| LSTM with RNN | FER 2013 | Rescaling, Resize, Load&Label | ~3.8 million | 50 | Test(Val) Accuracy | 0.358 | NA |
| LSTM with CNN | FER 2013 | Rescaling, Resize, Load&Label | ~3.7 million | 50 | Test(Val) Accuracy | 0.586 | NA | 
