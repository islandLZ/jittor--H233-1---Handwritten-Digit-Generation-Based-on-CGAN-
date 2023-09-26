# Jittor 第三届计图挑战赛热身赛 CGAN

![主要结果](./result.png)

在数字图片数据集 MNIST 上训练 Conditional GAN（Conditional generative adversarial nets）模型，通过输入一个随机向量 z 和额外的辅助信息 y (如类别标签)，生成特定数字的图像。

## 简介
本项目包含了第三届计图挑战赛热身赛 - 手写数字生成比赛的代码实现。本项目的特点是：要训练一个将随机噪声和类别标签映射为数字图片的Conditiona1GAN模型，并生成比赛官方给定用户随机ID对应的数字图片结果。

## 安装 
本项目可在 1 张 4000 上运行。

#### 运行环境
- windows11
- python >= 3.7
- jittor >= 1.3.0

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
预训练模型模型下载地址为[预训练模型](https://pan.baidu.com/s/1UTLMjmZZZZ5WwRbzj6veNA?pwd=0jeg)，提取码：0jeg，下载后放入目录 `./weights/` 下。

## 数据预处理
无

## 训练
单卡训练可运行以下命令：
```
python CGAN.py
```

## 推理
把./CGAN.py文件里面的“模型训练”部分注释掉，再运行以下命令：
```
python CGAN.py
```

## 致谢

此项目基于论文[CGAN:](./ConditionGAN.pdf) *Conditional Generative Adversarial Nets* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。
