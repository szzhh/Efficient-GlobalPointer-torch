## Efficient GlobalPointer：少点参数，多点效果

### 介绍

基于 GlobalPointer 的改进，[Keras 版本](https://spaces.ac.cn/archives/8877) 的 torch 复现，核心还是 token-pair 。

### 数据集

[CMeEE](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414) 存放在:
train_cme_path = ./datasets/CME/train.json

eval_cme_path = ./datasets/CME/dev.json

### 预训练模型

1、RoBerta系列 [RoBERTa-zh-Large-PyTorch](https://github.com/brightmart/roberta_zh)

2、点这里直接[goole drive](https://drive.google.com/file/d/1yK_P8VhWZtdgzaG0gJ3zUGOKWODitKXZ/view)下载

### 运行

注意把train/predict文件中的 bert_model_path 路径改为你自己的

#### train

```python
python train_CME.py
```

#### predict

```
python predict_CME.py
```

### 效果

![image-20230301122008694](https://raw.githubusercontent.com/szzhh/cloudimg/main/picgo/image-20230301122008694.png)

