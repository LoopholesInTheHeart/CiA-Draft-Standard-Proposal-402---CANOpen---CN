<!-- TOC -->

- [3. 定义和缩写](#3-定义和缩写)
    - [CAN](#can)
    - [CiA](#cia)
    - [COB](#cob)
    - [COB-ID](#cob-id)
    - [PDO](#pdo)
    - [SDO](#sdo)
    - [pp](#pp)
    - [pv](#pv)
    - [vl](#vl)
    - [hm](#hm)
    - [ip](#ip)
    - [tq](#tq)
    - [all](#all)
    - [ce](#ce)
    - [dc](#dc)
    - [pc](#pc)

<!-- /TOC -->

---

## 3. 定义和缩写 
>DEFINITIONS AND ABBREVIATION 

### CAN   
CAN控制网络
>CAN Controller Area Network

### CiA   
CiA组织/CiA标准/CAN总线在自动化中的应用
>CiA CAN in 
mation e. V.

### COB   
COB通信对象(CAN中的消息单元)，是CAN网络中的运输单位，CANOpen数据都必须通过她来发送
>COB Communication Object (CAN message). A unit of transportation in a CAN network.Data must be sent across a network inside a COB.

### COB-ID
COB消息的ID号/标识符,COB-ID号在网络中通常是唯一的,还确定了在MAC子层中的优先级  
>COB-ID COB-Identifier. Identifies a COB uniquely in a network. The identifier determines the priority of that COB in the MAC sub-layer too.  
__译注：COB-ID是确定PDO编号，并且将两侧设备数据统合在一起最重要的东西，当设备两侧所定义的协议中的COB-ID一致时，协议就建立起来了(拥有共同的ID号)__

### PDO   
PDO是过程数据对象，是用于在设备之间交换数据的对象
>PDO Process Data Object. Object for data exchange between several devices.  
__译注：PDO传输速率极快，但通常数据量较为简单，使用时有前提限制(NMT命令节点启动)，具体可参考CiA DS301内容__

### SDO   
SDO是服务数据对象，通过访问对象进行对等通信
>SDO Service Data Object. Peer to peer communication with access to the object dictionary of a device.  
__译注：PDO通常只在主控制器启动时下发数据，用于配置驱动器参数等__

### pp   
轮廓位置模式
>pp Profile Position Mode

### pv   
轮廓速度模式
>pv Profile Velocity Mode

### vl   
速度模式
>vl Velocity Mode

### hm   
回原模式
>hm Homing Mode

### ip   
插值位置模式
>ip Interpolated Position Mode

### tq   
轮廓 力矩/电流模式
>tq Profile Torque Mode

### all   
在所有模式中都需要提供(对该Object进行支持/...)
>all Mandatory for all modes

### ce   
对象字典中的公共条目(共有部分)
>ce Common entries in the object dictionary

### dc   

>dc Device Control

### pc   
位置控制函数/功能 *（？歧义* 
>pc Position Control Function
