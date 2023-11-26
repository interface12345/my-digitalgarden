---
{"dg-publish":true,"permalink":"//","tags":["gardenEntry"]}
---

## 动态路由协议分类
### 按算法分类
* 距离矢量路由协议 DV型：RIP、Eigrp、BGP “道听途说”，路标
* 链路状态路由协议 LS型：OSPF、ISIS 地图
### 按范围分类
* 内部网关路由协议（IGP）AS内部：RIP、Eigrp、OSPF、ISIS
* 外部网关路由协议（EGP）AS外部：BGP
### 按是否携带子网掩码分类
* 有类路由协议 RIPv1 “更新报文中不携带Mask”
* 无类路由协议 RIPv2、Eigrp、OSPF、ISIS、BGP
Eigrp是思科私有路由协议
## RIP
路由器之间交互路由表，学习本地没有的路由
RIP使用跳数（hop）作为度量值
每经过一台路由器跳数加一
metricout 发出去时+1
metricin 接收时+0
基于传输层协议UDP，端口号：520
1. RIPv1
	* RIPv1是有类别路由协议，不支持VLSM和CIDR。
	* 以广播的形式发送报文。
	* 不支持认证。
2. RIPv2
	* RIPv2为无类别路由协议，支持VLSM，支持路由聚合与CIDR。
	* 支持以广播或者组播（224.0.0.9）方式发送报文。
	* 支持明文认证和MD5密文认证。




---

[[数据通信目录\|数据通信目录]]
[[Obsidian使用手册\|Obsidian使用手册]]