# Neutron 网络基础

## 说明

本书记录了笔者在工作及日常学习中的一些学习笔记以及经验。这是一本关于Neutron的基础书籍，或许其最终的篇幅会的很长，但还是希望大家把他当成一本基础书籍来翻阅。下面是本书在编写时候的一些说明：

* 严格性不足。笔者希望能编写一本内容严格的书籍出来，但由于能力、时间的原因，目前不能保证书中的内容百分百准确。虽然或许书中的某些内容存在错误，但笔者会保证这些内容对于Neutron的基础来说是足够了的。当读者在日常的工作中要用到某个知识点的时候，本书能起到一个引路人的作用，帮助读者更快更好的去掌握这个知识点。
* 注重广度而非深度。由于本书的定位是Neutron的基础知识，所以笔者会更加偏向于基础知识的广度而非深度。

## 写作周期

本书会分为三个阶段进行编写：

1. 初稿，完成大体框架。不包含图片
2. 对初稿的语言、内容进行加工，补充图片
3. 定稿

目前处于第一个阶段。

## 错误纠正

由于笔者水平有限，书中难免有错误。如果大家发现了问题欢迎大家指出，可以：

* 提issue
* 发送错误内容邮件给tianhuan@bingotree.cn

## 目录&进度

注意：目前处于第一阶段，下面的目录可能会有微调。

```
第一章 本书介绍
第二章 Neutron的部署、运维、高可用
    常用命令（ip/iptables/tc & qdisc/tcpdump/route/brctl/veth）
    namespace简介及用法
    ovs简介及常用命令
    libvirt/qemu中的网络
    Neutron部署
    Neutron日常维护及监控
    Neutron高可用（各个组件高可用探讨、部署方法）
    Neutron安全
    Neutron升级
第三章 Neutron实现
    开发环境的搭建
    如何共享代码
    基础类库
        重要基础类库（stevedore）
        非重要基础类库
    Big Picture
    ML2
        设计思想
        ovs流表操作练习
        实现分析
    DHCP Agent
        设计思想
        实现分析
    L3 Agent
        设计思想
        路由相关操作练习
        实现分析
    Metadata Agent
        设计思想
        实现分析
    SRIOV Agent
        设计思想
        实现分析
    Service Chain
        设计思想
        实现分析
    其它
        ARP防毒化
        Dragon Flow
        思科ACI
        ...
第四章 其它组件与Neutron的交互
    Nova
    Trove
    ...
第五章 底层网络基础
    5.1内核网络相关基础知识    # 一期完成
        sk_buff数据结构    # 一期完成
        net_device数据结构    # 一期完成
        硬件中断&module机制    # 一期完成
        softirq    # 一期完成
        proc文件系统    # 一期完成
    5.2协议栈中的收包/发包  # 一期完成
        PCIe设备驱动的加载    # 一期完成
        收包路径    # 一期完成
        发包路径    # 一期完成
        lo/veth的实现    # 一期完成
        多队列/RSS/RPS/RFS  # 一期完成
        LSO/LRO/GSO/GRO/TSO/USO # 一期完成
        DPDK    # 一期完成
    5.3网络namespace的实现 # 一期完成
    5.4Linux Bridge的实现   # 一期完成
    5.5OVS的实现
第六章 SDN
第七章 容器中的网络 # 一期完成
    容器 or 传统虚拟化？    # 一期完成
    Docker  # 一期完成
    Kubernetes  # 一期完成
    libnetwork  # 一期完成
    Neutron与容器 # 一期完成
第八章 后记
```

