##Research on health data visualization##

- by 李孟珂

---
#### 数据可视化意义
现代的数据可视化（Data visualization）技术指的是运用计算机图形学和图像处理技术，将数据转换为图形或图像在屏幕上显示出来，并进行交互处理的理论、方法和技术。
随着网络和电子商务的发展，信息可视化（Information visualization）也被提出，不仅能用图像来显示多维的非空间数据，使用户加深对数据含义的理解，而且用直观形象的图像来指引检索过程，加快检索速度。
随着可视化技术的不断发展，数据可视化与信息可视化的分界已越来越不明显。

---
#### Review of Literature
1. 交互式高维数据可视化
提出一个基本的三步交互式数据可视化的数据分析任务：找到完形、提出查询、并进行比较。这些任务支持交互式视图操作三个类:聚焦,连接,和安排视图。
并详细介绍了一个多元数据可视化的系统--XGobi。这个介绍不全面,但强调XGobi工具集中的例子,链接,和安排视图;即高维预测,与散点图刷,和矩阵的条件图。
主要讨论的是由高维投影形成的一个极其重要的XGobi的一部分。着重关注渐近的插图常态的高维投影(Diaconis定理和弗里德曼),使用可视化的阶乘的高维数据集实验,和交互地生成矩阵方法与高维投影条件。

2. 数据挖掘蚁群优化算法 【2002】
本文提出了一种数据挖掘算法称为Ant-Miner(基于蚁群的数据挖掘)。Ant-Miner的目标就是从数据中提取分类规则。算法是基于真实蚁群的行为研究和一些数据挖掘的概念和原则。我们比较Ant-Miner和CN2的性能,一个众所周知的数据挖掘分类算法,在六个公共领域数据集。结果表明:1)Ant-Miner对预测的准确性可以与CN2匹敌,2)由Ant-Miner发现的规则列表相比于由CN2发现的更简单。

3. 信息可视化和可视化数据挖掘 【2002】
可视化数据挖掘的优点是用户直接参与数据挖掘过程。有大量的信息可视化技术已经在过去的十年里支持大型数据集的挖掘。在本文中,我们提出一个基于数据类型可视化的分类信息可视化，可视化数据挖掘技术,可视化技术,交互和变形技术。

4. 可视化技术挖掘大型数据库
在本文中,我们描述和评估一个新的基于可视化的挖掘大型数据库的方法。主要思想是通过将每个数据值映射到一个像素并准备充分的像素，把可能多的数据项展示在屏幕上。
本文的主要目的是评估所提出的可视化数据挖掘技术，比较其他著名的多维数据可视化技术:平行坐标可视化技术模式。在评估数据可视化挖掘技术时，感知数据属性是最重要的，CPU时间和二级存储访问的数量只是次要的。

5. 从可视化数据探索到可视化数据挖掘 【2003】
我们调查工作的不同使用图形化映射和交互技术的可视化数据挖掘大数据集表示为表数据。基本术语与数据挖掘、数据集,和可视化。以前的工作,综述了信息可视化技术和系统的不同分类。讨论了交互技术的作用,除了工作解决问题的选择和评估可视化技术。我们回顾一些代表作的使用信息可视化技术在挖掘数据的上下文中。这包括可视化数据探索和可视化表达具体的挖掘算法的结果。我们还审查最近的创新方法,试图将可视化集成到DM / KDD过程,用它来提高用户交互和理解。

6. 集群的自组织映射 【2000】
自组织映射(self-organizing map SOM)是在数据挖掘的探索性阶段的一个很好的工具。它把输入空间映射到低维正则网格原型，可以被有效地利用与可视化和探索数据属性。当SOM单元的数量大,便于定量分析地图和数据,类似的单元需要分组,即,集群。在本文中,研究了不同的SOM聚类方法。两级过程优先(The two-stage procedure-first)使用SOM来生产原型,然后在第二层聚类，结果发现,比直接聚类数据减少计算时间。

7. 树形图:一个空间层次信息结构的可视化方法 【1991】
描述了一种可视化分层结构化信息的方法。树形图100%利用可用的显示空间,把完整的层次结构映射到一个矩形区域空间。有效的利用空间可以允许非常大的层次结构的显示，促进语义信息的表示。树形图可以描述两个层次结构的结构和内容。然而,方法是最适合用于当叶节点的内容和层次结构是最重要的,并且内容与内部节点相关信息在很大程度上是来自他们的子节点的情况下。

8. Show Me:自动演示进行视觉分析 【2007】
这篇文章介绍Show Me,一个集成的用户界面命令,自动演示合并到一个商业视觉分析系统，叫Tableau。Tableau的一个关键方面是VizQL语言,用于指定视图,扩展自动演示的生成表的视图(通常称为小多个显示)。商业应用的一个关键研究问题在于自动演示的用户体验,它必须支持的流动可视化分析。先前的研究的重点没有提及用户体验。Show Me的用户体验包括自动选择标记类型，向视图中添加单个field，以及构建多个fields。虽然这些功能是可选的，但是log显示ShowMe正在被商业用户使用。

9. 北极星:系统的查询、分析和可视化的多维关系数据库 【2002】
在过去几年里,大型多维数据库已成为常见的各种应用,如数据仓库和科学计算。
因为数据集的大小,密集的图形表示比电子表格和图表更有效。
此外,必须能够让分析师能快速变化视图,因为他们的一个工作周期，必须先提出假设,然后实验。
在本文中,提出的北极星,扩展了著名的数据透视表借口,来探索大型多维数据库。
创新点包括构建基于图形显示的视觉规范和生成一个精确的关系查询的能力。
视觉规范可以迅速并逐步发展,进行结构复杂的查询和可视化，给分析师视觉反馈。

10. 数据可视化 【1993】书
这本书教你:七个阶段的数据可视化——获取、解析、过滤、挖掘、展示、精炼、交互。
---
#### references

[1] Interactive High-Dimensional Data Visualization
Andreas Buja , Dianne Cook & Deborah F. Swayne Research Scientist 

[2] Data mining with an ant colony optimization algorithm
R.S. Parpinelli, H.S. Lopes, A.A. Freitas

[3] Information visualization and visual data mining
D.A. Keim. 

[4] A brief history of data visualization
Michael Friendly

[5] From visual data exploration to visual data mining: a survey
M.C. Ferreira de Oliveira, H. Levkowitz

[6] Clustering of the self-organizing map
 Juha Vesanto, Esa Alhoniemi
 
[7] Tree-maps: a space-filling approach to the visualization of hierarchical information structures
 Brian Johnson, Ben Shneiderman
 
[8] Show Me: Automatic Presentation for Visual Analysis
 Jock D. Mackinlay, Pat Hanrahan, Chris Stolte
 
[9] Polaris: a system for query, analysis, and visualization of multidimensional relational databases
 Chris Stolte, Diane Tang, Pat Hanrahan

[10] Visualizing Data
William S. Cleveland
