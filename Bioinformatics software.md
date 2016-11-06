## Bioinformatics software ##

要求：
- 研究生物信息学所需要的数据库和工作软件

简介：
- 生物信息（bioinformatics）中的“信息（-informatics）”指的是从海量的数据中进行挖掘，从而得到知识的过程。在这个过程中，会涉及到数据的管理，数据的运算，数据挖掘和建模仿真。其中，数据管理部分主要是数据库（database），数据的运算部分主要是指各种生物信息的软件（software tools）。

---

###数据库
1. Classification and diagnostic prediction of cancers using gene expression profiling and artificial neural networks
- **data description:** 
    1. small, round blue-cell tumors (SRBCTs)
    小圆蓝细胞肿瘤
    2. These cancers belong to four distinct diagnostic categories and often present diagnostic dilemmas in clinical practice
    这些癌症属于四个不同的诊断类别和经常在临床实践中存在诊断困境
- **main idea:** develop a method of classifying cancers to specific diagnostic categories based on their gene expression signatures using artificial neural networks(ANNs)
- **methods:**
- **conclusion:** 1. demonstrates the potential applications of these methods for tumor diagnosis and the identification of candidate targets for therapy.
展示了潜在的应用这些方法对肿瘤诊断和治疗候选目标的识别。

2. Hybrid computing using a neural network with dynamic external memory
- **data description:** 
- **main idea:** develop a method of improving the ANN's ability to represent variables and data structures and to store data over long timescales
- **methods:** differentiable neural computer (DNC)
- **conclusion:** DNCs have the capacity to solve complex, structured tasks that are inaccessible to neural networks without external read–write memory
 DNC有能力解决复杂的、结构化的任务，并且不需要外部读写内存

3. Generating sequences with recurrent neural networks 递归神经网络生成序列
- **data description:** 
    1. 《华尔街日报》语料库潘树图资料库的部分
    2. 100 百万字节的完整的英文维基百科数据
- **main idea:** shows how Long Short-term Memory recurrent neural networks can be used to generate complex sequences with long-range structure, simply by predicting one data point at a time.  长短期记忆的神经网络可以仅仅通过预测一个数据点来生成复杂的序列与远程结构。最后实现的系统可以生成高度真实的草书笔迹。
- **methods:** standard RNNs are unable to store information of past inputs for a very long time.采用了LSTM，并且用堆叠LSTM定义了一个deep RNN。
- **conclusion:** 

4. **Distilling the knowledge in a neural network**
- **data description:** MINST dataset
- **main idea:** to compress the knowledge in an ensemble into a single model which is much easier to deploy and we develop this approach further using a different compression technique.
用已有的整体神经网络太庞大，计算量大，本文提出了一种压缩神经网络的方法，把神经网络中多个模型精炼为单模型。
Unlike a mixture of experts, these specialist models can be trained rapidly and in parallel.
并且这些特殊的单模型可以快速的、并行的训练。
- **methods:**

5. Imagenet classification with deep convolutional neural networks
- **data description:**  classify the 1.3 million high-resolution images in the LSVRC-2010 ImageNet training set into the 1000 different classes
- **main idea:** 训练大型深度卷积神经网络对大量高分辨率图像进行分类
- **methods:** The neural network, which has 60 million parameters and 650,000 neurons, consists of five convolutional layers, some of which are followed by max-pooling layers, and three fully-connected layers with a final 1000-way softmax. To make training faster, we used non-saturating neurons and a very efficient GPU implementation of the convolution operation. 
该神经网络由六千万个参数和六十五万个神经元，包括五个卷积层，并连接一个最大池化层和三个全连接层。在加速训练方面，采用非饱和神经元和GPU运算。采用"dropout"方法来降低过拟合。

6. Human-level control through deep reinforcement learning
- **data description:**
- **main idea:**
- **methods:**

7. On the number of linear regions of deep neural networks. 
- **data description:**
- **main idea:**
- **methods:**

---
###参考文献
1. Classification and diagnostic prediction of cancers using gene expression profiling and artificial neural networks
Javed Khan1, 2, 7, Jun S. Wei1, 7, Markus Ringnér1, 3, 7, Lao H. Saal1, Marc Ladanyi4, Frank Westermann5, Frank Berthold6, Manfred Schwab5, Cristina R. Antonescu4, Carsten Peterson3 & Paul S. Meltzer1

