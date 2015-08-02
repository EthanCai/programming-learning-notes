# Operating Systems

Mach [Intro: http://www-2.cs.cmu.edu/afs/cs/project/mach/public/www/mach.html,Paper: http://www-2.cs.cmu.edu/afs/cs/project/mach/public/www/doc/publications.html]

传统的kernel实现中，对中断的响应是在一个“大函数”里实现的。称为大函数的原因是从中断的入口到出口都是同一个控制流，当有中断重入发生的时候，实现逻辑将变得非常复杂。大多数的OS，如UNIX，都采用这种monolithic kernel architecture。

1985年开始的Mach项目，提出了一种全新的microkernel结构，使得由于70年代UNIX的发展到了极致而觉得后续无枝可依的学术界顿时找到了兴奋点，也开始了沸沸扬扬的monokernel与microkernel的争论。

插播一个花絮：Mach的主导者Richard Rashid，彼时是CMU的教授，受BillGates之托去游说JimGray加盟MS。结果把自己也被绕了进来，组建了Microsoft Research。他到中国来做过几次21Century Computing的keynotes。

Exokernel [Intro:http://pdos.csail.mit.edu/exo/，Paper:http://pdos.csail.mit.edu/PDOS-papers.html#Exokernels]

虽然microkernel的结构很好，但实际中并没有广泛应用，因为performance太差，而且大家逐渐发现OS的问题并不在于实现的复杂性，而更多在于如何提高application使用资源的灵活性。这也就是在kernel extension（例如loadable module in Linux）出现后，有关OS kernel architecture的争论就慢慢淡出人们视线的原因。

Exokernel正是在这样的背景中出现的，它并不提供传统OS的abstraction（process,virtual memory等），而是专注于资源隔离与复用（resource isolation and multiplexing），由MIT提出。在exokernel之上，提供了一套库，著名的libOS，用于实现各种OS的interface。这样的结构为application提供了最大的灵活度，使不同的application可以或专注于调度公平性或响应实时性，或专注于提高资源使用效率以优化性能。以今天的眼光来看，exokernel更像是一个virtual machine monitor。

Singularity [Intro:http://research.microsoft.com/os/Singularity/,Paper: http://www.
research.microsoft.com/os/singularity/publications/HotOS2005_BroadNewResearch.pdf]

Singularity出现在virus，spyware取之不尽、杀之不绝的21世纪初期，由Microsoft Research提出。学术界和工业界都在讨论如何提供一个trust-worthy computing环境，如何使计算机系统更具有manage-ability。Singularity认为要解决这些问题，底层系统必须提供hardisolation，而以前人们都依赖的硬件virtual memory机制并无法提供高灵活性和良好性能。在.Net和Java等runtime出现之后，一个软件级的解决方案成为可能。

Singularity在microkernel的基础上，通过.Net构建了一套type-safed assembly作为ABI，同时规定了数据交换的message passing机制，从根本上防止了修改隔离数据的可能。再加上对application的安全性检查，从而提供一个可控、可管理的操作系统。由于.NetCLR的持续优化以及硬件的发展，加了这些检查后的Singularity在性能上的损失相对于它提供的这些良好特性，仍是可以接受的。

这种设计目前还处于实验室阶段，是否能最终胜出，还需要有当年UNIX的机遇。

# Virtual Machines

VMWare ["MemoryResource Management in VMware ESX Server"，OSDI’02,Best paper award]
耳熟能详的vmware，无需多说。

XEN [“Xen and the Art of Virtualization”, OSDI’04]
性能极好的VMM，来自Cambridge。

Denali [“Scaleand Performance in the Denali Isolation Kernel”, OSDI’02, UW]
为internetservices而设计的application level virtual machine，在普通机器上可运行数千个VMs。其VMM基于isolation kernel，提供隔离，但并不要求资源分配绝对公平，以此减少性能消耗。

Entropia [“The Entropia VirtualMachine for Desktop Grids”, VEE’05]
要统一利用公司内桌面机器资源来进行计算，需要对计算任务进行良好的包装，以保证不影响机器正常使用并与用户数据隔离。Entropia就提供了这样的一个计算环境，基于windows实现了一个application level virtual machine。其基本做法就是对计算任务所调用的syscall进行重定向以保证隔离。类似的工作还有FVM：“AFeather-weight Virtual Machine for Windows Applications”。

# Design Revisited

“Are Virtual Machine Monitors Microkernels Done Right?”，HotOS’05

这个题目乍听起来，十分费解，其意思是VMMs其实就是Microkernel的正确实现方法。里面详细讨论了VMM和Microkernel，是了解这两个概念的极好参考。

“Thirty Years Is Long Enough: Getting Beyond C”, HotOS’05

C可能是这个世界上最成功的编程语言，但其缺点也十分明显。比如不支持thread，在今天高度并行的硬件结构中显得有点力不从心，而这方面则是functional programming language的长处，如何结合二者的优点，是一个很promising的领域。

# Programming Model

“Why Threads Are a Bad Idea”

单使用thread结构的server是很难真正做到高性能的，原因在于内存使用、切换开销、同步开销和保证锁正确性带来的编程复杂度等。

“SEDA: An Architecture for Well-Conditioned, Scalable Internet Services”，OSDI’01

Thread不好，但event也没法解决所有问题，于是我们寻找一个结合的方法。SEDA将应用拆分为多个stage，不同stage通过queue相连接，同一个stage内可以启动多个thread来执行queue中的event，并且可通过反馈来自动调整thread数量。

## Software Transactional Memory

如果内存可以提供transaction语义，那么我们面对的世界将完全两样，language, compiler, OS, runtime都将发生根本变化。虽然intel现在正在做hardware transactional memory，但估计可预见的将来不会商用，所以人们转而寻求软件解决方案。可想而知，这个方案无法base在native assembly上，目前有C#,haskell等语言的实现版本。资料比较多，参见Wikipedia。

# Distributed Algorithms

**Logical clock**, [“Time,clocks, and the ordering of events in a distributed system”, Leslie Lamport, 1978]

这是一篇关于Logic clock, time stamp, distributed synchronization的经典paper。

**Byzantine** [“The ByzantineGenerals Problem”, Leslie Lamport, 1982]

分布式系统中的错误各种各样，有出错就能停机的，有出错了拖后腿的，更严重的是出错了会做出恶意行为的。最后的这种malicious behavior，就好像出征将军的叛变，将会对系统造成严重影响。对于这类问题，Lamport提出了Byzantine failure model，对于一个由3f+1个replica组成的statemachine，只要叛变的replica数量小于等于f，整个state machine还能正常工作。

**Paxos** [“The part-time parliament”, Leslie Lamport, 1998]

如何在一个异步的分布式环境中达成consensus，这是分布式算法研究的最根本问题。Paxos是这类算法的顶峰。不过这篇paper太难了，据说全世界就3.5人能看懂，所以Lamport后来又写了一篇普及版paper：“Paxos Made Simple” ，不过还是很难懂。另外，也可参看Butler Lampson写的“The ABCD’s of Paxos”（PODC’01），其中关于replicated state machine的描述会严重启发你对并行世界本质的认识，图灵奖的实力可不是盖的。

这上面反复出现了一个名字：Leslie Lamport，他在distributed computing这个领域挖坑不辍，终成一代宗师。关于他，也有几则轶事。记得以前他在MSR的主页是这么写的，“当我在研究logicalclock的时候，BillGates还穿着开裆裤(in diaper)…”（大意如此，原文现在找不到了）。另外，他在写paper的时候，很喜欢把其他牛人的名字变换一下编排进去。这可能也是他还没拿到图灵奖的原因。[注1]

关于Lamport的其他成就，还可以参见这篇向他60岁生日献礼的paper：“Lamport on mutual exclusion: 27 years of planting seeds”, PODC’01。

# Overlay Networking, and P2P DHT

RON [“Resilient Overlay Networks”, SOSP’01]

RON描述了如何在应用层搭建一个overlay，以提供秒级广域网网络层故障恢复速度，而现有的通过路由协议来恢复通信的时间至少在几十分钟。这种快速恢复特性和灵活性使得overlay networking现在被广泛应用。

## Application Level Multicast

“End System Multicast”, SigMetrics’00

“Scalable Application Layer Multicast”, SigComm’02

关于ALM的paper很多，基本上都是描述如何搭建一个mesh network用以鲁棒的传输控制信息，另外再搭建一个multicast tree用以高效传输数据，然后再根据多媒体数据的特点做一些layered delivery。前几年出现的coolstream, pplive等系统都是这类系统的商业化产品。

## P2P

P2P的出现改变了网络。按照各种P2P网络的结构，可以分为三种。
1. Napster式，集中式目录服务，数据传输Peer to peer。
2. Gnutella式，通过在邻居间gossip来查询，也被称为unstructured P2P。
3. DHT，与unstructured P2P不同的是，DHT进行的查询有保证，如果数据存在，可在一定的hop数内返回。这个hop数通常为logN，N为系统节点数。

典型的DHT有CAN, Chord,Pastry, Tapestry等四种。这些研究主要在算法层面，系统方面的工作主要是在其上建立广域网存储系统。还有一些人在机制层面进行研究，例如如何激励用户共享、防止作弊等。

# Distributed Systems

GFS/MapReduce/BigTable/Chubby/Sawzall
Google的系列paper，大家比较熟悉，不再多说。在此可查。

## Storage

Distributed storage system的paper太多了。下面列出几篇最相关的。

“Chain Replication for Supporting High Throughput and Availability”, OSDI’04。

“Dynamo: Amazon’s Highly Available Key-value Store”，SOSP’07。

“BitVault: a Highly Reliable Distributed Data Retention Platform”, SIGOPS OSR’07。

“PacificA: Replication inLog-Based Distributed Storage Systems”, MSR-TR。

## Distributed Simulation

“Simulating Large-Scale P2P Systems with the WiDS Toolkit”, MASCOTS’05。Distributed simulation有意思的地方是simulated protocol是distributed的，而这个simulation engine本身也是distributed的。Logical和physical的time和event交杂在系统中，需要仔细处理。

# Controversial Computing Models

现在的软件系统已经复杂到了人已经无法掌握的程度，很多系统在发布时都仍然带着许多确定性(deterministic)或非确定性(non-deterministic)的bugs，只能不断的patch。既然作为人类，不够精细的特性决定了我们无法把系统的bug fix干净，我们只能从其他角度入手研究一种让系统在这令人沮丧的环境中仍能工作的方法。这就像一个分布式系统，故障无法避免，我们选择让系统作为整体来提供高可靠性。

以下3个便是典型代表。基本上，主要研究内容都集中于1) 如何正确保存状态；2)如何捕捉错误并恢复状态；3)在进行单元级恢复时，如何做到不影响整体。

