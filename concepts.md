# 主要概念



![image](/images/concepts.png)

## 私有专区

用户独享的资源池（物理宿主机）的集合。

## 资源池

用户独享的物理宿主机资源。一个资源池具备32核，内存可选64G、96G、128G、160G，数据盘可选4T、6T，可在专用资源块上申请专区主机。

## 私有专区主机

专区主机和UCloud公有云其他的云主机物理层隔离，不会与其他用户的云主机发生IO竞争，但网络互通。但包括登录、开机、关机、升降级、重装、监控、绑定EIP、关联VPC、绑定UDisk等操作与主机完全一致。

私有专区支持的云主机机型包括：

### 标准机型

**配置支持：**

CPU：1核～16核 

内存：1GB～64GB

数据盘磁盘空间：0GB～1TB

暂不支持网络增强特性

 [云主机磁盘I/O基准性能测试](uhost/testdata/io_uhost)

## 地域与可用区

可用区是一组物理和电力上相互隔离的资源的组合。一个可用区可能是由一个机房、或者多个机房的一部分组合后设计而成。
经合理设计后，故障影响范围会被隔离在单个可用区内。

地理上相互靠近的若干可用区，通过高速稳定的网络连接，可以组成一个地域。同地域内的可用区之间的内网能够互通。

目前提供私有专区服务的地域包含北京二、上海二和广州。具体可用区则划分为北京二可用区B、北京二可用区C、北京二可用区D；上海二可用区B以及广州可用区B。

关于其他产品概念，例如镜像、网络，请参考 [云主机产品概念](uhost/introduction/concept)。
