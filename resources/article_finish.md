**1. Data center cooling using model-predictive control**
该篇文章暂未找到相关信息！

**2. Cooling control based on model predictive control using temperature information of IT equipment for modular data center utilizing fresh-air**

<span style="color:blue">
摘要： *提出了一种基于模型预测控制（MPC）的模块化数据中心利用新鲜空气的冷却控制方法。该方法减少了信息技术设备和数据中心冷却设备的总能耗，同时考虑了节能与IT设备温度信息之间的关系。这种基于MPC的方法通过设备风扇控制服务器中中央处理器（CPU）的温度以进行冷却。为了设计所提出的方法，建立了一个预测模型，该模型通过设备风扇的转速，新鲜空气温度，服务器利用率以及其他因素来表示CPU温度。此外，所提出的控制方法被应用于实际的模块化数据中心。将该方法的能耗与传统方法的能耗进行比较，传统方法基于比例积分（PI）控制来控制服务器机架的入口和出口之间的温差。提供了与传统方法的实际比较实验，以验证该方法的有效性。结果表明，在实际的模块化数据中心中，与传统的控制方法相比，该方法可节能20％以上。*
</span>

==本文重点：==

<span style="color:red">本文为直接使用新鲜空气来冷却的模块化数据中心提出了一种基于模型预测控制（MPC）的冷却控制方法。所提出的方法减少了IT设备和数据中心冷却设备的总能耗，同时考虑了CPU温度管理与节能之间的关系。</span>

<span style="color:blue">总结部分：
*为了减少总功耗，我们在考虑CPU温度管理与节能之间的关系的同时，利用IT设备的温度信息，提出了一种基于MPC的模块化数据中心的冷却控制方法。由于我们的模块化数据中心直接使用新鲜空气，因此开发了一种表示CPU温度动态特性的状态空间模型，以考虑新鲜空气温度的干扰和IT设备的利用率。该模型能够预测不同条件下的动态CPU温度。结果，证实了所提出的控制方法在满足限制CPU温度的条件的同时降低了设施风扇的功耗。与传统的相比，新风温度为12°C时功耗降低了约76％，新风温度为30°C时降低了20％。因此，已经证实了实际效果。由于所提出的方法能够稳定地控制温度并促进节能操作，因此，将来我们希望将我们的方法应用于各种类型的模块化数据中心。*</span>



**3. A Holistic and Optimal Approach for Data Center Cooling Management**

摘要:*托管数据设备不断增长的IT设备的当今数据中心的高效可靠运行很大程度上依赖于冷却系统，从而以最小的环境足迹来满足IT设备的热管理需求。动态的IT工作负载以及制冷效率的空间差异会在数据中心内造成时间和空间的不均匀性。大多数数据中心都使用区域冷却执行器，例如计算机机房空调（CRAC），以减轻局部“热点”。如果没有适当的局部冷却致动机制，通常会过度提供冷却能力，从而导致能源浪费。为了解决这个问题，我们引入了自适应通风孔砖（AVT）来进行局部冷却调节，并基于质量和能量平衡原理开发一个整体的多变量模型，以捕获分区和局部冷却促动对托管IT设备的机架入口温度的影响。然后，提出了一种模型预测控制器，以在满足机架热要求的同时将总冷却功率降至最低。在这样一个统一的框架中协调区域和本地制冷驱动器，以在数据中心内供应，运输和分配制冷资源。提议的整体冷却方法已在生产数据中心得到验证。实验结果表明，与最新的控制解决方案相比，可节省多达36％的CRAC单元鼓风机功率。*

==文章重点：==
数据中心冷却从本质上讲是一个最佳控制问题，其中，在机架入口温度保持在或低于指定阈值的同时，响应动态IT工作负载，总冷却功率已降至最低。温度阈值不一定在整个数据中心内都是统一的，而是取决于IT设备所服务的不同功能，例如计算，存储和联网。IT设备中托管的IT工作负载的服务合同也会影响温度阈值。

总结部分：
本文提出了一种整体的数据中心冷却方案，以优化冷却资源的供应，运输和分配。基于开发的集成模型，设计了模型预测控制器，以协调区域冷却和局部冷却致动，从而最大程度地降低冷却功耗。通过在生产数据中心进行的实验发现，提出的方案可以将CRAC单元的鼓风机功率降低多达36％。为了扩展提出的工作，作者正在研究其在大型数据中心中的可伸缩性以及具有自组织和优化功能的分散式冷却控制框架。

**4. Failure Resistant Data Center Cooling Control Through Model-Based Thermal Zone Mapping**

摘要：
*由于巨大的冷却成本，数据中心冷却效率的改善已经积极追求多年。除了冷却效率外，冷却系统的可靠性对于保证正常运行时间也至关重要。在传统的N+1或更高冗余度的数据中心冷却系统设计中，所有机房空调(CRAC)单元要么持续在线，要么按照预定的时间表进行循环。然而，两种冷却系统的配置都有各自的缺点。当所有的通信单元都在线时，数据中心的供应通常是过剩的，而且效率很低。另一方面，虽然可以通过使用CRAC单元和关闭备份来提高制冷效率，但要保证足够的制冷供应和避免总供大于求，很难安排制冷循环。在这篇论文中，我们的目标是在保持数据中心冷却冗余的同时，达到较高的冷却效率。利用基于模型的热区映射，我们首先对数据中心进行分区，以实现所需的冷却影响冗余度。然后，我们为每个CRAC单元设计一个分布式控制器来调节其影响范围内的热状态。分布式控制器之间相互协调，以最少的冷却功率实现所需的数据中心热状态。当CRAC机组或其相关控制器发生故障时，通过预定义的热区，受影响的热区仍然在其他分散冷却控制器的控制“半径”内，因此它们的热状态由有源CRAC机组砂控制器正确管理。我们
采用这种抗失效的数据中心冷却控制方法，既提高了冷却效率，又具有鲁棒性。此外，由于分布式控制系统能够自动适应维护所需的新冷却设备配置，因此在冷却系统维护方面也具有更高的灵活性。*

