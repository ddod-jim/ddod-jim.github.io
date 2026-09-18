## Slide 1

![image.png](./ppt/media/image1.png "Google Shape;159;p25")

智驾 量产经验分享 ： 自动驾驶  技术演进与产业全景

一段热血沸腾的端到端进化史

Waymo \| Tesla \| Momenta \| 元戎 \| 理想 \| 华为 \| 地平线

## Slide 2

![image.png](./ppt/media/image1.png "Google Shape;167;p26")

萌芽期 (2004-2012)

DARPA 挑战赛启动，Waymo 开启 L4 研发， 技术方案All In 激光雷达

成长期 (2013-2018)

分层架构（感知+规控）成为主流，感知范式转为深度学习驱动

突破期 (2019-2022)

BEV 方案变成主流，感知精度进一步提升，L2++ 商业模式跑通

爆发期 (2023-Present)

DLP 开始驱动规控转为深度学习，端到端助力城市NOA成功量产

自动驾驶发展的四个纪元

## Slide 3

![image.png](./ppt/media/image2.png "Google Shape;187;p27")

![image.png](./ppt/media/image2.png "Google Shape;188;p27")

![image.png](./ppt/media/image3.png "Google Shape;189;p27")

![image.png](./ppt/media/image4.png "Google Shape;190;p27")

1.0 时代：感知 + 规则控制

传统模块化架构

将系统分为感知 (Perception)、预测 (Prediction)、决策 (Planning) 与控制 (Control) 四个独立模块。

优势： 可解释性强，便于调试与回溯。

瓶颈： 长尾场景 (Corner Cases) 难以覆盖，\"IF-ELSE\" 规则爆炸。

代表： 早期 Waymo 与 传统 Tier 1 方案。

▹

▹

▹

## Slide 4

![image.png](./ppt/media/image2.png "Google Shape;205;p28")

![image.png](./ppt/media/image2.png "Google Shape;206;p28")

1.0 时代：感知 + 规则控制

跨相机问题如何解决？

![](./ppt/media/image45.png "Google Shape;210;p28")

## Slide 5

![image.png](./ppt/media/image2.png "Google Shape;215;p29")

![image.png](./ppt/media/image3.png "Google Shape;216;p29")

![image.png](./ppt/media/image6.png "Google Shape;217;p29")

2.0 时代：BEV + T ransformer

从 2D 到 3D 的飞跃

