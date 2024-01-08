> **Note**
>
> 仅供个人学习参考，请勿用于其他行为

# <div align=center width="40"> 国科大 生物信息学期末考试题及参考答案（个人复习用）</div>
# 1. 什么是生物信息学？如何理解生物信息学的含义？
> 1. 英文解释：Genome informatics is a scientific discipline that encompasses all aspects of genome information acquisition, processing, storage, distribution, analysis, and interpretation.<br>**它是一个学科领域，包含着基因组信息的获取、处理、存储、分配 、分析和解释的所有方面。**
> 2. 生物信息学是把基因组DNA序列信息分析作为源头，破译隐藏在DNA序列中的遗传语言，特别是非编码区的实质；同时在发现了新基因信息之后进行蛋白质空间结构模拟和预测。
> 3. 生物信息学的研究目标是揭示“基因组信息结构的复杂性及遗传语言的根本规律”。它是当今世纪自然科学和技术科学领域中“基因组、“信息结构”和“复杂性”这三个重大科学问题的有机结合。
>
> 怎么理解：
>
>  

# 2. 发现新基因的两种方法是什么？算法的本质是什么？
> **1. 通过大规模基因测序，查找具有编码特征的序列**
> 
> 从大规模基因组测序得到的数据出发，使用不同数据方法，进行标识、查找和预测，并将找到的可能的新基因同数据库中已有的基因对比，从而确定是否为新基因。
> 
> 可分为：
  - 基于信号，如剪切位点、序列中的启动子与终止子等。
  - 基于组分，即基因家族、特殊序列间比较，Complexity analysis，Neural Network
>
>  本质：
>
> 

> **2. 利用EST数据库发现新基因并进行拼接组装**
> 
> 当测序获得一条EST序列时，它来自哪一个基因的哪个区域是未知的（随机的），所以属于同一个基因的不同EST序列之间常有交叠的区域。根据这种“交叠”现象，就能找出属于同一个基因的所有EST序列，进而将它们拼接成和完整基因相对应的全长cDNA序列。而到目前为止，公共EST数据库(dbEST)中已经收集到约800万条的人的EST序列。估计这些序列已覆盖了人类全部基因的95%以上，平均起来每个基因有10倍以上的覆盖率。
> 

# 3. 利用蛋白质或核酸序列数据库进行生物进化研究的主要步骤是什么？在这一领域当前存在的重要困难是什么？有何解决途径？
> **1. 计算步骤**
>  - **序列相似性比较：** 待研究序列与DNA或蛋白质序列库进行比较，用于确定该序列的生物属性，也就是找出与此序列相似的已知序列是什么。完成这一工作只需要使用两两序列比较算法。常用分析有BLAST等；
>  - **序列同源性分析：** 待研究序列加入到一组与之同源，但来自不同物种的序列中进行多序列同时比较，以确定该序列与其它序列间的同源性大小。这是理论分析方法中最关键的一步。完成这一工作必须使用多序列比较算法。常用的程序包有CLUSTAL等；
>  - **构建系统进化树：** 一般单独一种方法是不够的，通常需要多种方法才能构建反映物种间进化关系的进化树。根据序列同源性分析的结果，重建反映物种间进化关系的进化树。为完成这一工作已发展了多种软件包，例如PYLIP、MEGA等；
>  - **稳定性检验（分支的确定）：** 只有稳定的分支才有意义，为了检验构建好的进化树的可靠性，通常构建过程要随机成百上千次，大概率（70%以上）出现的分支点才是可靠的，通用的方法使用 Bootstrap算法，相应的软件已包括在构建系统进化树所用的软件包当中。


# 4. A:什么是SNP？为什么SNP的研究是重要的？举出2~3个SNP相关的网站【补：SNP研究有哪些优点？】

# 4. B:什么是系统生物学？系统生物学对生物功能实现的理解有何本质变化？【补：系统生物学的研究思路是什么？】

