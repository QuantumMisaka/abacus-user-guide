# ABACUS使用教程

# 一、介绍

ABACUS（Atomic-orbtial Based Ab-initio Computation at UStc，中文名原子算筹）是国产开源密度泛函理论软件，相关介绍 ABACUS 的新闻可在[ABACUS 新闻稿整理](abacus-news.md)查看，以下是一些常用地址：

ABACUS 在 DeepModeling 社区中的 GitHub 仓库地址为：

[https://github.com/deepmodeling/abacus-develop](https://github.com/deepmodeling/abacus-develop)

ABACUS 的 Gitee 镜像仓库地址为：

[https://gitee.com/deepmodeling/abacus-develop](https://gitee.com/deepmodeling/abacus-develop)

ABACUS 网站访问：

[http://abacus.ustc.edu.cn/](http://abacus.ustc.edu.cn/)

文档（包括安装方法、输入输出参数介绍、功能介绍、算例介绍、开发者须知等）：

[https://abacus.deepmodeling.com/en/latest/](https://abacus.deepmodeling.com/en/latest/)。

本教程系列旨在帮助新手用户入门了解 ABACUS 的使用。秉着开源软件的理念，本文档是由开源社区的老师同学们贡献所成。如果你也想贡献一份文档，我们十分欢迎，请参考[如何贡献ABACUS使用教程](abacus-contribute.md)

# 二、ABACUS基本操作教程

1. ABACUS的编译介绍
   1. [官方编译教程](https://abacus.deepmodeling.com/en/latest/quick_start/easy_install.html)
   2. [知乎上用户提供的ABACUS 3.0安装教程](https://zhuanlan.zhihu.com/p/574031713)
   3. [<mark style="color:red;">编译无MPI的ABACUS</mark>](https://xmywuqhxb0.feishu.cn/docx/JCv0dHPP6o69JdxtG33cIcTnnke)<mark style="color:red;"></mark>
   4. 曙光DCU平台编译教程：[ABACUS 在曙光 DCU 集群上的编译与使用](abacus-dcu.md)
2. ABACUS建模介绍
   1. 准备晶胞和原子位置等信息的文件STRU：[<mark style="color:red;">如何转换STRU的格式</mark>](https://xmywuqhxb0.feishu.cn/docx/M6NSdwkMdoQJQlxrcVCczioDnlb)<mark style="color:red;"></mark>
   2. 准备赝势：
   [模守恒赝势生成方法简介](abacus-upf.md)
   3. 数值原子轨道基组生成教程：
      1. [数值原子轨道（一）：ABACUS 中的数值原子轨道命名和使用方法](abacus-nac1.md)
      2. [数值原子轨道（二）：生成给定模守恒赝势的数值原子轨道](abacus-nac2.md)
      3. [数值原子轨道（三）：产生高精度数值原子轨道](abacus-nac3.md)
3. Kohn-Sham密度泛函理论
   1. 电子自洽迭代
      1. 平面波PW（缺）
      2. 数值原子轨道LCAO（缺）
   2. 带自旋的体系计算：[<mark style="color:red;">ABACUS磁性材料计算使用教程</mark>](https://xmywuqhxb0.feishu.cn/docx/E4ZvdMJzGonWJhxanBacS6dWnsP)<mark style="color:red;"></mark>
   3. \+U计算：[<mark style="color:red;">ABACUS DFT+U使用教程</mark>](https://xmywuqhxb0.feishu.cn/docx/SLqAdIXKyojyVBxVvOdc4LKsnub)<mark style="color:red;"></mark>
   4. 结构优化（缺）
   5. 分子动力学：[ABACUS 分子动力学使用教程](abacus-md.md)
4. DeePKS方法（缺）
5. 隐式溶剂计算等相关功能（缺）
6. 随机波函数密度泛函理论：[ABACUS 随机波函数DFT方法使用教程](abacus-sdft.md)
7. 无轨道密度泛函理论：[ABACUS 无轨道密度泛函理论方法使用教程](abacus-ofdft.md)
8. 分析结果
   1. 能带计算
      1. [<mark style="color:red;">如何正确画能带，NSCF读电荷密度</mark>](https://xmywuqhxb0.feishu.cn/docx/K8GRdTst4oXQNoxnQVbcFZTmntb)<mark style="color:red;"></mark>
      2. [<mark style="color:red;">用ABACUS-ASE自动产生能带路径</mark>](https://xmywuqhxb0.feishu.cn/docx/KjzEdIsAfoNvaWxHrXSc2QWgnZX)<mark style="color:red;"></mark>
   2. PDOS计算
      1. [<mark style="color:red;">ABACUS里怎样做DOS和PDOS计算</mark>](https://xmywuqhxb0.feishu.cn/docx/ONSldj82VoNGKSxaoDQcoKBtnGh)<mark style="color:red;"></mark>
9. 和其他软件对接
   1. [ABACUS+Phonopy 计算声子谱](abacus-phonopy.md)
   2. [ABACUS+ShengBTE 计算晶格热导率](abacus-shengbte.md)
   3. [ABACUS+DPGEN 使用教程](abacus-dpgen.md)
   4. [ABACUS+LibRI 做杂化泛函计算教程](abacus-libri.md)
   5. [ABACUS+Candela 使用教程](abacus-candela.md)
   6. ABACUS+CINEB教程（缺）
      1. [<mark style="color:red;">ABACUS-ASE做NEB计算</mark>](https://dptechnology.feishu.cn/wiki/wikcnzar41sN8ZtGLtm3PLnarSc) <mark style="color:red;"></mark> （简单算例）

# 三、使用经验

1. 有VASP使用背景的用户上手ABACUS教程：[<mark style="color:red;">ABACUS新人使用的一些注意事项</mark>](https://xmywuqhxb0.feishu.cn/docx/KN3KdqbX6o9S6xxtbtCcD5YPnue)<mark style="color:red;"></mark>