**5. Using Model Predictive Control in Data Centers for Dynamic Server Provisioning**

摘要：
*数据中心日益增长的能耗已成为当今的一个重要问题。本文讨论了协调动态服务器供应和热动力学对数据中心能量控制的好处和挑战。该模型预测控制方法考虑了数据中心的计算和热特性及其相互作用，并结合动态服务器配置来优化整个数据中心的能耗。服务质量和热约束在优化过程中得到加强。仿真结果表明，所提出的控制方法对数据中心节能效果显著。*

总结：
本文介绍了区域级动力学和数据中心级动力学模型，仿真部分采用了恒功率控制、非协调控制和协调控制三种控制策略。在优化问题中考虑了动态服务器配置、服务器效率和热动力学三个方面。通过动态更改活动服务器数量、参考温度和将负载分配到不同的服务器区域，数据中心的能源效率得到了显著提高。仿真结果表明，在优化过程中协调动态服务器配置和热动力学可以降低整个数据中心的能耗。三种情况的比较提供了一个例子，在数据中心存在冷却不足的情况下，实现节能。
在仿真过程中，为了保证服务质量，MPC控制器对数据中心负荷预测的准确性至关重要。未来有必要研究基于各种负载和服务类型的动态服务器供应。控制策略的主要目标是使整个数据中心的能耗最小化。在运行数据中心时，更多的其他重要因素可以添加到成本函数中。

**6. [ACM Press the fifteenth edition of ASPLOS - Pittsburgh, Pennsylvania, USA (2010.03.13-2010.03.17)] Proceedings of the fifteenth edition of ASPLOS on Architectural support for programming languages and operating systems - ASPLOS \"10 - Joint optimization of idle and cooling power in data centers while maintaining response time**

该篇文章暂未找到相关信息！



7. Pakbaznia E , Pedram M . [ACM Press the 14th ACM/IEEE international symposium - San Fancisco, CA, USA (2009.08.19-2009.08.21)] Proceedings of the 14th ACM/IEEE international symposium on Low power electronics and design - ISLPED \"09 - Minimizing data center cooling and server power costs[C]// International Symposium on Low Power Electronics & Design. DBLP, 2009:145.
8. A review of data center cooling technology, operating conditions and the corresponding low-grade waste heat recovery opportunities
9. Viability of dynamic cooling control in a data center environment
10. From chip to cooling tower data center modeling: Part I Influence of server inlet temperature and temperature rise across cabinet
11. Reducing data center energy consumption via coordinated cooling and load management
12. Smart Chip, System and Data Center enabled by Flexible Cooling Resources
13. Optimization of data center cooling efficiency using reduced order flow modeling within a flow network modeling approach
    在流网络建模方法中，使用简化的顺序流建模优化数据中心的冷却效率
14. COORDINATING LIQUID AND FREE AIR COOLING WITH WORKLOAD ALLOCATION FOR DATA CENTER POWER MINIMIZATION
    协调液体和自由空气冷却与工作量分配，以使数据中心的功率最小化
15. Application of Heat Pipe System in Data Center Cooling
    热管系统在数据中心冷却中的应用
16. Research of Data Center Fresh Air Ventilation Cooling System
    数据中心新风通风冷却系统研究
17. Economizer Based Data Center Liquid Cooling with Advanced Metal Interfaces
    基于省煤器的数据中心液体冷却与先进的金属接口
18. Walsh E J , Breen T J , Punch J , et al. [IEEE 2010 12th IEEE Intersociety Conference on Thermal and Thermomechanical Phenomena in Electronic Systems (ITherm) - Las Vegas, NV, USA (2010.06.2-2010.06.5)] 2010 12th IEEE Intersociety Conference on Thermal and Thermomechanical Phenomena in Electronic Systems - From chip to cooling tower data center modeling: Part II Influence of chip temperature control philosophy[C]// Thermal & Thermomechanical Phenomena in Electronic Systems. IEEE, 2010:1-7.
    [IEEE 2010 12 IEEE Intersociety热与热机的现象在电子会议系统(ITherm)——拉斯维加斯,NV),美国(2010.06.2-2010.06.5)]2010年第12届IEEE Intersociety热大会和热机的现象在电子系统——从芯片到冷却塔数据中心建模:第二部分芯片温度控制哲学的影响
19. Models for Dependability and Sustainability Analysis of Data Center Cooling Architectures
    数据中心冷却体系结构的可靠性和可持续性分析模型
20. Impact of rack-level compaction on the data center cooling ensemble
    机架级压缩对数据中心冷却系统的影响
21. Green Data Center Cooling: Achieving 90% Reduction: Airside Economization and Unique Indirect Evaporative Cooling
    绿色数据中心冷却:减少90%:空气侧经济性和独特的间接蒸发冷却
22. A sustainable data center with heat-activated cooling
    一个可持续的数据中心与热激活冷却
23. Thermal Time Shifting: Decreasing Data Center Cooling Costs with Phase-Change Materials
    热时移:使用相变材料降低数据中心的冷却成本
24. Using Machine Learning for Data Center Cooling Infrastructure Efficiency Prediction
    利用机器学习进行数据中心冷却基础设施效率预测

