## Research on Bioinformatics Software ##

要求：
- 研究生物信息学所需要的数据库和**工作软件**

---
### 简介
- 生物信息（bioinformatics）中的“信息（-informatics）”指的是从海量的数据中进行挖掘，从而得到知识的过程。在这个过程中，会涉及到数据的管理，数据的运算，数据挖掘和建模仿真。其中，数据管理部分主要是数据库（database），数据的运算部分主要是指各种生物信息的软件（software tools）。
- 根据不同的特点，可以把这些资源分成不同的类别。比如根据数据性质可以将database分为原始数据（Original data）数据库和二级数据（Secondary data）数据库。再比如根据软件是独立的工具还是网络服务器，可以将software tools分为standalone programs和web servers。 根据发布者的类别可以分为centralized resources和individual resources。
- ![bioinformatics architecture][1]

### 知识背景
- 计算机基础（linux+perl+R 或者 python+matlab）
- 生信基础知识（测序+数据库+数据格式）
- 生信研究领域（全基因组，全转录组，全外显子组，捕获目标区域测序）
- 生信应用领域（肿瘤筛查，产前诊断，流行病学，个性化医疗）

---
### 数据库
三大主流数据库：
- NCBI（National Center for Biotechnology Information）
- EBI（European Bioinformatics Institute）
- UCSC（University of California Santa Cruz）Genome Browser

---
### 常用软件
1. 多序列分析
序列对齐（sequence alignment）的目的是通过两个或多个核酸序列或蛋白质序列进行对齐，并将其中相似的结构区域突出显示。通过比较未知序列与已知序列（尤其是功能和结构已知的序列）之间的同源性，往往可以很容易地预测未知序列的功能。
- ClustalW/X
最为著名的序列多重对齐软件包。用户可自行下载进行数据分析。接受多种输入格式，包括FASTA、EMBL、SWISS-PROT、PIR、GCG/MSF等，但所有输入序列必须在同一文件中。如果输入序列中的非空格号85%以上为A、C、G、T、U、N，判定为核酸序列，否则作为蛋白质序列计算。但核酸和蛋白质序列不能在同一文件中。

- Match-Box
同时考虑序列数据和氨基酸性质进行序列多重对齐分析。

2. 系谱分析:临床上判断单基因病的遗传方式常用系谱分析法。系谱 (pedigree)或称家图是指对某遗传病患者家族各成员的发病情况进行详细调查，再以特定的符号和格式绘制成反映家族各成员相互关系和发病情况的图解。是遗传风险分析、连锁分析和 产前诊断 中必不可少的工具。 
- PAUP
它包括距离矩阵、不变量和极大似然方法和许多指标和统计检验。一般被用来计算后验概率分裂和拓扑树的距离。
- GCG package
是一个有超过130个程序的完整软件包,可以操作和分析核酸、蛋白质序列。它具有以下功能：
    1. 比较。比较两个或多个序列。创建、编辑、显示和分析多重序列比对。
    2. 数据库搜索和检索。核酸或蛋白质序列数据库搜索序列类似于查询序列或序列模式。
    3. DNA / RNA二级结构。预测和显示最优和次优的DNA或RNA二级结构。
    4. 编辑和出版。从数字化仪输入序列或键盘和编辑它们。
    5. 进化。确定和显示来自多个序列比对的进化发展史。
    6. 片段组装。管理和组装核苷酸序列片段的测序项目。
    7. 基因的发现和模式识别。识别终端、重复、蛋白质编码区,和其他共识模式。
    8. HMMER(隐马尔可夫模型)。创建一个概要文件隐马尔可夫模型(HMM)代表相关序列的相似性和使用模型数据库搜索、序列比对,或生成随机序列。
    9. 映射。计算和显示限制消化和模拟RNA指纹。
    10. 引物预测。预测最佳引物PCR（聚合酶链）反应。
    11. 蛋白质分析。识别序列在蛋白质序列和预测肽隔离。
    12. 翻译。核酸翻译成蛋白质和向后翻译蛋白质成核酸

- MEGA/METREE
是计算机软件进行统计分析分子进化,构建系统发育树。

- GAMBIT

- MacClade

- ClustalX

- MEGA

