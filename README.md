## Neural network on unstructured health data analysis ##

要求：
- 神经网络分析非结构化数据（包括文献和医生的诊断病例，疾病和用药）
- 以及在图形、声音以及其他表型结合（包括可微神经网络DNC的应用）

---

##文献阅读
查阅的均为英文文献，在原文引用的同时给出中文翻译。

1. 
- **data description:** 
    1. small, round blue-cell tumors (SRBCTs)
    小圆蓝细胞肿瘤
    2. These cancers belong to four distinct diagnostic categories and often present diagnostic dilemmas in clinical practice
    这些癌症属于四个不同的诊断类别和经常在临床实践中存在诊断困境
- **purpose:** develop a method of classifying cancers to specific diagnostic categories based on their gene expression signatures using artificial neural networks(ANNs)
- **methods:**
- **conclusion:** 1. demonstrates the potential applications of these methods for tumor diagnosis and the identification of candidate targets for therapy. 展示了潜在的应用这些方法对肿瘤诊断和治疗候选目标的识别。

2. 
- **data description:** 
- **purpose:** develop a method of improving the ANN's ability to represent variables and data structures and to store data over long timescales
- **methods:** differentiable neural computer (DNC)
- **conclusion:** DNCs have the capacity to solve complex, structured tasks that are inaccessible to neural networks without external read–write memory
 DNC有能力解决复杂的、结构化的任务，并且不需要外部读写内存
3. 
- **data description:** 
- **purpose:** develop a method of improving the ANN's ability to represent variables and data structures and to store data over long timescales
- **methods:** differentiable neural computer (DNC)
- **conclusion:** DNCs have the capacity to solve complex, structured tasks that are inaccessible to neural networks without external read–write memory
 DNC有能力解决复杂的、结构化的任务，并且不需要外部读写内存


---
##参考文献
1. Classification and diagnostic prediction of cancers using gene expression profiling and artificial neural networks
Javed Khan1, 2, 7, Jun S. Wei1, 7, Markus Ringnér1, 3, 7, Lao H. Saal1, Marc Ladanyi4, Frank Westermann5, Frank Berthold6, Manfred Schwab5, Cristina R. Antonescu4, Carsten Peterson3 & Paul S. Meltzer1

2. Hybrid computing using a neural network with dynamic external memory
Alex Graves,    Greg Wayne,	Malcolm Reynolds,	Tim Harley,	Ivo Danihelka,	Agnieszka Grabska-Barwińska,	Sergio Gómez Colmenarejo,	Edward Grefenstette,	Tiago Ramalho,	John Agapiou,	Adrià Puigdomènech Badia,	Karl Moritz Hermann,	Yori Zwols,	Georg Ostrovski,	Adam Cain,	Helen King,	Christopher Summerfield,	Phil Blunsom,	Koray Kavukcuoglu	& Demis Hassabis

3. Graves, A. Generating sequences with recurrent neural networks. Preprint at http://arxiv.org/abs/1308.0850 (2013) 
4. 
4. Hinton, Geoffrey, Vinyals, Oriol, and Dean, Jeff. Distilling the knowledge in a neural network.
arXiv preprint arXiv:1503.02531, 2015

5. Krizhevsky, Alex, Sutskever, Ilya, and Hinton, Geoffrey E. Imagenet classification with deep convolutional neural networks. In Advances in neural information processing systems, pp. 1097–1105, 2012
6. 
6. Mnih, Volodymyr, Kavukcuoglu, Koray, Silver, David, Rusu, Andrei A, Veness, Joel, Bellemare, Marc G, Graves, Alex, Riedmiller, Martin, Fidjeland, Andreas K, Ostrovski, Georg, et al. 
Human-level control through deep reinforcement learning.Nature, 518(7540):529–533, 2015

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

11. Sutskever, I., Vinyals, O. & Le, Q. V. Sequence to sequence learning with neural networks. 
In Advances in Neural Information Processing Systems Vol. 27 (eds Ghahramani, Z. et al.) 3104–3112 (Curran Associates, 2014) 
