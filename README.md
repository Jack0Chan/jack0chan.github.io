[toc]

# 江智浩课题组实验室手册

## 零、前言

大家一起来编辑。目前写成markdown文件，如果有更好的形式请联系推荐给陈光耀，最好是有模糊搜索功能（或者我们自己写一个也行，可能会用到这个：[近邻词汇检索](https://tool.mingdawoo.com/lang/nearby_word)）。



### 附：实验室各事物主要负责人（按名字排序）

注意只是主要负责人，其实有啥问题不一定非得找主要负责人，其他同学应该也清楚相关情况。

1.  陈光耀：实验室安全，实验室活动组织，多核服务器管理，小额财务报销，各种实验室事务。
2.  陈逸伦：财务助理，服务器管理助理，各种实验室事务。
3.  顾吉成：NAS管理，外星人服务器管理，各种实验室事务。
4.  唐韧之：NAS管理，外星人服务器管理，各种实验室事务。



## 一、打印机配置及使用

打印机名称：FUJI XEROX Dokuprint P455 d。

### 1. 有线使用方法

打印机旁边有USB接口，直接连接到笔记本电脑上即可使用。

### 2. 无线使用配置方法

打开 控制面板-查看设备和打印机，点击 ”添加打印机“。参数设置如下：

-   设备类型(T)：自动检测
-   主机名或 IP 地址(A)：10.19.129.48
-   端口名称：10.19.129.48
-   勾选 ”查询打印机并自动选择要使用的打印机驱动程序“

添加完成后，在 控制面板-查看设备和打印机 中会看到 "FUJI XEROX Dokuprint P455 d" 打印机，打印时选择该打印机即可。



## 二、论文写作

### 1. 变量命名方法（实验、写作）-- 驼峰命名法

有时候，我们需要在论文中提及某些变量，变量命名有许多种方法，比较常见的是**下划线命名法**和**驼峰命名法（Camel-Case）**。就投递论文经验来看，有些reviewer不喜欢下划线命名法，就视觉感受而言论文中过多的下划线确实会导致比较差的论文观感，为此我们建议在写代码和写论文的时候，使用**驼峰命名法**以保证论文的美观，同时提高写作效率。下面是一些使用建议。

驼峰命名法（Camel-Case）：

1.  变量名用小驼峰法（lowerCamelCase）

    -   例如：numStudent
    -   对于一些缩写后不影响阅读的，可以舍弃某个或某些元音（见仁见智），比如 numStdent。 

2.  模块、函数等名字用大驼峰法（UpperCamelCase）

3.  对于分层的结构，比如$H1\_1$，$H1\_2$，$H2\_1$，$H2\_2$这种，我们可以用

    -   例如：LV1Heart1，LV1Heart2，LV2Heart1，LV2Heart2来表示。比如LV1Heart1表示Level1HeartModel1。因为表示的是心脏模型，不是变量名，所以用大驼峰命名法。

### 2. arXiv提交踩坑

出现以下问题可能会被管理员嫌弃。

1. arXiv在提交的过程中会自动保存metadata，提交之后会一直保存你的提交。如果要重新提交，在原来的提交中选择提交，而不是start a new submission。
2. 由于浏览器缓存问题，在提交时可能看不到过去的提交，此时应该清空浏览器缓存而不是尝试新的提交。



## 三、服务器

每个同学都会获得服务器账号，用户名为名字首字母小写（比如张三的用户名为zs），密码请询问管理员。

各服务器ip地址：

1.  多核服务器：
2.  外星人：
3.  GitLab：http://10.19.129.80:30000/

### 1. 多核服务器使用（windows + 多核心CPU）

#### 1）服务器配置

-   设备名称：CPSLab
-   操作系统：Windows10 专业工作站
-   CPU：[Intel® Xeon® Gold 6248R Processor](https://ark.intel.com/content/www/us/en/ark/products/199351/intel-xeon-gold-6248r-processor-35-75m-cache-3-00-ghz.html)
    -   14 nm，24C/48T
    -   3.00 GHz Base，4.00 GHz Turbo
    -   35.75 M Cache，10.4 GT/s Bus Speed
    -   205 W Thermal Design Power (TDP)
    -   Max Memory Size: 1 TB
-   显卡：亮机卡
-   内存：128G，CPU最大支持内存为 1 TB



### 2. 外星人使用（Ubuntu + 高性能单核CPU + 高性能显卡）

#### 1）服务器配置

-   设备名称：
-   操作系统：Ubuntu
-   CPU：[Intel® Core™ i9-10900KF Processor](https://ark.intel.com/content/www/us/en/ark/products/199331/intel-core-i9-10900kf-processor-20m-cache-up-to-5-30-ghz.html)
    -   14 nm，10C/20T
    -   3.70 GHz Base，5.30 GHz Turbo
    -   20 MB Cache，8 GT/s Bus Speed
    -   125W Thermal Design Power (TDP)
-   显卡：[GeForce RTX 3090 显卡 | NVIDIA](https://www.nvidia.cn/geforce/graphics-cards/30-series/rtx-3090/)
    -   NVIDIA CUDA® 核心数量：10496
    -   基础频率 1.40 GHz，加速频率 1.70GHz
    -   显存位宽：384 位
    -   标准显存配置：24 GB GDDR6X
    -   NVIDIA 架构：Ampere
    -   Tensor Cores：第 3 代
    -   功率：最低350W，推荐750W
-   内存：128G，已经是CPU最大支持内存



### 3. 实验室GitLab使用

我们的GitLab地址为：http://10.19.129.80:30000/

可以用GitHub Desktop克隆下来，克隆的时候选择使用URL克隆。



## 四、LaTex经验

### 1. LaTex输入中文

如果LaTex打中文出现如下错误：

```
! Improper alphabetic constant.
<to be read again> 
\hspace 
l.1 ...berline {第一章\hspace {.3em}}测试}{5}
```

原因是在 `\documentclass{ctexbook}` 中少写了一个 `[UTF8]`  ，加上它就没有这个错误了，即改为如下代码后，就没有该错误了：

```latex
\documentclass[UTF8]{ctexbook}
\begin{document}
\title{中文 \LaTeX{} 测试}
\author{姓名}
\maketitle
\tableofcontents
\chapter{测试}
中文测试.
\chapter{再测试}
中文测试.
\end{document}
```

### 2. LaTex表格在线编辑

https://www.tablesgenerator.com/ 



## 五、上科大相关

### 1. 学院英文名

信息学院：School of Information Science and Technology

电子信息工程的英文名称为： Electronic Information Engineering

计算机科学与技术的英文名称为：Computer Science and Technology

工学学士的英文名称为：Bachelor of Engineering

### 2. 学校基本信息

毕业派遣所需学校基本信息

1.  单位基本信息

    单位名称：上海科技大学

    单位所在地：上海市浦东新区华夏中路393号

    单位邮编：201210

2.  单位联系人信息

    单位联系人：胡老师

    联系人电话：021-20685449

    联系人邮箱：gadmission@shanghaitech.edu.cn

3.  档案寄存信息

    档案转寄单位名称：上海科技大学

    档案转寄单位地址：上海市浦东新区华夏中路393号上海科技大学图书馆102室

    档案转寄单位邮编：201210

    档案接收部门：图书信息中心（档案馆）

    接收联系人：谢老师

    接收联系电话：021-20685214

### 3. 上科大PPT模板、Logo



## 六、 实验室福利

注意：hw只能用来参考，严禁抄袭，如有发现，从严处理。

1.  CS240算法设计课程cheatsheet、hw、考试
2.  CS244计算理论复习总结、hw、参考资料
3.  研究生思想政治考试资料

