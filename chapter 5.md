
- [5. 工作原理](#5-工作原理)
    - [5.1. 引言/介绍](#51-引言介绍)
    - [5.2. 通过分析进行标准化](#52-通过分析进行标准化)
    - [5.3. 对象字典](#53-对象字典)
        - [5.3.1. 索引和子索引的使用](#531-索引和子索引的使用)


---

## 5. 工作原理  
>OPERATING PRINCIPLE

### 	5.1. 引言/介绍 
>Introduction 

此配置文件的目的是为CAN网络上的驱动器提供可理解且独特的行为。 用于驱动器和运动控制的CANopen设备配置文件建立在称为CANopen的CAN通信配置文件之上，描述了CAN网络中所有设备通用的基本通信机制。
>The purpose of this profile is, to give drives an understandable and unique behavior on the CANnetwork. The CANopen Device Profile for Drives and Motion Control is built on top of a CAN communication profile, called CANopen, describing the basic communication mechanisms common to all devices at the CAN-network.

驱动单元的目的是将轴控制器或其他运动控制产品连接到CAN总线。 它们可以接收通常用于I/O配置的服务数据对象所做的配置信息，限制扩展参数或应用程序的特定参数。 在运行时，可以通过轮询或事件驱动（中断）通过CAN总线从驱动单元获取数据。
>The purpose of drive units is to connect axle controllers or other motion control products to the CAN bus. They can receive configuration information what is done via service data objects normally for I/O configurations, limit parameters for scaling or application specific parameters. At run time, data can be obtained from the drive unit via CAN bus by either polling or event driven (interrupt).

运动控制产品具有用于实时操作的过程数据对象映射(PDO)，其可以使用服务数据对象(SDO)来配置（参见/ 3 /）。 该通信信道用于交换实时数据，如设定点或实际值，如位置实际值
>The motion control products have a process data object mapping for real time operation, which may be configured using service data objects (see /3/). This communication channel is used to interchange real-time data like set-points or actual values like a position actual value e.g.

### 	5.2. 通过分析进行标准化 
>Standardization via profiling. 
	
设备规范的配置文件方法的两个主要优点在于系统集成和设备标准化。
>The two principal advantages of the profile approach for device specification are in the areas of system integration and device standardization. 

如果两个独立设备制造商设计必须通信的产品，则必须为两个制造商提供另一个制造商的设备规范（来使两个产品兼容）。 这些规范在正式和术语方面将因公司而异。 设备配置文件的概念提供了生成此类规范的标准。 通过采用这种方法，所有制造商都将以类似的方式指定他们的设备，这大大减少了系统集成的工作量。
>If two independent device manufacturers design products that have to communicate, then both manufacturers must be provided with a device specification from the other one. These specifications will widely differ in formal and terminological aspects from one company to another. The concept of device profiling provides a standard for producing such specifications. By adopting this approach, all manufacturers will specify their devices in a similar fashion, what greatly reduces the effort involved in system integration.

设备规范的配置文件方法的另一个明显优势是，它可以用于指导制造商生产标准化设备。 标准化设备的优点很多。 最重要的是，标准化设备将系统集成商与特定供应商分离。 如果一个供应商无法满足特殊的应用需求，系统设计人员可以轻松地使用其他供应商提供的设备。 另一方面，设备制造商不再被迫为每个客户实施私有协议。
>The other obvious advantage of the profile approach for device specification is, that it can be used to guide manufacturers into producing standardized devices. The advantages of standardized devices are numerous. Perhaps most important is the idea, that a standardized device decouples a system integrator from a specific supplier. If one supplier cannot meet special application demands, a system designer can use devices from another supplier with reduced effort. On the other hand the device manufacturers are not forced any more to implement private protocols for each customer.

设备配置文件定义了“标准”设备。 此标准设备代表真正的基本功能，此设备类中的每个设备都必须支持。 这种强制性功能对于确保至少简单的非制造商特定的设备操作是必要的。 例如，标准驱动单元提供“快速停止”功能来停止驱动器。 此功能被定义为必需功能，因此可以使用相同的消息暂停支持驱动器和运动控制的CANopen设备配置文件的任何驱动器单元。
>A device profile defines a ‘standard’ device. This standard device represents really basic functionality, every device within this device class must support. This mandatory functionality is necessary to ensure, that at least simple non-manufacturer-specific operation of a device is possible. For example the standard drive unit provides a 'Quick stop' function to stop a drive. This function is defined as mandatory, such that any drive unit supporting the CANopen Device Profile for Drives and Motion Control, can be halted using the same message. 

### 	5.3. 对象字典 
>The object dictionary 
	
####		5.3.1. 索引和子索引的使用 
>Index and sub-index usage 


16位索引用于寻址对象字典中的所有条目。如果是简单变量，则直接引用该变量的值。但是，对于记录和数组，索引会寻址整个数据结构。为了允许通过网络访问数据结构的各个元素，定义了一个子索引。对于单对象字典条目，如一个无符号8位数、布尔值、32位数等，子索引的值始终为零。对于复杂的对象字典条目，例如具有多个数据字段的数组或记录，子索引引用由主索引指向的数据结构中的字段。索引计数从一开始。例如，在“因子组”一章中存在名为位置编码器分辨率的对象608Fh。因为这可能是分数，所以使用数组中的两个整数来描述它。驱动器以以下方式使用这两个值：
>A 16-bit index is used to address all entries within the object dictionary. In case of a simple variable this references the value of this variable directly. In case of records and arrays however, the index addresses the whole data structure. To allow individual elements of structures of data to be accessed via the network a sub-index has been defined. For single object dictionary entries such as anUnsigned8, Boolean, Integer32 etc. the value for the sub-index is always zero. For complex object dictionary entries such as arrays or records with multiple data fields the sub-index refers to fields within a data-structure pointed to by the main index. Index counting starts with one. For example in the chapter Factor Group exists the object 608Fh named position encoder resolution. Because this may be a fraction, two integers in an array are used to describe it. The drive uses the two values in the following manner:


position encoder resolution = encoder increments / motor revolutions

子索引概念可用于访问这些不同数据类型的字段，如下所示:
>The sub-index concept can be used to access these individual fields which may be of different datatype as shown below:


|   Index    |   Sub |     Name  |   Data type   |
| -----------|-------|-----------|---------------|
|   648Fh  | 0 |    Nmuber of elements |    UNSIGNED8   |
|          | 1 |    Encoder increments |    UNSIGNED32   |
|          | 2 |    Motor revolutions  |    UNSIGNED32   |

表1：索引和子索引用法
>Table 1:Usage of index and sub-index