3. 基因结构预测分析
- GENSCAN
旨在可基因组序列中预测完整的基因结构,包括外显子、内含子、启动子和聚腺苷酸化信号。它不同于大多数现有的基因发现算法,它允许部分基因以及成套基因和多基因的发生在一个序列,在一种或两种DNA链。程序版本适用于脊椎动物,线虫(实验),玉米和拟南芥序列目前可用。脊椎动物版本在果蝇序列的效果相当好。序列可以在网站提交,GENSCAN网站是斯坦福大学。

- GeneFinder

- Gene Feature Searches

- Grail

- GrailEXP

- GeneMark
是一个在细菌的DNA序列寻找基因的系统。该算法是基于5阶非齐次马尔可夫链,它是用于定位流感嗜血杆菌的完整基因组中的基因、尿道支原体、和其他几个完整的基因组。
网站包括文档和一个可以提交序列的Web界面。这个系统是在亚特兰大,乔治亚理工学院。

- Veil

- AAT

- GENEID
http://www.imim.es/GeneIdentification/Geneid/geneid_input.html
Genlang
http://cbil.humgen.upenn.edu/~sdong/genlang_home.html
GeneParser
http://beagle.colorado.edu/~eesnyder/GeneParser.html

- Glimmer
是一个使用插值马尔可夫模型(IMMs)来识别微生物的DNA编码区域的系统。IMMs是马尔可夫模型的泛化,允许以极大的灵活性的选择“背景”,即：有多少之前的基组将会被用于预测下一个基组。Glimmer一直在完整基因组流感嗜血杆菌、大肠杆菌、幽门螺旋杆菌,尿道支原体和其他基因组上进行测试,结果到目前为止已经证明它是高度准确的。
完整的系统,包括源代码,都可以从这个网站获得。

- Procrustes
http://www-hto.usc.edu/software/procrustes/

4. 基因分类
GO Annotator

5. 蛋白质结构预测分析
Expasy
http://www.expasy.ch/
CBS
http://www.cbs.dtu.dk
Predicting protein secondary structure
http://dot.imgen.bcm.tmc.edu:9331/pssprediction/pssp.html
Predicting protein 3D Structures
- Predicting protein structures

6. 进化树分析
- Phylip是最通用的进化树分析软件。主要包括以下几个方面的功能软件：
    1. DNA和蛋白质序列数据的分析软件
    2. 序列数据转变成距离数据后，对距离数据分析的软件
    3. 对基因频率和连续的元素分析的软件
    4. 把序列的每个碱基/氨基酸独立看待（碱基/氨基酸只有0和1的状态）时，对序列进行分析的软件
    5. 按照DOLLO简约性算法对序列进行分析的软件
    6. 绘制和修改进化树的软件。 

- PUZZLE 核酸序列、蛋白序列相似性分析及进化树构建工具。根据序列数据的最大相似性构建进化树，一个软件，并且对树进行bootstrap评估。可对大量数据进行快速分析构建，程序还包含数个统计测试。 

7. 其它分析工具和软件
Putative DNA Sequencing Errors Check
http://www.bork.embl-heidelberg.de/Frame/
MatInspector
http://www.gsf.de/cgi-bin/matsearch.pl
FastM
http://www.gsf.de/cgi-bin/fastm.pl
Web Signal Scan
http://www.dna.affrc.go.jp/htdocs/sigscan/signal.html
BCM Search Launcher
http://dot.imgen.bcm.tmc.edu:9331/seq-util/seq-util.html
Webcutter
http://www.firstmarket.com/cutter/cut2.html
Translate DNA to protein
http://www.expasy.ch/tools/dna.html
ABIM
http://www-biol.univ-mrs.fr/english/logligne.html
sequence motifs:
Pfam
http://www.sanger.ac.uk/Pfam/
http://pfam.wustl.edu/
ProDom
http://protein.toulouse.inra.fr/prodom.html
PRINTS
http://www.biochem.ucl.ac.uk/bsm/dbbrowser/PRINTS/

---
### 参考文献
本文研究主要来源于维基百科、谷歌学术，以及斯坦福大学、华盛顿大学等软件官网。

  [1]: images/2016-11-06-12-4434686be90434f7b697227a427d2716_r.jpg.png "4434686be90434f7b697227a427d2716_r.jpg.png"
