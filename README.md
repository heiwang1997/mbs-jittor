# MultiBodySync: 基于三维扫描同步的多刚体运动分割技术

本仓库是论文 [MultiBodySync: Multi-Body Segmentation and Motion Estimation via 3D Scan Synchronization](https://arxiv.org) 的 [计图](https://cg.cs.tsinghua.edu.cn/jittor/) 实现。
计图是由清华大学计算机系 [图形学实验室](https://cg.cs.tsinghua.edu.cn/) 推出的一个完全基于动态编译、内部使用创新的元算子和统一计算图的深度学习框架。

- 目前我们正在积极与计图团队合作，在完成之前，你也可以参考这里的[Pytorch实现](https://github.com/huangjh-pub/multibody-sync)
- 近日，“计图”人工智能算法挑战赛正在如火如荼进行，欢迎大家来[这里](https://www.educoder.net/competitions/index/Jittor-1)观战！
- Welcome to use Jittor! It is faster than pytorch according to [this paper](https://cg.cs.tsinghua.edu.cn/papers/SCIS-2020-jittor.pdf). Also it is flexible and fully supported by our splendid [team](https://cg.cs.tsinghua.edu.cn/jittor/about/)!
- We launched a new open access journal, **[Computational Visual Media](http://www.springer.com/computer/image+processing/journal/41095) (CVMJ)**. It publishes original high-quality research papers and significant review articles on novel ideas, methods, and systems relevant to visual media.

## 简介

![Logo](assets/teaser.jpg)

MultiBodySync是一个支持端到端训练的**多输入、多刚体运动分割与注册算法**。具有如下的特性：
- 保证多点云输入之间的匹配与运动分割的循环一致性；
- 可泛用的基于运动信息的鲁棒分割。

## 安装计图

用 [Anaconda](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/) 能够比较方便的管理Python的各种包。在创建好环境之后，可以运行下面的命令安装依赖：

```shell script
# 安装计图 (如果遇到问题可以参考：https://cg.cs.tsinghua.edu.cn/jittor/download/)
sudo apt install python3.7-dev libomp-dev
sudo python3.7 -m pip install git+https://github.com/Jittor/jittor.git
```
