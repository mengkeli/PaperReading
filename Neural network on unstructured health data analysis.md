## Neural network on unstructured health data analysis ##

要求：
- 神经网络分析非结构化数据（包括文献和医生的诊断病例，疾病和用药）
- 以及在图形、声音以及其他表型结合（包括可微神经网络DNC的应用）

---
### 背景介绍
---
![unstructred vs structured data][1]


###文献阅读
---
查阅的均为英文文献，给出部分中文翻译，重要文献加粗显示。
1. An integrated data preparation scheme for neural network data analysis
2. 
- **data description:**
- **main idea:**
- **methods:**






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

7. 
- **data description:**
- **main idea:**
- **methods:**

8. Very deep convolutional networks for large-scale image recognition.
- **data description:**
- **main idea:** we investigate the effect of the convolutional n
etwork depth on its accuracy in the large-scale image recognition setting.  Our main contribution is a thorough evaluation of networks of increasing depth using an architecture with very small (3×3) convolution filters, which shows that a significant improvement on the  prior-art configurations can  be  achieved by  pushing the  depth to  16–19 weight layers.
本文研究了在大数据量的图像识别上，卷积网络的深度对识别准确度的影响。 主要用3×3的卷积滤波器，通过增加网络深度来对识别进行彻底的评估。
- **methods:**

9. A Framework for the Forensic Investigation of Unstructured Email Relationship Data
- **data description:** 邮件
- **main idea:** 提出了一种新颖的框架来帮助司法调查非结构化的电子邮件数据。（主要在于分析该邮件与其他邮件的交流网络）。非结构化数据更为复杂,因为它包含的信息一个社交网络,如人际关系, 识别关键的节点和权力关系, 目前没有标准化的工具来进行调查分析。
- **methods:**  社交网络分析、数据可视化，

10. A Graph-based Approach for Semantic Data Mining 基于图的语义数据挖掘
- **data description:**
- **main idea:** 首先,开发一个信息集成解决方案基于metaheuristic优化时需要访问的数据挖掘任务异构数据源。其次,我描述的图形界面领域知识和数据结构可以采用RDF模型和它的图形表示。最后,我描述几个图理论分析方法挖掘相结合的信息来源。
- **methods:**

11. Information Accountability of Healthcare Big Data 
- **data description:**
- **main idea:**
- **methods:**

12.
- **data description:**
- **main idea:**
- **methods:**


14. Neural machine translation by jointly learning to align and translate
- **data description:** English-French平行语料:Europarl(61M),新闻评论(5.5M)、联合国(421M)和两个爬取的语料分别为90M和272.5M, 共计850M。
- **purpose:**  提高现有机器翻译的准确性
- **methods:** 
    1. the previous experience is to encode a source  sentence  into  a  fixed-length  vector  from  which  a  decoder  generates  a translation. now we extend this by allowing a model to automatically(soft) search for parts of a source sentence that are relevant to predicting a target word, without forming these parts as a hard segment.
The most important distinguishing feature of this approach from the basic encoder–decoder is that
it does not attempt to encode a whole input sentence into a single fixed-length vector. Instead, it en-codes the input sentence into a sequence of vectors and chooses a subset of these vectors adaptively while decoding the translation.  explicitly. 在机器翻译的时候，以往的经验是，把源语言编码成一个定长的向量，再由解码器解码成翻译的文字。新方法是不需要硬编码成定长的向量，而是选取源语言的部分，形成一个向量序列，使用其中的序列中的子集来预测目标词汇。
    2. 训练了两个模型：RNN Encoder-Decoder 和 论文提出的新方法。
    3. 

- **conclusion:** 该方法在英译法的翻译中，比现有的基于短语的翻译器表现出色，尤其是在长句子的翻译上。

- 
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


  [1]: 


  [1]: images/2016-11-08-11-Firefox_Screenshot_2016-11-08T08-11-35.482Z.png "Firefox_Screenshot_2016-11-08T08-11-35.482Z.png"
