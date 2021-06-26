# Volume 6 Low Energy Controller

# 卷6 低功耗控制器



## 1 SCOPE

## 1 概述

Bluetooth Low Energy(LE) devices operate in the unlicensed 2.4GHz ISM(Industrial Scientific Medical) band. A frequency hopping transceiver is used to combat interference and fading.<sup>1</sup>

Which <sup>1</sup>:

1.The transceiver defined in this Part does not meet the requirements for 'frequency hopping' in some governmental regulations. See the Bluetooth Low Energy Regulatory Aspects White Paper for more information.

1、此部分定义的收发器不满足一些国家条例中“跳频”的要求。参考Bluetooth Low Energy Regulatory Aspects White Paper 以了解更多信息。

蓝牙低功耗(LE)设备工作在免许可的2.4GHz ISM频段。并使用跳频收发器对抗干扰和衰减。

Two modulation schemes are defined. The mandatory modulation scheme ("1 Msym/s modulation") uses a shaped, binary FM to minimize transceiver complexity. The symbol rate is 1 Msym/s. An optional modulation scheme ("2 Msym/s modulation") is similar but uses a symbol rate o f 2 Msym/s.

标准定义了两种调制方案。强制支持的调制方案(“1 Msym/s调制”)使用二进制整形FM以最小化收发器复杂度。其符号率为1 Msym/s。可选的调制方案(“2 Msym/s 调制”)类似，但使用2 Msym/s符号率。

The 1 Msym/s modulation supports two PHYs:

+ LE 1M, with uncoded data at 1 Mb/s;
+ LE Coded, with the Access Address, Coding Indicator, and TERM1 coded at 125 kb/s and the payload coded at either 125 kb/s or 500 kb/s.

1 Msym/s 调制支持两种PHY:

+ LE 1M,数据率1 Msym/s无编码
+ LE 编码，Access Address, Coding indicator及TERM1编码速率为125 kb/s，而负载数据编码为500 kb/s.

A device shall support the LE 1M PHY. Support for the LE Code PHY is optional.

设备必须支持LE 1M PHY，可选支持LE Coded PHY。

The 2 Msym/s modulation supports a single PHY.

2 Msym/s调制只支持一种PHY.

A Time Division Duplex(TDD) scheme is used on all PHYs. The specification defines the requirements for a Bluetooth radio for the Low Energy radio.

所有PHY上都实现了时分双工机制。本规范定义了低功耗射频对蓝牙射频的要求。

Requirements are defined for two reasons:

+ Provide compatibility between radios used in the system
+ Define the quality of the system

定义相关要求有两个原因：

+ 为系统中使用的射频提供兼容性
+ 定义系统质量

An LE radio shall have a transmitter or a receiver, or both.

LE 射频需要支持发送机或接收机，或者都支持。

The LE radio shall fulfill the stated requirements for the operation conditions declared by the equipment manufacture (see Section A.1).

LE射频必须满足所述设备厂家定义的工作条件要求。

The specification is based on the established regulations for Europe, Japan, North America, Taiwan, South Korea and China. The standard documents listed below are only for information, and are subject to change or revision at any time.

本规范基于以下国家已建规则：欧洲，日本，北美，台湾，南韩和中国。以下列出的标准文档仅做参考，并随时可能更改或修订。

The Bluetooth SIG maintains regulatory content associated with Bluetooth technology in the 2.4GHz ISM band on its web site, at  https://www.blue-tooth.com/develop-with-bluetooth/build/regulatory-knowledge-database.

蓝牙SIG在其官网上管理2.4GHz ISM频段中蓝牙技术相关的调整后的内容，网址： https://www.blue-tooth.com/develop-with-bluetooth/build/regulatory-knowledge-database。

**Europe:**

Approval Standards: European Telecommunications Standards Institute, ETSI Documents: EN 300 328, EN 300 440, EN 301 489-17

**欧洲：**

审批标准：欧洲电信标准协会，ETSI 文档：EN 300 328, EN 300 440, EN 301 489-17

**Japan:**

Approval Standards: Japanese Radio Law, JRL

Documents: Japanese Radio Law: Article 4.3, Article 28, Article 29, Article 38

Radio Equipment Regulations: Article 5, Article 6, Article 7, Article 14, Article 24, Article 9.4, Article 49.20.1.C.2, Article 49.20.1.E.3

Radio Law Enforcement Regulations: Article 6.2, Article 6.4.4.1, Article 7

**日本：**

审批标准：日本无线电法律，JRL

文档：日本无线电法律：条例4.3，条例28，条例29，条例38

无线电设备条例：条例5，条例6，条例7，条例14，条例24，条例9.4，条例49.20.1.C.2，条例49.20.1.E.3

无线电法律强制条例：条例6.2，条例6.4.4.1，条例7

**North America:**

Approval Standards: Federal Communications Commission, FCC, USA Documents: CFR47, Part 15: Section 15.205 and 15.247

Approval Standards: Industry Canada, IC, Canada

Documents: RSS_210 and RSS 139

**北美：**

审批标准：联邦通信委员会， FCC，USA

文档：CRF47，Part 15：章节15.205，15.209和15.247

许可标准：加拿大工业部，IC，加拿大

文档：RSS-210和RSS139。

**Taiwan:**

Approval Standards: National Communications Commission, NCC

Documents: Low Power 0002 (LP0002); Low-power Radio-frequency Devices Technology Regulations

**台湾：**

审批标准： 国家通信委员会，NCC

文档：低功率0002 (LP0002); 低功率射频设备技术条例。

**South Korea:**

Approval Standards: Korea Communications Commission, KCC

Documents: Rules on Radio Equipment 2008-116

**南韩：**

审批标准：韩国通信委员会，KCC

文档：无线设备2008-16中的规则

**China:**

Approval Standards: Ministry of Industry and information Technology, MIIT

Documents: MIIT regulation [2002]353

**中国：**

审批标准：工信部，MIIT

文档：MIIT条例 [2002]353

































































