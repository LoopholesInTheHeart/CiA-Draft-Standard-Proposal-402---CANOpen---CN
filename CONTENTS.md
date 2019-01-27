CONTENTS
===

<!-- TOC -->  
 [1. 范围](#1-范围)  
 [2. 参考文件/引用](#2-参考文件引用)  
 [3. 定义和缩写](#3-定义和缩写)  
 [4. 概述](#4-概述)  
 [5. 工作原理](#5-工作原理)  
 [6. 紧急消息](#6-紧急消息)  
 [7. 预解释](#7-预解释)  
 [8. 对象字典](#8-对象字典)  
 [9. 共同条目/常见条目](#9-共同条目常见条目)  
 [10. 设备控制](#10-设备控制)  
 [11. 因素组/影响参数/影响因子  *（？歧义*](#11-因素组影响参数影响因子--歧义)  
 [12. 轮廓位置模式](#12-轮廓位置模式)  
 [13. 回归/回原模式](#13-回归回原模式)  
 [14. 位置控制功能](#14-位置控制功能)
 <!-- /TOC -->  

---

#### 1. 范围
	>SCOPE 
	
---

#### 2. 参考文件/引用 
	>REFERENCES 
	
---

#### 3. 定义和缩写 
	>DEFINITIONS AND ABBREVIATION 
	
---

#### 4. 概述
	>OVERVIEW

	4.1. 访问驱动器 
	>Access to the drive 

	4.2. 驱动器架构 
	>Architecture of the drive 
	
---

#### 5. 工作原理  
	>OPERATING PRINCIPLE

	5.1. 引言/介绍 
	>Introduction 
	
	5.2. 通过分析进行标准化 
	>Standardization via profiling. 
	
	5.3. 对象字典 
	>The object dictionary 
	
		5.3.1. 索引和子索引的使用 
		>Index and sub-index usage 
		
---

#### 6. 紧急消息 
	>EMERGENCY MESSAGES. 
 
	6.1. 原则/原理 *（？歧义* 
	>Principle 

	6.2. 错误代码 
	>Error codes 
	
---

#### 7. 预解释 
	>PREDEFINITIONS 

	7.1. 预定义对象 
	>Predefined objects 

		7.1.1. 对象1000 h:设备类型
		>Object 1000 h : Device type

		7.1.2. 对象1001 h:错误寄存器 
		>Object 1001 h : Error register 
		
		7.1.3. 对象67FF h:单一设备类型 
		>Object 67FF h : Single device type 
	
	7.2. PDO映射 
	>PDO mapping 
	
		7.2.1. 接收pdo 
		>Receive PDOs 
		
		7.2.2. 发送pdo 
		>Transmit PDOs 
		
---

#### 8. 对象字典 
	>OBJECT DICTIONARY 
	
---

#### 9. 共同条目/常见条目 
	>COMMON ENTRIES
	
	9.1. 一般信息
	>General information 

		9.1.1. 电机数据	
		>Motor data
	
		9.1.2. 驱动数据	
		>Drive data
	
	9.2. 对象字典条目	
	>Object dictionary entries

		9.2.1本章定义的对象	 
		>Objects defined in this chapter

	9.3. 对象描述	 
	>Object description

  		9.3.1. 对象6007 h：中止连接选项代​​码  
		>Object 6007 h : Abort connection option code

		9.3.2. 对象603F h：错误代码	
		>Object 603F h : Error code

		9.3.3. 对象6402 h：电机类型  
		>Object 6402 h : Motor type

		9.3.4. 对象6403 h：电机目录号	
		>Object 6403 h : Motor catalog number

		9.3.5. 对象6404 h：电机制造商  
		>Object 6404 h : Motor manufacturer

		9.3.6. 对象6405 h：http电机目录地址	
		>Object 6405 h : http motor catalog address

		9.3.7. 对象6406 h：电机校准日期   
		>Object 6406 h : Motor calibration date

		9.3.8. 对象6407 h：电机服务期   
		>Object 6407 h : Motor service period

		9.3.9. 对象6410 h：电机数据	 
		>Object 6410 h : Motor data

		9.3.10. 对象6502 h：支持的驱动模式   
		>Object 6502 h : Supported drive modes

		9.3.11. 对象6503 h：驱动器目录号   
		>Object 6503 h : Drive catalog number

		9.3.12. 对象6504 h：驱动器制造商  
		>Object 6504 h : Drive manufacturer

		9.3.13. 对象6505 h：http驱动器目录地址  
		>Object 6505 h : http drive catalog address

		9.3.14. 对象6510 h：驱动数据  
		>Object 6510 h : Drive data

		9.3.15. 对象60FD h：数字输入	
		>Object 60FD h : Digital inputs

		9.3.16. 对象60FE h：数字输出  
		>Object 60FE h : Digital outputs
		
---

#### 10. 设备控制  
	>DEVICE CONTROL

	10.1. 一般/通用信息  
	>General information	

		10.1.1. 状态机   
		> State machine

	10.2. 对象字典条目	
	>Object dictionary entries

		10.2.1本章定义的对象	 
		>Objects defined in this chapter.

	10.3. 对象描述	 
	>Object description

		10.3.1. 对象6040 h：控制字   
		>Object 6040 h : Controlword

		10.3.2. 对象6041 h：状态字	 
		>Object 6041 h : Statusword
		
		10.3.3. 对象605B h：关闭选项代码  
		>Object 605B h : Shutdown option code 

		10.3.4. 对象605C h：禁用操作选项代码	
		>Object 605C h : Disable operation option code

		10.3.5. 对象605A h：快速停止/急停 选项代码   
		>Object 605A h : Quick stop option code

		10.3.6. 对象605D h：暂停选项代码	
		>Object 605D h : Halt option code

		10.3.7. 对象605E h：故障反应选项代码  
		>Object 605E h : Fault reaction option code

		10.3.8. 对象6060 h：操作模式   
		>Object 6060 h : Modes of operation

		10.3.9. 对象6061h：操作模式显示  
		>Object 6061h : Modes of operation display

	10.4. 功能描述	
	>Functional description

		10.4.1. 操作模式功能  
		>Modes of operation function

		10.4.2. 驱动器禁用功能/驱动器禁能	
		>Drive disabling function

		10.4.3. 快速停止功能/急停	
		>Quick stop function 

		10.4.4. 停止功能   
		>Stop function

		10.4.5. 故障反应	 
		>Fault reaction
		
---

#### 11. 因素组/影响参数/影响因子  *（？歧义*
	>FACTOR GROUP  
  
    11.1. 一般信息  
    >General information  
    
        11.1.1. 因素/参数/影响因子  *（？歧义*
        >Factors  
        
        11.1.2. 物理/物理单位 和内部单位之间的关系  *（？歧义*
        >Relationship between physical and internal units  
        
    11.2. 对象字典条目/对象字典映射表  
    >Object dictionary entries  
        
        11.2.1. 本章定义的对象  
        >Objects defined in this chapter  
    
    11.3. 对象描述  
    >Object description  
    
        11.3.1. 对象6089h：位置符号索引  *（？歧义*
        >Object 6089h: Position notation index  
        
        11.3.2. 对象608Ah：位置尺寸索引  *（？歧义*
        >Object 608Ah: Position dimension index  
        
        11.3.3. 对象608Bh：速度符号索引  *（？歧义*
        >Object 608Bh: Velocity notation index  
        
        11.3.4. 对象608C h：速度尺寸指数  *（？歧义*
        >Object 608C h: Velocity dimension index  
        
        11.3.5. 对象608D h：加速度表示法指数  *（？歧义*
        >Object 608D h: Acceleration notation index  
        
        11.3.6. 对象608Eh：加速尺寸指数  *（？歧义*
        >Object 608Eh: Acceleration dimension index  
        
        11.3.7. 对象608Fh：位置编码器分辨率  
        >Object 608Fh: Position encoder resolution  
        
        11.3.8. 对象6090h：速度编码器分辨率  
        >Object 6090h: Velocity encoder resolution  
        
        11.3.9. 对象6091h：齿轮比  
        >Object 6091h: Gear ratio  
        
        11.3.10. 对象6092h：进给常数.​​  
        >Object 6092h: Feed constant  
        
        11.3.11. 对象6093h：位置因子  
        >Object 6093h: Position factor  
        
        11.3.12. 对象6094h：速度编码器因子  
        >Object 6094h: Velocity encoder factor  
        
        11.3.13. 对象6095h：速度因子1  
        >Object 6095h: Velocity factor 1  
        
        11.3.14. 物体6096h：速度因子2  
        >Object 6096h: Velocity factor 2  
        
        11.3.15. 对象6097h：加速因子  
        >Object 6097h: Acceleration factor  
        
        11.3.16. 对象607Eh：极性  
        >Object 607Eh: Polarity  
---

#### 12. 轮廓位置模式
	>PROFILE POSITION MODE  

	12.1. 一般信息
		>General information  

		12.1.1. 输入数据描述
			>Input data description  

		12.1.2. 输出数据说明
			>Output data description  

		12.1.3. 内部状态
			>Internal states  

	12.2. 对象字典条目
	>Object dictionary entries  

		12.2.1. 本章定义的对象
			>Objects defined in this chapter  

		12.2.2. 其他章节中定义的对象
			>Objects defined in other chapters  

	12.3. 对象描述
	>Object description  

		12.3.1. 对象607Ah：目标位置
			>Object 607Ah: Target position  

		12.3.2. 对象607Bh：位置范围限制
			>Object 607Bh: Position range limit  

		12.3.3. 对象607Dh：软件位置限制
			>Object 607Dh: Software position limit  

		12.3.4. 对象607Fh：最大轮廓速度
			>Object 607Fh: Max profile velocity  

		12.3.5. 对象6080h：最大电机速度
			>Object 6080h: Max motor speed  

		12.3.6. 对象6081h：轮廓速度
			>Object 6081h: Profile velocity  

		12.3.7. 对象6082h：结束速度
			>Object 6082h: End velocity  

		12.3.8. 对象6083h：轮廓加速度
			>Object 6083h: Profile acceleration  

		12.3.9. 对象6084h：轮廓减速
			>Object 6084h: Profile deceleration  

		12.3.10. 对象6085h：快速停止减速
			>Object 6085h: Quick stop deceleration  

		12.3.11. 对象6086h：运动配置文件类型
			>Object 6086h: Motion profile type  

		12.3.12. 对象60C5h：最大加速度
			>Object 60C5h: Max acceleration  

		12.3.13. 对象60C6h：最大减速度
			>Object 60C6h: Max deceleration  

	12.4. 功能描述
	>Functional description  

---

#### 13. 回归/回原模式
	>HOMING MODE  

    13.1. 一般信息
        >General information  

        13.1.1. 输入数据描述
            >Input data description  

        13.1.2. 输出数据说明
            >Output data description  

        13.1.3. 内部状态
            >Internal states  

    13.2. 对象字典条目
        >Object dictionary entries  

        13.2.1. 本章定义的对象
            >Objects defined in this chapter  

        13.2.2. 其他章节中定义的对象
            >Objects defined in other chapters  

    13.3. 对象描述
        >Object description  

        13.3.1. 对象607Ch：原点偏移
            >Object 607Ch: Home offset  

        13.3.2. 对象6098h：回归/回原方法
            >Object 6098h: Homing method  

        13.3.3. 对象6099h：回归/回原速度
            >Object 6099h: Homing speeds  

        13.3.4. 对象609Ah：回归/回原加速度
            >Object 609Ah: Homing acceleration  

    13.4. 功能描述
        >Functional description  

        13.4.1. 回归/回原方法
            >Homing methods 
		
---
	
#### 14. 位置控制功能  
	>POSITION CONTROL FUNCTION

	14.1. 一般信息  
	>General information 

		14.1.1. 跟随/跟踪错误   
		>Following error

		14.1.2. 到达位置  
		>Position reached

		14.1.3. 输入数据描述  
		>Input data description

		14.1.4. 输出数据描述  
		>Output data description 

	14.2. 对象字典条目  
	>Object dictionary entries

		14.2.1. 本章定义的对象  
		>Objects defined in this chapter

		14.2.2. 其他章节中定义的对象  
		>Objects defined in other chapters

	14.3. 对象描述  
	>Object description

		14.3.1. 对象6062h：位置需求值  
		>Object 6062h: Position demand value

		14.3.2. 对象6063h：定位实际值*  
		>Object 6063h: Position actual value*

		14.3.3. 对象6064h：定位实际值  
		>Object 6064h: Position actual value 

		14.3.4. 对象6065h：跟随/跟踪错误窗口  
		>Object 6065h: Following error window
		
		14.3.5. 对象6066h：跟随/跟踪超时错误  
		>Object 6066h: Following error time out
		
		14.3.6. 对象6067h：位置窗口  
		>Object 6067h: Position window
		
		14.3.7. 对象6068h：位置窗口时间  
		>Object 6068h : Position window time
		
		14.3.8. 对象60F4h：跟随错误实际值  
		>Object 60F4h: Following error actual value
		
		14.3.9. 对象60FAh：控制工作  
		>Object 60FAh: Control effort
		
		14.3.10. 对象60FBh：位置控制参数集  
		>Object 60FBh: Position control parameter set
		
		14.3.11. 对象60FCh：位置需求值*  
		>Object 60FCh: Position demand value*
		
	14.4. 功能说明
	>Functional description 
