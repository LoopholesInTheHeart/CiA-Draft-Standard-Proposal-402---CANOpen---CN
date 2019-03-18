CONTENTS
===

## 目录

<!-- TOC -->

- [目录](#目录)
- [1. 范围](#1-范围)
- [2. 参考文件/引用](#2-参考文件引用)
- [3. 定义和缩写](#3-定义和缩写)
- [4. 概述](#4-概述)
    - [4.1. 访问驱动器](#41-访问驱动器)
    - [4.2. 驱动器架构](#42-驱动器架构)
- [5. 工作原理](#5-工作原理)
    - [5.1. 引言/介绍](#51-引言介绍)
    - [5.2. 通过分析进行标准化](#52-通过分析进行标准化)
    - [5.3. 对象字典](#53-对象字典)
        - [5.3.1. 索引和子索引的使用](#531-索引和子索引的使用)
- [6. 紧急消息](#6-紧急消息)
    - [6.1. 原则/原理 *（？歧义*](#61-原则原理-歧义)
    - [6.2. 错误代码](#62-错误代码)
- [7. 预定义](#7-预定义)
    - [7.1. 预定义对象](#71-预定义对象)
        - [7.1.1. 对象1000 h:设备类型](#711-对象1000-h设备类型)
        - [7.1.2. 对象1001 h:错误寄存器](#712-对象1001-h错误寄存器)
        - [7.1.3. 对象67FF h:单一设备类型](#713-对象67ff-h单一设备类型)
    - [7.2. PDO映射](#72-pdo映射)
        - [7.2.1. 接收pdo](#721-接收pdo)
        - [7.2.2. 发送pdo](#722-发送pdo)
- [8. 对象字典](#8-对象字典)
- [9. 共同条目/常见条目](#9-共同条目常见条目)
    - [9.1. 一般信息](#91-一般信息)
        - [9.1.1. 电机数据](#911-电机数据)
        - [9.1.2. 驱动器数据](#912-驱动器数据)
    - [9.2. 对象字典条目](#92-对象字典条目)
        - [9.2.1本章定义的对象](#921本章定义的对象)
    - [9.3. 对象描述](#93-对象描述)
        - [9.3.2. 对象603F h：错误代码](#932-对象603f-h错误代码)
        - [9.3.3. 对象6402 h：电机类型](#933-对象6402-h电机类型)
        - [9.3.4. 对象6403 h：电机目录号](#934-对象6403-h电机目录号)
        - [9.3.5. 对象6404 h：电机制造商](#935-对象6404-h电机制造商)
        - [9.3.6. 对象6405 h：http电机目录地址](#936-对象6405-hhttp电机目录地址)
        - [9.3.7. 对象6406 h：电机校准日期](#937-对象6406-h电机校准日期)
        - [9.3.8. 对象6407 h：电机服务期](#938-对象6407-h电机服务期)
        - [9.3.9. 对象6410 h：电机数据](#939-对象6410-h电机数据)
        - [9.3.10. 对象6502 h：支持的驱动模式](#9310-对象6502-h支持的驱动模式)
        - [9.3.11. 对象6503 h：驱动器目录号](#9311-对象6503-h驱动器目录号)
        - [9.3.12. 对象6504 h：驱动器制造商](#9312-对象6504-h驱动器制造商)
        - [9.3.13. 对象6505 h：http驱动器目录地址](#9313-对象6505-hhttp驱动器目录地址)
        - [9.3.14. 对象6510 h：驱动数据](#9314-对象6510-h驱动数据)
        - [9.3.15. 对象60FD h：数字输入](#9315-对象60fd-h数字输入)
        - [9.3.16. 对象60FE h：数字输出](#9316-对象60fe-h数字输出)
- [10. 设备控制](#10-设备控制)
    - [10.1. 一般/通用信息](#101-一般通用信息)
        - [10.1.1. 状态机](#1011-状态机)
    - [10.2. 对象字典条目](#102-对象字典条目)
        - [10.2.1本章定义的对象](#1021本章定义的对象)
    - [10.3. 对象描述](#103-对象描述)
        - [10.3.1. 对象6040 h：控制字](#1031-对象6040-h控制字)
        - [10.3.2. 对象6041 h：状态字](#1032-对象6041-h状态字)
        - [10.3.3. 对象605B h：关闭选项代码](#1033-对象605b-h关闭选项代码)
        - [10.3.4. 对象605C h：禁用操作选项代码](#1034-对象605c-h禁用操作选项代码)
        - [10.3.5. 对象605A h：快速停止/急停 选项代码](#1035-对象605a-h快速停止急停-选项代码)
        - [10.3.6. 对象605D h：暂停选项代码](#1036-对象605d-h暂停选项代码)
        - [10.3.7. 对象605E h：故障反应选项代码](#1037-对象605e-h故障反应选项代码)
        - [10.3.8. 对象6060 h：操作模式](#1038-对象6060-h操作模式)
        - [10.3.9. 对象6061h：操作模式显示](#1039-对象6061h操作模式显示)
    - [10.4. 功能描述](#104-功能描述)
        - [10.4.1. 操作模式功能](#1041-操作模式功能)
        - [10.4.2. 驱动器禁用功能/驱动器禁能](#1042-驱动器禁用功能驱动器禁能)
        - [10.4.3. 快速停止功能/急停](#1043-快速停止功能急停)
        - [10.4.4. 停止功能](#1044-停止功能)
        - [10.4.5. 故障反应](#1045-故障反应)
- [11. 因素组/影响参数/影响因子  *（？歧义*](#11-因素组影响参数影响因子--歧义)
    - [11.1. 一般信息](#111-一般信息)
        - [11.1.1. 因素/参数/影响因子  *（？歧义*](#1111-因素参数影响因子--歧义)
        - [11.1.2. 物理/物理单位 和内部单位之间的关系  *（？歧义*](#1112-物理物理单位-和内部单位之间的关系--歧义)
    - [11.2. 对象字典条目/对象字典映射表](#112-对象字典条目对象字典映射表)
        - [11.2.1. 本章定义的对象](#1121-本章定义的对象)
    - [11.3. 对象描述](#113-对象描述)
        - [11.3.1. 对象6089h：位置符号索引  *（？歧义*](#1131-对象6089h位置符号索引--歧义)
        - [11.3.2. 对象608Ah：位置单位索引  *（？歧义*](#1132-对象608ah位置单位索引--歧义)
        - [11.3.3. 对象608Bh：速度符号索引  *（？歧义*](#1133-对象608bh速度符号索引--歧义)
        - [11.3.4. 对象608C h：速度单位指数索引  *（？歧义*](#1134-对象608c-h速度单位指数索引--歧义)
        - [11.3.5. 对象608D h：加速度表示法指数索引  *（？歧义*](#1135-对象608d-h加速度表示法指数索引--歧义)
        - [11.3.6. 对象608Eh：加速单位指数索引  *（？歧义*](#1136-对象608eh加速单位指数索引--歧义)
        - [11.3.7. 对象608Fh：位置编码器分辨率](#1137-对象608fh位置编码器分辨率)
        - [11.3.8. 对象6090h：速度编码器分辨率](#1138-对象6090h速度编码器分辨率)
        - [11.3.9. 对象6091h：齿轮比](#1139-对象6091h齿轮比)
        - [11.3.10. 对象6092h：进给常数.​​](#11310-对象6092h进给常数​​)
        - [11.3.11. 对象6093h：位置因子](#11311-对象6093h位置因子)
        - [11.3.12. 对象6094h：速度编码器因子](#11312-对象6094h速度编码器因子)
        - [11.3.13. 对象6095h：速度因子1](#11313-对象6095h速度因子1)
        - [11.3.14. 物体6096h：速度因子2](#11314-物体6096h速度因子2)
        - [11.3.15. 对象6097h：加速因子](#11315-对象6097h加速因子)
        - [11.3.16. 对象607Eh：极性](#11316-对象607eh极性)
- [12. 规划位置模式](#12-规划位置模式)
    - [12.1. 一般信息](#121-一般信息)
        - [12.1.1. 输入数据描述](#1211-输入数据描述)
        - [12.1.2. 输出数据说明](#1212-输出数据说明)
        - [12.1.3. 内部状态](#1213-内部状态)
    - [12.2. 对象字典条目](#122-对象字典条目)
        - [12.2.1. 本章定义的对象](#1221-本章定义的对象)
        - [12.2.2. 其他章节中定义的对象](#1222-其他章节中定义的对象)
    - [12.3. 对象描述](#123-对象描述)
        - [12.3.1. 对象607Ah：目标位置](#1231-对象607ah目标位置)
        - [12.3.2. 对象607Bh：位置范围限制](#1232-对象607bh位置范围限制)
        - [12.3.3. 对象607Dh：软件位置限制](#1233-对象607dh软件位置限制)
        - [12.3.4. 对象607Fh：最大规划速度](#1234-对象607fh最大规划速度)
        - [12.3.5. 对象6080h：最大电机速度](#1235-对象6080h最大电机速度)
        - [12.3.6. 对象6081h：规划速度](#1236-对象6081h规划速度)
        - [12.3.7. 对象6082h：结束速度](#1237-对象6082h结束速度)
        - [12.3.8. 对象6083h：规划加速度](#1238-对象6083h规划加速度)
        - [12.3.9. 对象6084h：规划减速](#1239-对象6084h规划减速)
        - [12.3.10. 对象6085h：快速停止减速](#12310-对象6085h快速停止减速)
        - [12.3.11. 对象6086h：运动配置文件类型](#12311-对象6086h运动配置文件类型)
        - [12.3.12. 对象60C5h：最大加速度](#12312-对象60c5h最大加速度)
        - [12.3.13. 对象60C6h：最大减速度](#12313-对象60c6h最大减速度)
    - [12.4. 功能描述](#124-功能描述)
- [13. 回归/回原模式](#13-回归回原模式)
    - [13.1. 一般信息](#131-一般信息)
        - [13.1.1. 输入数据描述](#1311-输入数据描述)
        - [13.1.2. 输出数据说明](#1312-输出数据说明)
        - [13.1.3. 内部状态](#1313-内部状态)
    - [13.2. 对象字典条目](#132-对象字典条目)
        - [13.2.1. 本章定义的对象](#1321-本章定义的对象)
        - [13.2.2. 其他章节中定义的对象](#1322-其他章节中定义的对象)
    - [13.3. 对象描述](#133-对象描述)
        - [13.3.1. 对象607Ch：原点偏移](#1331-对象607ch原点偏移)
        - [13.3.2. 对象6098h：回归/回原方法](#1332-对象6098h回归回原方法)
        - [13.3.3. 对象6099h：回归/回原速度](#1333-对象6099h回归回原速度)
        - [13.3.4. 对象609Ah：回归/回原加速度](#1334-对象609ah回归回原加速度)
    - [13.4. 功能描述](#134-功能描述)
        - [13.4.1. 回归/回原方法](#1341-回归回原方法)
- [14. 位置控制功能](#14-位置控制功能)
    - [14.1. 一般信息](#141-一般信息)
        - [14.1.1. 跟随/跟踪错误](#1411-跟随跟踪错误)
        - [14.1.2. 到达位置](#1412-到达位置)
        - [14.1.3. 输入数据描述](#1413-输入数据描述)
        - [14.1.4. 输出数据描述](#1414-输出数据描述)
    - [14.2. 对象字典条目](#142-对象字典条目)
        - [14.2.1. 本章定义的对象](#1421-本章定义的对象)
        - [14.2.2. 其他章节中定义的对象](#1422-其他章节中定义的对象)
    - [14.3. 对象描述](#143-对象描述)
        - [14.3.1. 对象6062h：位置需求值](#1431-对象6062h位置需求值)
        - [14.3.2. 对象6063h：定位实际值*](#1432-对象6063h定位实际值)
        - [14.3.3. 对象6064h：定位实际值](#1433-对象6064h定位实际值)
        - [14.3.4. 对象6065h：跟随/跟踪错误窗口](#1434-对象6065h跟随跟踪错误窗口)
        - [14.3.5. 对象6066h：跟随/跟踪超时错误](#1435-对象6066h跟随跟踪超时错误)
        - [14.3.6. 对象6067h：位置窗口](#1436-对象6067h位置窗口)
        - [14.3.7. 对象6068h：位置窗口时间](#1437-对象6068h位置窗口时间)
        - [14.3.8. 对象60F4h：跟随错误实际值](#1438-对象60f4h跟随错误实际值)
        - [14.3.9. 对象60FAh：控制工作](#1439-对象60fah控制工作)
        - [14.3.10. 对象60FBh：位置控制参数集](#14310-对象60fbh位置控制参数集)
        - [14.3.11. 对象60FCh：位置需求值*](#14311-对象60fch位置需求值)
    - [14.4. 功能说明](#144-功能说明)
- [15 插补/插值位置模式  *（？歧义*](#15-插补插值位置模式--歧义)
    - [15.1 一般信息](#151-一般信息)
        - [15.1.1 输入数据描述](#1511-输入数据描述)
        - [15.1.2 输出数据描述](#1512-输出数据描述)
        - [15.1.3 内部状态](#1513-内部状态)
    - [15.2 复合数据类型](#152-复合数据类型)
        - [15.2.1 插值时间周期记录  *（？歧义*](#1521-插值时间周期记录--歧义)
        - [15.2.2 插值数据配置记录](#1522-插值数据配置记录)
    - [15.3 对象字典条目](#153-对象字典条目)
        - [15.3.1 本章定义的对象](#1531-本章定义的对象)
        - [15.3.2 其他章节中定义的对象](#1532-其他章节中定义的对象)
    - [15.4 对象描述](#154-对象描述)
        - [15.4.1 对象60C0h：插值子模式选择](#1541-对象60c0h插值子模式选择)
        - [15.4.2 对象60C1h：插值数据记录](#1542-对象60c1h插值数据记录)
        - [15.4.3 对象60C2h：插值时间周期](#1543-对象60c2h插值时间周期)
        - [15.4.4 对象60C3h：插值同步定义](#1544-对象60c3h插值同步定义)
        - [15.4.5 对象60C4h：插值数据配置](#1545-对象60c4h插值数据配置)
    - [15.5 功能描述](#155-功能描述)
        - [15.5.1 插值位置模式](#1551-插值位置模式)
        - [15.5.2 带有多个轴的线性插补位置模式](#1552-带有多个轴的线性插补位置模式)
        - [15.5.3 插值位置模式的缓冲策略](#1553-插值位置模式的缓冲策略)
- [16.规划速度模式](#16规划速度模式)
    - [16.1. 一般信息](#161-一般信息)
        - [16.1.1. 输入数据描述](#1611-输入数据描述)
        - [16.1.2. 输出数据描述](#1612-输出数据描述)
        - [16.1.3. 内部状态](#1613-内部状态)
    - [16.2. 对象字典条目](#162-对象字典条目)
        - [16.2.1. 本章定义的对象](#1621-本章定义的对象)
        - [16.2.2. 其他章节中定义的对象](#1622-其他章节中定义的对象)
    - [16.3. 对象描述](#163-对象描述)
        - [16.3.1. 对象6069h：速度传感器实际值](#1631-对象6069h速度传感器实际值)
        - [16.3.2. 对象606Ah：传感器选择代码](#1632-对象606ah传感器选择代码)
        - [16.3.3. 对象606Bh：速度需求值](#1633-对象606bh速度需求值)
        - [16.3.4. 对象606Ch：速度实际值](#1634-对象606ch速度实际值)
        - [16.3.5. 对象606Dh：速度窗口](#1635-对象606dh速度窗口)
        - [16.3.6. 对象606Eh：速度窗口时间](#1636-对象606eh速度窗口时间)
        - [16.3.7. 对象606Fh：速度阈值](#1637-对象606fh速度阈值)
        - [16.3.8. 对象6070h：速度阈值时间](#1638-对象6070h速度阈值时间)
        - [16.3.9. 对象60FFh：目标速度](#1639-对象60ffh目标速度)
        - [16.3.10. 对象60F8h：最大滑点](#16310-对象60f8h最大滑点)
        - [16.3.11. 对象60F9h：速度控制参数集](#16311-对象60f9h速度控制参数集)
    - [16.4. 功能说明](#164-功能说明)
- [17.规划扭矩模式](#17规划扭矩模式)
    - [17.1. 一般信息](#171-一般信息)
        - [17.1.1. 内部状态](#1711-内部状态)
    - [17.2. 对象字典条目](#172-对象字典条目)
        - [17.2.1. 本章定义的对象](#1721-本章定义的对象)
        - [17.2.2. 其他章节中定义的对象](#1722-其他章节中定义的对象)
    - [17.3. 对象描述](#173-对象描述)
        - [17.3.1. 对象6071h：目标扭矩](#1731-对象6071h目标扭矩)
        - [17.3.2. 对象6072h：最大扭矩](#1732-对象6072h最大扭矩)
        - [17.3.3. 对象6073h：最大电流](#1733-对象6073h最大电流)
        - [17.3.4. 对象6074h：扭矩需求值](#1734-对象6074h扭矩需求值)
        - [17.3.5. 对象6075h：电机额定电流](#1735-对象6075h电机额定电流)
        - [17.3.6. 对象6076h：电机额定转矩](#1736-对象6076h电机额定转矩)
        - [17.3.7. 对象6077h：扭矩实际值](#1737-对象6077h扭矩实际值)
        - [17.3.8. 对象6078h：当前实际扭矩值](#1738-对象6078h当前实际扭矩值)
        - [17.3.9. 对象6079h：直流链路电路电压](#1739-对象6079h直流链路电路电压)
        - [17.3.10. 对象6087h：扭矩斜率](#17310-对象6087h扭矩斜率)
        - [17.3.11. 对象6088h：扭矩配置文件类型](#17311-对象6088h扭矩配置文件类型)
        - [17.3.12. 对象60F7h：功率级参数](#17312-对象60f7h功率级参数)
        - [17.3.13. 对象60F6h：转矩控制参数](#17313-对象60f6h转矩控制参数)
- [18.速度模式](#18速度模式)
    - [18.1. 一般说明](#181-一般说明)
        - [18.1.1. 输入数据描述](#1811-输入数据描述)
        - [18.1.2. 输出数据描述](#1812-输出数据描述)
        - [18.1.3. 速度模式的结构](#1813-速度模式的结构)
        - [18.1.4. 子功能描述](#1814-子功能描述)
        - [18.1.5. 内部状态](#1815-内部状态)
    - [18.2. 复合数据类型](#182-复合数据类型)
        - [18.2.1.  vl速度加速减速记录](#1821--vl速度加速减速记录)
    - [18.3. 对象字典条目](#183-对象字典条目)
        - [18.3.1. 本章定义的对象](#1831-本章定义的对象)
        - [18.3.2. 其他章节中定义的对象](#1832-其他章节中定义的对象)
    - [18.4. 对象描述](#184-对象描述)
        - [18.4.1. 对象6042h：vl目标速度](#1841-对象6042hvl目标速度)
        - [18.4.2. 对象6043h：vl速度需求](#1842-对象6043hvl速度需求)
        - [18.4.3. 对象6053h：vl百分比需求](#1843-对象6053hvl百分比需求)
        - [18.4.4. 对象6054h：vl实际百分比](#1844-对象6054hvl实际百分比)
        - [18.4.5. 对象6055h：vl操纵百分比](#1845-对象6055hvl操纵百分比)
        - [18.4.6. 对象604Eh：vl速度参考](#1846-对象604ehvl速度参考)
        - [18.4.7. 对象604Ch：vl单位因子](#1847-对象604chvl单位因子)
        - [18.4.8. 对象604Bh：vl设定点因子](#1848-对象604bhvl设定点因子)
        - [18.4.9. 对象604Dh：vl极数](#1849-对象604dhvl极数)
        - [18.4.10. 对象6046h：vl速度最小最大量](#18410-对象6046hvl速度最小最大量)
        - [18.4.11. 对象6047h：vl速度最小值](#18411-对象6047hvl速度最小值)
        - [18.4.12. 对象6058h：vl频率电机最小最大量](#18412-对象6058hvl频率电机最小最大量)
        - [18.4.13.对象6059h：vl频率电动机最大最大值](#18413对象6059hvl频率电动机最大最大值)
        - [18.4.14. 对象6056h：vl速度电机最小最大量](#18414-对象6056hvl速度电机最小最大量)
        - [18.4.15. 对象6057h：vl速度电机最大最大值](#18415-对象6057hvl速度电机最大最大值)
        - [18.4.16. 对象6048h：vl速度加速度](#18416-对象6048hvl速度加速度)
        - [18.4.17. 对象6049h：vl速度减速度](#18417-对象6049hvl速度减速度)
        - [18.4.18. 对象604Ah：vl快速停止速度](#18418-对象604ahvl快速停止速度)
        - [18.4.19. 对象604Fh：vl斜坡函数时间](#18419-对象604fhvl斜坡函数时间)
        - [18.4.20. 对象6050h：vl减速时间](#18420-对象6050hvl减速时间)
        - [18.4.21. 对象6051h：vl快速停止时间](#18421-对象6051hvl快速停止时间)
        - [18.4.22. 对象6044h：vl控制工作](#18422-对象6044hvl控制工作)
        - [18.4.23. 对象6045h：vl操纵速度](#18423-对象6045hvl操纵速度)
        - [18.4.24. 对象6052h：vl名义百分比](#18424-对象6052hvl名义百分比)
    - [18.5. 功能说明](#185-功能说明)
        - [18.5.1. 百分比函数](#1851-百分比函数)
        - [18.5.2. 因子函数和反向因子函数](#1852-因子函数和反向因子函数)
        - [18.5.3. 极数功能](#1853-极数功能)
        - [18.5.4. 速度限制功能](#1854-速度限制功能)
        - [18.5.5. 速度电机限制功能](#1855-速度电机限制功能)
        - [18.5.6. 斜率/斜坡功能](#1856-斜率斜坡功能)
        - [18.5.7. 最小斜率/斜坡功能](#1857-最小斜率斜坡功能)
        - [18.5.8. 参考计算](#1858-参考计算)
        - [18.5.9. 闭环开环控制功能](#1859-闭环开环控制功能)
- [19.附录](#19附录)
    - [19.1. 对象字典](#191-对象字典)
        - [19.1.1. 常见条目](#1911-常见条目)
        - [19.1.2. 设备控制](#1912-设备控制)
        - [19.1.3. 因素组](#1913-因素组)
        - [19.1.4. 规划位置模式](#1914-规划位置模式)
        - [19.1.5. 回原模式](#1915-回原模式)
        - [19.1.6. 位置控制功能](#1916-位置控制功能)
        - [19.1.7. 插值位置模式](#1917-插值位置模式)
        - [19.1.8. 规划速度模式](#1918-规划速度模式)
        - [19.1.9. 规划扭矩模式](#1919-规划扭矩模式)
        - [19.1.10. 速度模式](#19110-速度模式)
    - [19.2. 对象字典的索引](#192-对象字典的索引)
    - [19.3. 对象字典的名称](#193-对象字典的名称)
    - [19.4. 符号和单位的定义](#194-符号和单位的定义)
        - [19.4.1. 单位索引表](#1941-单位索引表)
        - [19.4.2. 符号索引表](#1942-符号索引表)

<!-- /TOC -->
---

## 1. 范围								 
>SCOPE 
	
[返回目录](#目录)  
  
---

## 2. 参考文件/引用 
>REFERENCES 
	
[返回目录](#目录)  
  
---

## 3. 定义和缩写 
>DEFINITIONS AND ABBREVIATION 
	
[返回目录](#目录)  
  
---

## 4. 概述
>OVERVIEW

### 	4.1. 访问驱动器 
>Access to the drive 

### 	4.2. 驱动器架构 
>Architecture of the drive 
	
[返回目录](#目录)  
  
---

## 5. 工作原理  
>OPERATING PRINCIPLE

### 	5.1. 引言/介绍 
>Introduction 
	
### 	5.2. 通过分析进行标准化 
>Standardization via profiling. 
	
### 	5.3. 对象字典 
>The object dictionary 
	
####		5.3.1. 索引和子索引的使用 
>Index and sub-index usage 
		
[返回目录](#目录)  
  
---

## 6. 紧急消息 
>EMERGENCY MESSAGES. 
 
### 	6.1. 原则/原理 *（？歧义* 
>Principle 

### 	6.2. 错误代码 
>Error codes 
	
[返回目录](#目录)  
  
---

## 7. 预定义 
>PREDEFINITIONS 

### 	7.1. 预定义对象 
>Predefined objects 

####		7.1.1. 对象1000 h:设备类型
>Object 1000 h : Device type

####		7.1.2. 对象1001 h:错误寄存器 
>Object 1001 h : Error register 
		
####		7.1.3. 对象67FF h:单一设备类型 
>Object 67FF h : Single device type 
	
### 	7.2. PDO映射 
>PDO mapping 
	
####		7.2.1. 接收pdo 
>Receive PDOs 
		
####		7.2.2. 发送pdo 
>Transmit PDOs 
		
[返回目录](#目录)  
  
---

## 8. 对象字典 
>OBJECT DICTIONARY 
	
[返回目录](#目录)  
  
---

## 9. 共同条目/常见条目 
>COMMON ENTRIES
	
### 	9.1. 一般信息
>General information 

####		9.1.1. 电机数据	
>Motor data
	
####		9.1.2. 驱动器数据	
>Drive data
	
### 	9.2. 对象字典条目	
>Object dictionary entries

####		9.2.1本章定义的对象	 
>Objects defined in this chapter

### 	9.3. 对象描述	 
>Object description

  ####		9.3.1. 对象6007 h：中止连接选项代​​码  
>Object 6007 h : Abort connection option code

####		9.3.2. 对象603F h：错误代码	
>Object 603F h : Error code

####		9.3.3. 对象6402 h：电机类型  
>Object 6402 h : Motor type

####		9.3.4. 对象6403 h：电机目录号	
>Object 6403 h : Motor catalog number

####		9.3.5. 对象6404 h：电机制造商  
>Object 6404 h : Motor manufacturer

####		9.3.6. 对象6405 h：http电机目录地址	
>Object 6405 h : http motor catalog address

####		9.3.7. 对象6406 h：电机校准日期   
>Object 6406 h : Motor calibration date

####		9.3.8. 对象6407 h：电机服务期   
>Object 6407 h : Motor service period

####		9.3.9. 对象6410 h：电机数据	 
>Object 6410 h : Motor data

####		9.3.10. 对象6502 h：支持的驱动模式   
>Object 6502 h : Supported drive modes

####		9.3.11. 对象6503 h：驱动器目录号   
>Object 6503 h : Drive catalog number

####		9.3.12. 对象6504 h：驱动器制造商  
>Object 6504 h : Drive manufacturer

####		9.3.13. 对象6505 h：http驱动器目录地址  
>Object 6505 h : http drive catalog address

####		9.3.14. 对象6510 h：驱动数据  
>Object 6510 h : Drive data

####		9.3.15. 对象60FD h：数字输入	
>Object 60FD h : Digital inputs

####		9.3.16. 对象60FE h：数字输出  
>Object 60FE h : Digital outputs
		
[返回目录](#目录)  
  
---

## 10. 设备控制  
>DEVICE CONTROL

### 	10.1. 一般/通用信息  
>General information	

####		10.1.1. 状态机   
> State machine

### 	10.2. 对象字典条目	
>Object dictionary entries

####		10.2.1本章定义的对象	 
>Objects defined in this chapter.

### 	10.3. 对象描述	 
>Object description

####		10.3.1. 对象6040 h：控制字   
>Object 6040 h : Controlword

####		10.3.2. 对象6041 h：状态字	 
>Object 6041 h : Statusword
		
####		10.3.3. 对象605B h：关闭选项代码  
>Object 605B h : Shutdown option code 

####		10.3.4. 对象605C h：禁用操作选项代码	
>Object 605C h : Disable operation option code

####		10.3.5. 对象605A h：快速停止/急停 选项代码   
>Object 605A h : Quick stop option code

####		10.3.6. 对象605D h：暂停选项代码	
>Object 605D h : Halt option code

####		10.3.7. 对象605E h：故障反应选项代码  
>Object 605E h : Fault reaction option code

####		10.3.8. 对象6060 h：操作模式   
>Object 6060 h : Modes of operation

####		10.3.9. 对象6061h：操作模式显示  
>Object 6061h : Modes of operation display

### 	10.4. 功能描述	
>Functional description

####		10.4.1. 操作模式功能  
>Modes of operation function

####		10.4.2. 驱动器禁用功能/驱动器禁能	
>Drive disabling function

####		10.4.3. 快速停止功能/急停	
>Quick stop function 

####		10.4.4. 停止功能   
>Stop function

####		10.4.5. 故障反应	 
>Fault reaction
		
[返回目录](#目录)  
  
---

## 11. 因素组/影响参数/影响因子  *（？歧义*
>FACTOR GROUP  
  
### 	11.1. 一般信息  
>General information  
	
####		11.1.1. 因素/参数/影响因子  *（？歧义*
>Factors  
		
####		11.1.2. 物理/物理单位 和内部单位之间的关系  *（？歧义*
>Relationship between physical and internal units  
		
### 	11.2. 对象字典条目/对象字典映射表  
>Object dictionary entries  
		
####		11.2.1. 本章定义的对象  
>Objects defined in this chapter  
	
### 	11.3. 对象描述  
>Object description  
	
####		11.3.1. 对象6089h：位置符号索引  *（？歧义*
>Object 6089h: Position notation index  
		
####		11.3.2. 对象608Ah：位置单位索引  *（？歧义*
>Object 608Ah: Position dimension index  
		
####		11.3.3. 对象608Bh：速度符号索引  *（？歧义*
>Object 608Bh: Velocity notation index  
		
####		11.3.4. 对象608C h：速度单位指数索引  *（？歧义*
>Object 608C h: Velocity dimension index  
		
####		11.3.5. 对象608D h：加速度表示法指数索引  *（？歧义*
>Object 608D h: Acceleration notation index  
		
####		11.3.6. 对象608Eh：加速单位指数索引  *（？歧义*
>Object 608Eh: Acceleration dimension index  
		
####		11.3.7. 对象608Fh：位置编码器分辨率  
>Object 608Fh: Position encoder resolution  
		
####		11.3.8. 对象6090h：速度编码器分辨率  
>Object 6090h: Velocity encoder resolution  
		
####		11.3.9. 对象6091h：齿轮比  
>Object 6091h: Gear ratio  
		
####		11.3.10. 对象6092h：进给常数.​​  
>Object 6092h: Feed constant  
		
####		11.3.11. 对象6093h：位置因子  
>Object 6093h: Position factor  
		
####		11.3.12. 对象6094h：速度编码器因子  
>Object 6094h: Velocity encoder factor  
		
####		11.3.13. 对象6095h：速度因子1  
>Object 6095h: Velocity factor 1  
		
####		11.3.14. 物体6096h：速度因子2  
>Object 6096h: Velocity factor 2  
		
####		11.3.15. 对象6097h：加速因子  
>Object 6097h: Acceleration factor  
		
####		11.3.16. 对象607Eh：极性  
>Object 607Eh: Polarity  
[返回目录](#目录)  
  
---

## 12. 规划位置模式
>PROFILE POSITION MODE  

### 	12.1. 一般信息
>General information  

####		12.1.1. 输入数据描述
>Input data description  

####		12.1.2. 输出数据说明
>Output data description  

####		12.1.3. 内部状态
>Internal states  

### 	12.2. 对象字典条目
>Object dictionary entries  

####		12.2.1. 本章定义的对象
>Objects defined in this chapter  

####		12.2.2. 其他章节中定义的对象
>Objects defined in other chapters  

### 	12.3. 对象描述
>Object description  

####		12.3.1. 对象607Ah：目标位置
>Object 607Ah: Target position  

####		12.3.2. 对象607Bh：位置范围限制
>Object 607Bh: Position range limit  

####		12.3.3. 对象607Dh：软件位置限制
>Object 607Dh: Software position limit  

####		12.3.4. 对象607Fh：最大规划速度
>Object 607Fh: Max profile velocity  

####		12.3.5. 对象6080h：最大电机速度
>Object 6080h: Max motor speed  

####		12.3.6. 对象6081h：规划速度
>Object 6081h: Profile velocity  

####		12.3.7. 对象6082h：结束速度
>Object 6082h: End velocity  

####		12.3.8. 对象6083h：规划加速度
>Object 6083h: Profile acceleration  

####		12.3.9. 对象6084h：规划减速度
>Object 6084h: Profile deceleration  

####		12.3.10. 对象6085h：快速停止减速
>Object 6085h: Quick stop deceleration  

####		12.3.11. 对象6086h：运动配置文件类型
>Object 6086h: Motion profile type  

####		12.3.12. 对象60C5h：最大加速度
>Object 60C5h: Max acceleration  

####		12.3.13. 对象60C6h：最大减速度
>Object 60C6h: Max deceleration  

### 	12.4. 功能描述
>Functional description  

[返回目录](#目录)  
  
---

## 13. 回归/回原模式
>HOMING MODE  

### 	13.1. 一般信息
>General information  

####		13.1.1. 输入数据描述
>Input data description  

####		13.1.2. 输出数据说明
>Output data description  

####		13.1.3. 内部状态
>Internal states  

### 	13.2. 对象字典条目
>Object dictionary entries  

####		13.2.1. 本章定义的对象
>Objects defined in this chapter  

####		13.2.2. 其他章节中定义的对象
>Objects defined in other chapters  

### 	13.3. 对象描述
>Object description  

####		13.3.1. 对象607Ch：原点偏移
>Object 607Ch: Home offset  

####		13.3.2. 对象6098h：回归/回原方法
>Object 6098h: Homing method  

####		13.3.3. 对象6099h：回归/回原速度
>Object 6099h: Homing speeds  

####		13.3.4. 对象609Ah：回归/回原加速度
>Object 609Ah: Homing acceleration  

### 	13.4. 功能描述
>Functional description  

####		13.4.1. 回归/回原方法
>Homing methods 
		
[返回目录](#目录)  
  
---
	
## 14. 位置控制功能  
>POSITION CONTROL FUNCTION

### 	14.1. 一般信息  
>General information 

####		14.1.1. 跟随/跟踪错误   
>Following error

####		14.1.2. 到达位置  
>Position reached

####		14.1.3. 输入数据描述  
>Input data description

####		14.1.4. 输出数据描述  
>Output data description 

### 	14.2. 对象字典条目  
>Object dictionary entries

####		14.2.1. 本章定义的对象  
>Objects defined in this chapter

####		14.2.2. 其他章节中定义的对象  
>Objects defined in other chapters

### 	14.3. 对象描述  
>Object description

####		14.3.1. 对象6062h：位置需求值  
>Object 6062h: Position demand value

####		14.3.2. 对象6063h：定位实际值*  
>Object 6063h: Position actual value*

####		14.3.3. 对象6064h：定位实际值  
>Object 6064h: Position actual value 

####		14.3.4. 对象6065h：跟随/跟踪错误窗口  
>Object 6065h: Following error window
		
####		14.3.5. 对象6066h：跟随/跟踪超时错误  
>Object 6066h: Following error time out
		
####		14.3.6. 对象6067h：位置窗口  
>Object 6067h: Position window
		
####		14.3.7. 对象6068h：位置窗口时间  
>Object 6068h : Position window time
		
####		14.3.8. 对象60F4h：跟随错误实际值  
>Object 60F4h: Following error actual value
		
####		14.3.9. 对象60FAh：控制工作  
>Object 60FAh: Control effort
		
####		14.3.10. 对象60FBh：位置控制参数集  
>Object 60FBh: Position control parameter set
		
####		14.3.11. 对象60FCh：位置需求值*  
>Object 60FCh: Position demand value*
		
### 	14.4. 功能说明
>Functional description 

[返回目录](#目录) 
  
---

## 15 插补/插值位置模式  *（？歧义*  
>INTERPOLATED POSITION MODE
  
### 	15.1 一般信息  
>General information   
	
####		15.1.1 输入数据描述  
>Input data description  
		
####		15.1.2 输出数据描述  
>Output data description   
		
####		15.1.3 内部状态  
>Internal states  
		
### 	15.2 复合数据类型  
>Complex data types   
	
####		15.2.1 插值时间周期记录  *（？歧义*   
>Interpolation time period record  
		
####		15.2.2 插值数据配置记录  
>Interpolation data configuration record  
		
### 	15.3 对象字典条目  
>Object dictionary entries  
	
####		15.3.1 本章定义的对象  
>Objects defined in this chapter  
		
####		15.3.2 其他章节中定义的对象  
>Objects defined in other chapters  
		
### 	15.4 对象描述  
>Object descriptions   
	
####		15.4.1 对象60C0h：插值子模式选择  
>Object h: Interpolation sub mode select   
		
####		15.4.2 对象60C1h：插值数据记录  
>Object h: Interpolation data record  
		
####		15.4.3 对象60C2h：插值时间周期  
>Object h: Interpolation time period   
		
####		15.4.4 对象60C3h：插值同步定义  
>Object h: Interpolation sync definition  
		
####		15.4.5 对象60C4h：插值数据配置  
>Object h: Interpolation data configuration   
		
### 	15.5 功能描述  
>Functional description   
	
####		15.5.1 插值位置模式  
>Interpolated position mode   
		
####		15.5.2 带有多个轴的线性插补位置模式  
>Linear interpolated position mode with several axles   
		
####		15.5.3 插值位置模式的缓冲策略  
>Buffer strategies for the interpolated position mode  

[返回目录](#目录) 
  
---

##  16.规划速度模式  
>PROFILE VELOCITY MODE  
  
###		 16.1. 一般信息  
>General Information  

####		16.1.1. 输入数据描述  
>Input data description  
  
####		16.1.2. 输出数据描述  
>Output data description  
  
####		16.1.3. 内部状态  
>Internal states  
  
###		 16.2. 对象字典条目  
> Object dictionary entries  
  
####		16.2.1. 本章定义的对象  
>Objects defined in this chapter  
  
####		16.2.2. 其他章节中定义的对象  
>Objects defined in other chapters  
  
###		 16.3. 对象描述  
>Object description  
  
####		16.3.1. 对象6069h：速度传感器实际值  
>Object 6069h: Velocity sensor actual value  
  
####		16.3.2. 对象606Ah：传感器选择代码  
>Object 606Ah: Sensor selection code  
  
####		16.3.3. 对象606Bh：速度需求值  
>Object 606Bh: Velocity demand value  
  
####		16.3.4. 对象606Ch：速度实际值  
>Object 606Ch: Velocity actual value  
  
####		16.3.5. 对象606Dh：速度窗口  
>Object 606Dh: Velocity window  
  
####		16.3.6. 对象606Eh：速度窗口时间  
>Object 606Eh: Velocity window time  
  
####		16.3.7. 对象606Fh：速度阈值  
> Object 606Fh: Velocity threshold  
  
####		16.3.8. 对象6070h：速度阈值时间  
>Object 6070h: Velocity threshold time  
  
####		16.3.9. 对象60FFh：目标速度  
>Object 60FFh: Target velocity  
  
####		16.3.10. 对象60F8h：最大滑点  
>Object 60F8h: Max slippage  
  
####		16.3.11. 对象60F9h：速度控制参数集  
>Object 60F9h: Velocity control parameter set  
  
###		 16.4. 功能说明  
>Functional description  
  
[返回目录](#目录) 
  
---


##  17.规划扭矩模式  
>PROFILE TORQUE MODE  
  
###		 17.1. 一般信息  
>General information  
  
####		17.1.1. 内部状态  
>Internal states  
  
###		 17.2. 对象字典条目  
>Object dictionary entries  
  
####		17.2.1. 本章定义的对象  
>Objects defined in this chapter  
  
####		17.2.2. 其他章节中定义的对象  
> Objects defined in other chapters  
  
###		 17.3. 对象描述  
>Object description  
  
####		17.3.1. 对象6071h：目标扭矩  
>Object 6071h: Target torque  
  
####		17.3.2. 对象6072h：最大扭矩  
>Object 6072h: Max torque  
  
####		17.3.3. 对象6073h：最大电流  
>Object 6073h: Max current  
  
####		17.3.4. 对象6074h：扭矩需求值  
>Object 6074h: Torque demand value  
  
####		17.3.5. 对象6075h：电机额定电流  
>Object 6075h: Motor rated current  
  
####		17.3.6. 对象6076h：电机额定转矩  
>Object 6076h: Motor rated torque  
  
####		17.3.7. 对象6077h：扭矩实际值  
>Object 6077h: Torque actual value  
  
####		17.3.8. 对象6078h：当前实际扭矩值  
>Object 6078h: Current actual value  
  
####		17.3.9. 对象6079h：直流链路电路电压  
>Object 6079h: DC link circuit voltage  
  
####		17.3.10. 对象6087h：扭矩斜率  
>Object 6087h: Torque slope  
  
####		17.3.11. 对象6088h：扭矩配置文件类型  
>Object 6088h: Torque profile type  
  
####		17.3.12. 对象60F7h：功率级参数  
> Object 60F7h: Power stage parameters  
  
####		17.3.13. 对象60F6h：转矩控制参数  
>Object 60F6h: Torque control parameters  
  
[返回目录](#目录) 
  
---


##  18.速度模式  
>VELOCITY MODE  
  
###		 18.1. 一般说明  
>General description  
  
####		18.1.1. 输入数据描述  
>Input data description  
  
####		18.1.2. 输出数据描述  
>Output data description  
  
####		18.1.3. 速度模式的结构  
>Structure of the velocity mode  
  
####		18.1.4. 子功能描述  
>Subfunction description  
  
####		18.1.5. 内部状态  
>Internal states  
  
###		 18.2. 复合数据类型  
>Complex data types  
  
####		18.2.1.  vl速度加速减速记录  
>vl velocity acceleration deceleration record  
  
###		 18.3. 对象字典条目  
>Object dictionary entries  
  
####		18.3.1. 本章定义的对象  
>Objects defined in this chapter  
  
####		18.3.2. 其他章节中定义的对象  
>Objects defined in other chapters  
  
###		 18.4. 对象描述  
>Object description  
  
####		18.4.1. 对象6042h：vl目标速度  
>Object 6042h: vl target velocity  
  
####		18.4.2. 对象6043h：vl速度需求  
>Object 6043h: vl velocity demand  
  
####		18.4.3. 对象6053h：vl百分比需求  
>Object 6053h: vl percentage demand  
  
####		18.4.4. 对象6054h：vl实际百分比  
>Object 6054h: vl actual percentage  
  
####		18.4.5. 对象6055h：vl操纵百分比  
>Object 6055h: vl manipulated percentage  

####		18.4.6. 对象604Eh：vl速度参考  
>Object 604Eh: vl velocity reference  
  
####		18.4.7. 对象604Ch：vl单位因子  
>Object 604Ch: vl dimension factor  
  
####		18.4.8. 对象604Bh：vl设定点因子  
>Object 604Bh: vl setpoint factor  
  
####		18.4.9. 对象604Dh：vl极数  
>Object 604Dh: vl pole number  
  
####		18.4.10. 对象6046h：vl速度最小最大量  
>Object 6046h: vl velocity min max amount  
  
####		18.4.11. 对象6047h：vl速度最小值  
>Object 6047h: vl velocity min max  
  
####		18.4.12. 对象6058h：vl频率电机最小最大量  
>Object 6058h: vl frequency motor min max amount  
  
####		18.4.13.对象6059h：vl频率电动机最大最大值  
>Object 6059h: vl frequency motor min max  
  
####		18.4.14. 对象6056h：vl速度电机最小最大量  
>Object 6056h: vl velocity motor min max amount  
  
####		18.4.15. 对象6057h：vl速度电机最大最大值  
>Object 6057h: vl velocity motor min max  
  
####		18.4.16. 对象6048h：vl速度加速度  
>Object 6048h: vl velocity acceleration  
  
####		18.4.17. 对象6049h：vl速度减速度 
>Object 6049h: vl velocity deceleration  
  
####		18.4.18. 对象604Ah：vl快速停止速度  
>Object 604Ah: vl velocity quick stop  
  
####		18.4.19. 对象604Fh：vl斜坡函数时间  
>Object 604Fh: vl ramp function time  
  
####		18.4.20. 对象6050h：vl减速时间  
>Object 6050h: vl slow down time  
  
####		18.4.21. 对象6051h：vl快速停止时间  
>Object 6051h: vl quick stop time  
  
####		18.4.22. 对象6044h：vl控制工作  
>Object 6044h: vl control effort  
  
####		18.4.23. 对象6045h：vl操纵速度  
>Object 6045h: vl manipulated velocity  
  
####		18.4.24. 对象6052h：vl名义百分比  
>Object 6052h: vl nominal percentage  
  
###		 18.5. 功能说明  
>Functional description  
  
####		18.5.1. 百分比函数  
>Percentage function  
  
####		18.5.2. 因子函数和反向因子函数  
>Factor function and reverse factor function  
  
####		18.5.3. 极数功能  
>Pole number function  
  
####		18.5.4. 速度限制功能  
>Velocity limit function  
  
####		18.5.5. 速度电机限制功能  
>Velocity motor limit function  
  
####		18.5.6. 斜率/斜坡功能  
>Ramp function  
  
####		18.5.7. 最小斜率/斜坡功能  
>Ramp min function  
  
####		18.5.8. 参考计算  
>Reference calculation  
  
####		18.5.9. 闭环开环控制功能  
>Closed open loop control function  
  
[返回目录](#目录) 
  
---


##  19.附录  
>APPENDIX  
  
###		 19.1. 对象字典  
>Object dictionary by chapter  
  
####		19.1.1. 常见条目  
>Common Entries  

####		19.1.2. 设备控制  
>Device Control  
  
####		19.1.3. 因素组  
>Factor Group  
  
####		19.1.4. 规划位置模式  
>Profile Position Mode  
  
####		19.1.5. 回原模式  
>Homing Mode  
  
####		19.1.6. 位置控制功能  
>Position control function  
  
####		19.1.7. 插值位置模式  
>Interpolated position mode  
  
####		19.1.8. 规划速度模式  
>Profile velocity mode  
  
####		19.1.9. 规划扭矩模式  
>Profile Torque Mode  
  
####		19.1.10. 速度模式  
>Velocity Mode  
  
###		 19.2. 对象字典的索引  
>Object dictionary by index  
  
###		 19.3. 对象字典的名称  
>Object dictionary by name  
  
###		 19.4. 符号和单位的定义   
>Definition of dimension indices  
  
####		19.4.1. 单位索引表  
>Dimension index table  
  
####		19.4.2. 符号索引表  
>Notation index table 

		
[返回目录](#目录) 
  
---