# 5. 什么是contig和scaffold，L50和N50是什么?
> 1. contig：A contig (from contiguous) is a set of overlapping DNA segments that together represent a consensus region of DNA.
>    
>    重叠群（来自连续的）是一组重叠的、完整连续的DNA片断或Reads，中间没有缺失序列（gap）。
>    
> 2. scaffold：A scaffold is a portion of the genome sequence reconstructed from end-sequenced whole-genome shotgun clones. Scaffolds are composed of contigs and gaps.
> 
>    支架是从末端测序的全基因组鸟枪克隆重建的基因组序列的一部分。脚手架由重叠部分和间隙组成。
>
> 3. N50把contig或scaffold按照从大到小的顺序排列，长度达到基因组大小（所有contig或scaffold的长度）的50%时，那条contig/scaffold的长度，即为contig/scaffold N50. N50越大，说明基因组组装的质量越高。
> 
> 5. L50
>    长度总和产生N50的contig/scaffold的数量
>
> [网页答案](https://www.jianshu.com/p/117441ac6eb8)

# 6. 大数据分析需要注意的问题
![大数据分析](https://img-blog.csdnimg.cn/direct/11d8c431f8014c31afc8ea57db2bf670.jpeg)

# 7. 真阳性，真阴性，假阳性，假阴性，灵敏度，特异性
True Positive （真阳性, TP）被模型预测为正的正样本；可以称作判断为真的正确率
True Negative（真阴性, TN）被模型预测为负的负样本 ；可以称作判断为假的正确率
False Positive （假阳性, FP）被模型预测为正的负样本；可以称作误报率
False Negative（假阴性, FN）被模型预测为负的正样本；可以称作漏报率
灵敏度Sensitivity：
                TPR = TP /（TP + FN）
                正样本预测结果数 / 正样本实际数
特异性Specificity：
                TNR = TN /（TN + FP）
                负样本预测结果数 / 负样本实际数
# 8. [计算题] Nearest Neighbor Model for Watson-Crick Base Pairs
**Watson-Crick 碱基对的最近邻模型，描述了 DNA 中碱基对之间的相互作用力和稳定性**

Nearest Neighbor Model for Free Energy of a Sample Hairpin Loop：

**通过计算样品发夹环中碱基对的相互作用能量，可以评估该环状结构的稳定性和热力学特性**
![https://img-blog.csdnimg.cn/direct/8093797858be4b26ad39aff1dadaf137.png](https://img-blog.csdnimg.cn/direct/8093797858be4b26ad39aff1dadaf137.png)
![https://img-blog.csdnimg.cn/direct/651d803a0129497cbd0ab2f076516b69.png](https://img-blog.csdnimg.cn/direct/651d803a0129497cbd0ab2f076516b69.png)
# 9. [名词解释]
> 1. Genotype:thegenetic constitution of the organism.生物体的遗传构成。
>
> 2. Phenotype:thecomposite of an organism's observable characteristics or traits.生物体可观察到的特点或特征的总和。
>
> 3. Allele Frequencies：特定等位基因/所有等位基因。每个个体的两条染色体都要考虑。【2*纯合子+杂合子】
>
> 4. Cohort(队列)：a groupof people who share a common characteristic or experience within a definedperiod (e.g., are born, are exposed to a drug or vaccine or pollutant, orundergo a certain medical procedure). 在一定时期内具有共同特征或经历的一个群体。（例如，出生日期，使用同种药物、接种同种疫苗或接受特定的医学治疗）。
>
> 5. Missense mutation & Nonsense mutation（终止密码子的出现）
A point mutation in which a single nucleotide change results in a codonthat codes for a different amino acid. 一种点突变，其中单个核苷酸的变化导致编码不同氨基酸的密码子的改变。会改变蛋白质序列，一般发生在遗传密码子的第一位或第二位。
![https://img-blog.csdnimg.cn/direct/de5706ce324f4e1d984b4918bd8df54f.png](https://img-blog.csdnimg.cn/direct/de5706ce324f4e1d984b4918bd8df54f.png)
A pointmutation that results in a stop codon (nonsense codon) in a transcribed mRNA,which encodes incomplete and usually nonfunctional protein product.在转录的mRNA中引入终止密码子的点突变。会导致翻译提前终止，得到不完整、无生物功能的蛋白质。更易造成疾病。
![https://img-blog.csdnimg.cn/direct/0b93511375b749dba1b691f07dcda8bc.png](https://img-blog.csdnimg.cn/direct/0b93511375b749dba1b691f07dcda8bc.png)

# 参考链接
1. [【国科大——期末复习】生物信息学(陈润生)_期末考试答案（持续更新~）](https://blog.csdn.net/m0_61164319/article/details/133918588?spm=1001.2014.3001.5502)
