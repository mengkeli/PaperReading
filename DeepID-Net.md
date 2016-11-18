## DeepID-Net: multi-stage and deformable deep convolutiona l neural networks for object detection ##

- by 李孟珂

---
**Abstract**
针对目标检测问题，提出了一种多级的、可变形的深度卷积神经网络。
用几何上的约束和惩罚来建立一个池化层模型
多种分类器被结合起来处理不同难度的分类问题
提出一种新的预训练方法，使得在目标检测问题上具有更高的泛化能力

**Introduction**
在目标问题检测上最大的挑战是外观、光照、背景和变形。
第一，选取最有区分度的特征，如SIFT,HOG等特征
第二，处理目标部分的变形
第三，由分类器决定哪一个窗口中的内容被检测为一个封闭目标，如SVM、随机森林等

在DeepID-Net中，主要研究一下三点：
1. 对于l特征表达