2. Hybrid computing using a neural network with dynamic external memory
Alex Graves,    Greg Wayne,	Malcolm Reynolds,	Tim Harley,	Ivo Danihelka,	Agnieszka Grabska Barwińska,	Sergio Gómez Colmenarejo,	Edward Grefenstette,	Tiago Ramalho,	John Agapiou,	Adrià Puigdomènech Badia,	Karl Moritz Hermann,	Yori Zwols,	Georg Ostrovski,	Adam Cain,	Helen King,	Christopher Summerfield,	Phil Blunsom,	Koray Kavukcuoglu	& Demis Hassabis

3. Graves, A. Generating sequences with recurrent neural networks. Preprint at http://arxiv.org/abs/1308.0850 (2013) 

4. Hinton, Geoffrey, Vinyals, Oriol, and Dean, Jeff. Distilling the knowledge in a neural network.
arXiv preprint arXiv:1503.02531, 2015

5. Krizhevsky, Alex, Sutskever, Ilya, and Hinton, Geoffrey E. 
Imagenet classification with deep convolutional neural networks. 
In Advances in neural information processing systems, pp. 1097–1105, 2012
 
6. A framework for the forensic investigation of unstructured email relationship data
Towards a New Science of a Clinical Data Intelligence
Adaptive Visualization of Dynamic Unstructured Meshes
Quality of information for quality of life: Healthcare big data analytics
Finding Structured and Unstructured \ud Features to Improve the Search Result of \ud Complex Question
Information Accountability of Healthcare Big Data


7. Montufar, Guido F, Pascanu, Razvan, Cho, Kyunghyun, and Bengio, Yoshua.
On the number of linear regions of deep neural networks. 
In Advances in neural information processing systems, pp. 2924–2932, 2014

8. Simonyan, Karen and Zisserman, Andrew.
Very deep convolutional networks for large-scale image recognition.
arXiv preprint arXiv:1409.1556, 2014.

9. Silver, David, Huang, Aja, Maddison, Chris J, Guez, Arthur, Sifre, Laurent, van den Driessche, George, Schrittwieser, Julian, Antonoglou, Ioannis, Panneershelvam, Veda, Lanctot, Marc, et al. Mastering the game of go with deep neural networks and tree search.
Nature,529(7587):484–489, 2016.

10. Deep biomarkers of human aging: Application of deep neural networks to biomarker development
Evgeny Putin 1, 2 , Polina Mamoshina 1, 3 , Alexander Aliper 1 , Mikhail Korzinkin 1 , Alexey Moskalev 1, 4 , Alexey Kolosov 5 , Alexander Ostrovskiy 5 , Charles Cantor 6 , Jan Vijg 7 , Alex Zhavoronkov 1, 3

11. Sutskever, I., Vinyals, O. & Le, Q. V.
Sequence to sequence learning with neural networks. 
In Advances in Neural Information Processing Systems Vol. 27 (eds Ghahramani, Z. et al.) 3104–3112 (Curran Associates, 2014) 

12. Bottou, L. From machine learning to machine reasoning.
Mach. Learn. 94, 133–149 (2014) 

13. Graves, A., Wayne, G. & Danihelka, I. 
Neural Turing machines.
Preprint at http://arxiv.org/abs/1410.5401 (2014) 

14. Bahdanau, D., Cho, K. & Bengio, Y.
Neural machine translation by jointly learning to align and translate.
Preprint at http://arxiv.org/abs/1409.0473 (2014)  

15. Lake, B. M., Salakhutdinov, R. & Tenenbaum, J. B. 
Human-level concept learning through probabilistic program induction.
Science 350, 1332–1338 (2015) 

16. Rezende, D. J., Mohamed, S., Danihelka, I., Gregor, K. & Wierstra, D.  
One-shot generalization in deep generative models. 
In Proc. 33nd International Conference on Machine Learning (eds Balcan, M. F. & Weinberger, K. Q.) 1521–1529 (JMLR, 2016) 

17. Daumé, H. III, Langford, J. & Marcu, D. Search-based structured prediction.
Mach. Learn. 75, 297–325 (2009) 
