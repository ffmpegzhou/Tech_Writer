## 机房供电
keyword: 生命周期成本； 可扩充性；功率因数；
---

典型的机房负载：照明3%，UPS11%，制冷50%，关键负载36%；

### 估算负载
关键负载，包括业务所需的硬件设备，服务器、路由器、消防、监控等。

UPS负载：电池充电的功率一般占UPS实际功率的20%

照明负载：经验值-按每平方米21.5w计算

制冷负载：非重点，之后讨论；

### 确定电力线路容量
估算电力线路容量，以及备用发电机容量；

## UPS设计
keyword： 静态旁路；冗余；总拥有成本Total cost of ownership (TCO)；静态转换开关STS

后备电源位于市电与负载之间，用于隔离和净化断电、压降、电涌、谐波、线躁等情况。

UPS在系统中的设计简要分为：
* A单机（N）
* B串联冗余
* C并联冗余(N+1)
* D分布式冗余
* E双系统(2N+1)

A方案成本最低，UPS出现问题时立刻切换到静态旁路。

B方案正常运行状态下，副UPS完全不承担负载，主UPS出现故障则立刻切换到副UPS。

C方案必须用两个完全一样的UPS模块，可根据增长灵活扩容。但是需要外部的静态开关来保持负载均衡；

D方案和双系统几乎完全一致，唯一区别在于UPS模块数目不同。

E是最昂贵的配置，两条线路互为热备，可靠性极高。

UPS分类：
* 后备式
* 在线互动式
* 双转换在线式
* Delta转换在线式；

## 机柜供电要求

* 电压
* 功率 
* 冗余度
* 过载保护
* 连接器
* 一致性（标准化线缆）

### 7类主要的电源问题
* 瞬变：分为脉冲和暂态震荡，通常由闪电、接地不良、调速器引发。解决方法是加浪涌保护器。
* 中断。解决方法是加UPS。
* 电压突降：通常由大负载突然启动引发。解决方法是加软启动电源。
* 电压突升：通常由大负载突然下降、相位故障引发。解决方法是加UPS。
* 波形畸变：（直流偏移、谐波、线躁）；
* 电压波动：电压系统性变动。
* 频率变化：



