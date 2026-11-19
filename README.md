# Project 1 NumPy 图像编码器

本项目是 Python 程序设计课程的 Project 1，主要包括 NumPy 基础练习和图像编码器前向计算两部分。

图像编码器使用教师提供的固定模型参数，不进行训练。程序将输入图像转换为 512 维单位向量，主要练习数组变形、广播、矩阵乘法、多头注意力和 Transformer 的基本计算过程。

## 项目内容

- `numpy_homework.py`：8 道基础题和 4 道中等题。
- `image_encoder.py`：使用 NumPy 完成图像编码器中的 TODO。
- `preprocess_image.py`：图像缩放、裁剪和归一化。
- `run.py`：运行图像编码器。
- `check.py`：课程提供的检查程序。
- `report/`：实验报告及 LaTeX 源文件。
- `results/`：本地运行结果。

`helpers.py`、`preprocess_image.py`、`runtime.py`、`run.py`、`check.py`、配置文件和模型参数由课程提供。本项目主要完成 `numpy_homework.py` 和 `image_encoder.py` 中要求的内容。

## 环境安装

建议使用 Python 3.9 或更高版本。

```bash
python -m pip install -r requirements.txt
```

## NumPy 练习

运行：

```bash
python numpy_homework.py
```

程序会依次输出 12 道练习题的计算结果，并进行部分边界情况检查。

## 图像编码器
## 实现内容

图像编码器中完成的主要步骤包括：

1. 将图像划分为 49 个 patch；
2. 将特征拆分为多个 attention head；
3. 计算 scaled dot-product attention；
4. 完成 Transformer block 的残差连接和 MLP；
5. 加入 CLS token 与位置编码；
6. 生成并归一化最终图像向量。

## 运行情况

本地测试中，编码器能够处理单张图片和多张图片组成的 batch，最终输出向量长度接近 1。NumPy 练习可以从第一题完整运行到最后一题。


## 作者

- 姓名：王斯怡
- 学号：2025681039
- 专业：人工智能
- 学院：人工智能学院

## 说明

本项目仅用于课程学习。模型权重、测试资源和课程提供的框架代码不作为个人原创内容上传或声明。
