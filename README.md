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

# 参考链接
1. [【国科大——期末复习】生物信息学(陈润生)_期末考试答案（持续更新~）](https://blog.csdn.net/m0_61164319/article/details/133918588?spm=1001.2014.3001.5502)