BEV (Bird\'s Eye View) 技术将多个摄像头的 2D 图像实时转换为 3D 俯视图，解决了遮挡与空间一致性问题。

Transformer 应用： 实现特征在多摄像头间的高效融合。

去高精地图： BEV 技术是实现"轻地图"方案的关键。

核心突破： 特斯拉 2021 AI Day 确立的行业标准。

▹

▹

▹

## Slide 6

![image.png](./ppt/media/image1.png "Google Shape;232;p30")

空间一致性：  将多个摄像头画面统一投影至 3D 鸟瞰图 (BEV)，消除图像拼接断层。

时空融合：  Transformer 机制实现跨摄像头的长程注意力分配，增强遮挡目标的预测能力。

特征级融合：  通过该架构实现了从"看图像"到"感知世界"的跨越。

![image.png](./ppt/media/image7.png "Google Shape;236;p30")

![image.png](./ppt/media/image20.png "Google Shape;237;p30")

![image.png](./ppt/media/image5.png "Google Shape;238;p30")

![](./ppt/media/image43.png "Google Shape;239;p30")

2.0 时代：BEV + T ransformer

## Slide 7

![image.png](./ppt/media/image2.png "Google Shape;246;p31")

2 .0 时代： BEV + Transformer

异形障碍物问题如何解决 ？

![](./ppt/media/image9.png "Google Shape;250;p31")

## Slide 8

![image.png](./ppt/media/image2.png "Google Shape;255;p32")

3 .0 时代： Occupancy Network

![](./ppt/media/image11.png "Google Shape;258;p32")

感知真实世界的"体积"

进一步将世界体素化 (Voxelization)，不再识别

具体的"物体"，而是识别空间是否被占用。

这一技术有效解决了通用障碍物的识别难题，

如异形车、掉落的纸箱或突出的树枝，

大幅提升了极端场景下的安全性。

▹

▹

## Slide 9

![image.png](./ppt/media/image2.png "Google Shape;268;p33")

3 .0 时代 引领高速NOA的量产风暴

![](./ppt/media/image55.png "Google Shape;271;p33")

## Slide 10

![image.png](./ppt/media/image1.png "Google Shape;276;p34")

4 .0  时代   DLP + E2E 

从感知到控制的一体化

两段式 E2E： 感知输出中间特征，决策模块基于此特征学习轨迹。

一段式 E2E： 像素输入，动作输出 (Pixels to Torque)。信息无损流转。

范式转变： 从"基于规则"演进为"基于概率神经网络"，系统更具拟人性。

▹

▹

▹

![](./ppt/media/image12.png "Google Shape;286;p34")

## Slide 11

![image.png](./ppt/media/image1.png "Google Shape;291;p35")

从感知数据直接输出驾驶意图。Tesla V12 验证了"数据驱动"取代"逻辑规则"的可行性，大幅提升拟人性。

4 .0  时代   DLP + E2E  优势

▹

![](./ppt/media/image8.png "Google Shape;296;p35")

## Slide 12

![image.png](./ppt/media/image1.png "Google Shape;301;p36")

4 .0  时代 引领 城区NOA量产

![](./ppt/media/image51.png "Google Shape;304;p36")

## Slide 13

![image.png](./ppt/media/image1.png "Google Shape;309;p37")

从单车智能向数据驱动转型，自动驾驶正迎来其"iPhone 时刻"。

全覆盖

中国城市开通城市 NOA

70%

202 6  年新车 L2 级渗透率预期

1/10

E2E 架构较传统架构代码缩减量

落地现状：万亿级市场的量产节点

## Slide 14

![image.png](./ppt/media/image1.png "Google Shape;323;p38")

![image.png](./ppt/media/image10.png "Google Shape;324;p38")

![image.png](./ppt/media/image10.png "Google Shape;325;p38")

Waymo：L4 级坚守者

Tesla：量产规模先锋

多传感器冗余：  激光雷达、毫米波、视觉多重叠加，极致安全。

高精地图依赖：  侧重限定区域内的极致体验。

重资产模式：  自建车队，专注于 Robotaxi 商业化。

纯视觉 (Pure Vision)：  放弃雷达，极致压缩成本，追求全球通用。

海量数据驱动：  利用数百万辆车进行"影子模式"训练。

算法进化极快：  从模块化到端到端的引领者。

![image.png](./ppt/media/image15.png "Google Shape;334;p38")

![image.png](./ppt/media/image17.png "Google Shape;335;p38")

![image.png](./ppt/media/image19.png "Google Shape;336;p38")

![image.png](./ppt/media/image16.png "Google Shape;337;p38")

![image.png](./ppt/media/image14.png "Google Shape;338;p38")

![image.png](./ppt/media/image21.png "Google Shape;339;p38")

4.0 时代 路线之争：Waymo 的稳健与 Tesla 的激进

所有做城区的公司都有一个远景，就是去做L4的Robotaxi

## Slide 15

![image.png](./ppt/media/image1.png "Google Shape;347;p39")

![image.png](./ppt/media/image18.png "Google Shape;348;p39")

![image.png](./ppt/media/image13.png "Google Shape;349;p39")

![image.png](./ppt/media/image22.png "Google Shape;350;p39")

Momenta

智己 作为 标杆客户，从高速NOA、城区NOA、车载芯片等，帮助Momenta 完成技术积累 & 量产经验，目前量产车型 200款，量产车辆 80W辆

华为

问界 引爆 整个行业，以激光雷达作为技术主干，L2++ 时代当之无愧的王者，上下游链路集大成者（传感器、芯片、算法、软件架构）

地平线

通过"芯片+软件工具链"开放赋能， 征程系列席卷整个中国中低端市场，HSD 作为一段式端到端 代表，帮助地平线敲开高端芯片市场（J6P）

4.0 时代 中国 三大供应商

![](./ppt/media/image29.png "Google Shape;359;p39")

![](./ppt/media/image33.png "Google Shape;360;p39")

![](./ppt/media/image26.png "Google Shape;361;p39")

## Slide 16

![image.png](./ppt/media/image2.png "Google Shape;366;p40")

![image.png](./ppt/media/image23.png "Google Shape;367;p40")

![image.png](./ppt/media/image24.png "Google Shape;368;p40")

![image.png](./ppt/media/image23.png "Google Shape;369;p40")

![image.png](./ppt/media/image27.png "Google Shape;370;p40")

![image.png](./ppt/media/image28.png "Google Shape;371;p40")

![image.png](./ppt/media/image25.png "Google Shape;372;p40")

5.0 时代：VLA 与 世界模型

VLA 模型

Vision-Language-Action。让车辆不仅能看到，还能"理解"自然语言指令并执行复杂动作。

World Model

预测未来。系统能推演未来几秒内环境的变化，像人类一样具备预判能力。

具身智能

自动驾驶成为机器人技术在道路上的表现，实现真正的物理世界通用智能。

## Slide 17

![image.png](./ppt/media/image2.png "Google Shape;385;p41")

5.0 时代：VLA 

VLA 典型优势：  理解复杂场景与交警手势，优于基础信号灯判断

![](./ppt/media/image50.png "Google Shape;389;p41")

## Slide 18

![image.png](./ppt/media/image2.png "Google Shape;394;p42")

5.0 时代： 世界模型  

世界模型 典型优势：  预知未来

![](./ppt/media/image38.gif "Google Shape;398;p42")

## Slide 19

![image.png](./ppt/media/image2.png "Google Shape;403;p43")

![image.png](./ppt/media/image32.png "Google Shape;404;p43")

![image.png](./ppt/media/image31.png "Google Shape;405;p43")

∞

闭环数据迭代

量产 核心驱动力：数据飞轮

Momenta 与 特斯拉的制胜法宝

数据飞轮 (Data Flywheel) 通过大规模量产车回传的真实长尾场景数据，自动训练并优化模型，实现算法的自我进化。

数据基建： 自动化标注、超算中心 (Dojo)、云端训练引擎。

竞争壁垒： 谁拥有更多的量产车，谁就拥有更快的数据进化速度。

▹

▹

## Slide 20

数据飞轮：1%的尾端场景决定最终成败

自动驾驶竞争的本质是数据挖掘与利用的效率竞争，数据量不再是唯一标准。

![](./ppt/media/image54.png "Google Shape;423;p44")

## Slide 21

![image.png](./ppt/media/image1.png "Google Shape;428;p45")

![image.png](./ppt/media/image30.png "Google Shape;429;p45")

工具链解决的核心痛点：

1. 不同芯片底层的异构计算难题

2. 算法从实验室到车规级落地的长周期

3. 数十万长尾场景 (Corner Cases) 的挖掘与回归测试

高性能中间件：  自研操作系统 (OS)、驱动程序、传感器协议适配解 决异构算力平台的任务调度与超低延迟通信 (DDS)

成熟开发工具链：  提供从算子库到转换器的全套支持，缩短算法迁移周期 ，自动将浮点模型转化为定点，最大化硬件利用率

自动化数据闭环：  覆盖采集、清洗、自动标注 (Auto-labeling) 到模型训练的工程化体系。

![image.png](./ppt/media/image34.png "Google Shape;437;p45")

![image.png](./ppt/media/image36.png "Google Shape;438;p45")

![image.png](./ppt/media/image35.png "Google Shape;439;p45")

量产基石：中间件与标准化工具链

覆盖面全评估体系 ：  数字孪生 (Digital Twin)、场景重构、大规模影子模式，通过离线评估与在线模拟，进行千亿公里虚拟验证

![image.png](./ppt/media/image36.png "Google Shape;443;p45")

## Slide 22

![image.png](./ppt/media/image1.png "Google Shape;448;p46")

影子世界：超大规模仿真

![image.png](./ppt/media/image39.png "Google Shape;451;p46")

从虚拟到现实的跃迁

高保真渲染：  利用数字孪生技术还原真实交通流，生成数亿公里的虚拟行驶里程，覆盖极端天气与突发状况。

神经渲染 (NeRF)：  通过真实路测数据快速重建场景，实现"回放式"仿真，极大提升训练效率。

## Slide 23

![image.png](./ppt/media/image1.png "Google Shape;459;p47")

![image.png](./ppt/media/image37.png "Google Shape;460;p47")

注：地平线征程 6P 为新一代旗舰，标志着国产芯片在算力与能效比上已进入全球梯队。

量产发动机：智驾芯片性能对比 (TOPS)

## Slide 24

![image.png](./ppt/media/image1.png "Google Shape;468;p48")

6 .0  时代   迈向具身智能的自动驾驶

当自动驾驶走出汽车，它将成为机器人理解并与物理世界交互的通用基础，在技术高度趋同的未来，胜出者将属于那些拥有"数据规模、算力厚度与量产闭环"的企业。

算法架构： 感知与运动算法从汽车迁移至人形机器人；大 模型将理解物体的物理属性、重量与交互

量产能力：芯片、工具链、中间件需深度融合，实现极致效能比；数据飞轮助力模型能力更强

▹

▹

## Slide 25

![image.png](./ppt/media/image1.png "Google Shape;480;p49")

一个跨行者的深入思考

自动驾驶的工具链值得在具身智能重做一遍

自动驾驶的中间件值得在具身智能重做一遍

自动驾驶的交付体系、数据体系、模型体系值得在具身智能重做一遍

硬件收敛是迟早的问题，小脑 + 大脑同样重要，小脑决定下限问题，大脑决定上限问题；locomotion本质是一个硬件生意，硬件必将收敛，只是时间问题

拥抱开源、拥抱新技术，这是一个伟大的时代，坡长雪厚，但真正留在牌桌的一定是 以量产驱动 技术变革的公司

## Slide 26

![image.png](./ppt/media/image1.png "Google Shape;488;p50")

一点关于AGI 的粗浅认知

![](./ppt/media/image40.png "Google Shape;491;p50")

当机器掌握语言，强人工智能就会到来

12个月内，我们可能会进入AI 能写出所有代码的世界

世界模型是一个能孕育AGI的载体

## Slide 27

![image.png](./ppt/media/image1.png "Google Shape;499;p51")

Coding 的市场很大

![](./ppt/media/image44.png "Google Shape;502;p51")

## Slide 28

![image.png](./ppt/media/image1.png "Google Shape;507;p52")

很久没有见过这么激烈的厮杀了，上一轮是抖音VS快手

![](./ppt/media/image42.png "Google Shape;510;p52")

## Slide 29

![image.png](./ppt/media/image1.png "Google Shape;515;p53")

互联网中登(用户量) 看 ChatGPT

![](./ppt/media/image56.png "Google Shape;518;p53")

## Slide 30

![image.png](./ppt/media/image1.png "Google Shape;523;p54")

互联网中登( 留存 ) 看 ChatGPT

![](./ppt/media/image53.png "Google Shape;526;p54")

## Slide 31

![image.png](./ppt/media/image1.png "Google Shape;531;p55")

互联网中登( 时长 ) 看 ChatGPT

![](./ppt/media/image47.png "Google Shape;534;p55")

## Slide 32

![image.png](./ppt/media/image1.png "Google Shape;539;p56")

Anthropic 认为 收入才是硬道理

![](./ppt/media/image48.png "Google Shape;542;p56")

## Slide 33

![image.png](./ppt/media/image1.png "Google Shape;547;p57")

Anthropic 认为 收入才是硬道理

![](./ppt/media/image52.png "Google Shape;550;p57")

## Slide 34

![image.png](./ppt/media/image1.png "Google Shape;555;p58")

那就卷起来吧

![](./ppt/media/image49.png "Google Shape;558;p58")

![](./ppt/media/image41.png "Google Shape;559;p58")

## Slide 35

![image.png](./ppt/media/image1.png "Google Shape;564;p59")

模型的发布节奏

![](./ppt/media/image46.png "Google Shape;567;p59")