Recovery Oriented Computing

Failure oblivious computing, OSDI’04

Treating Bugs as Allergies, SOSP’05

# Debugging

系统很复杂，人类无法从逻辑上直接分析，只能通过data mining的方法在宏观上进行观察。
Black box debugging[“Performance debugging for distributed systems of black boxes”, SOSP’03]
对大型系统的performance debugging非常困难，因为里面的问题很多都是非确定性的，而且无法重现。只能通过对log的挖掘，找出配对的调用/消息以定位问题。

CP-miner [“A Tool for Finding Copy-paste and Related Bugs in Operating System Code”, OSDI’04]
很多人在重用代码的时候，都使用copy-paste。但有时候简单的CP会带来严重的问题，例如局部变量的重名等。CP-miner通过分析代码，建立语法树结构，然后mine出这类错误。

# Software Architecture

- Architecture, Design, Implementation
- Orleans: Distributed Virtual Actors for Programmability and Scalability

# Big Data

- [Twitter Heron: Stream Processing at Scale](http://dl.acm.org/citation.cfm?id=2742788)
- Bigtable: A Distributed Storage System for Structured Data
- The Google File System
- MapReduce: Simplified Data Processing on Large Clusters

# Image Process

- [Image Deblurring using Inertial Measurement Sensors](http://research.microsoft.com/en-us/um/redmond/groups/ivm/imudeblurring/)