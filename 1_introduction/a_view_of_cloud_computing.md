
**论文链接**：https://dl.acm.org/citation.cfm?id=1721672

### Problem definition
The dream of cloud computing has come true, but its conception is not clear. Lots of pepople
illustrate confusion and skepticism about it. The paper would identify what is cloud computing and
list some import obstacles and opportunities of cloud computing.


### Key insights/contributions
**1. make a clear definition about cloud computing and list its features and benefits**
- **conception**:
    - cloud computing include services over the Internet and the bottom hardware/system software. The IaaS and PaaS are more alike than different, and should not be distinguished
    - medium-sized or smaller data centers shouldn't be called cloud computing
    - cloud computing can be classified based on the cloud system software's level of abstraction and the level of management of the resources

- **features**:
    - there are enough(infinite) computing resources available that can be used by services to follow load surges on demand
    - the computing resources are scalable, so there is no need for an up-front commitment by cloud users
    - the billing unit is on a short-term basis

- **benefits**:
    - cost associativity can make computations faster with the same cost
    - In the long run, scale-up/down elasticity can not only reduce the cost but allow the steady-state expenditure to more closely match the steady-state workload

**2. list top 10 obstacles and opportunities for cloud computing**
- **Buisness Continuity and Service Availability**: the services hosted by the cloud computing provieders are not always availability and the data can't be guaranteed to not lose.
So the only plausible solution is select multiple cloud computing providers

- **Data Lock-in** : the storage APIs for cloud computing are still essentially proprietary, so it is hard for the user to migrate between different cloud providers. one solution would be to standardize the APIs in such a way that develper can deploy services and data across multiple cloud computing providers

- **Data Confidentiality/Auditability**: cloud users face security threats both from outside and inside the cloud. the outer threats should be solved by the provider and the user. the threats from inside can be solved by virtualization. the threat from the provider should be solved by contracts and courts. data can be stored by encryption to avoid the data escape.

- **Data transfer Bottlenectks**: data transder in the cloud is slow and expensive. For large datasets, it may be cheaper and faster to ship disks than transfer over the network

- **Performance Unpredictability**: network and disk I/O are more problematic than CPU/Memory. Possible solutions include virtualization of interrupts or I/O channels and usage of flash memory

- **Scalable Storage**: it is not clear about how to implement the scalability of storage. there are many attempts to answer the question, but still has much controversy

- **Bugs in Large Scale Distributed Systems**: bugs in the cloud computing environment may not be reproduced in smaller configurations. reliance on the virtual machine can help solve the problem

- **Scaling Quickly**: quick scalability can react to performance and correctness problems in time and conserve resources and money. A fast and easy-to-use sanpshot/restart tool can help developers to conserve more computing resources

- **Reputation Fate Sharing**: reputation-guarding services can help prevent malware. Transfer of legal liability is another issue which should be solved.

- **Software Licensing**: commercial software is expensive and its usage is limited, so they are not fit for the cloud computing. The solution may be open source to remain popular or commercial software companies change their licensing structure.


### Inputs & Outputs
- **Inputs**: None
- **Outputs**: None

### Evaluation methodology


### Weakness / flaws
1、the paper didn't give a quantitative criteria to justify whether a cluster is cloud computing
2、distinction between the cloud computing and conventional data centers(or utility computing/grid computing) is not detailed

### Opportunities for future work
1、introduce more technical architectures used by cloud computing
2、compare different cloud computing platforms

### Your problems in understanding the paper
How to quantify the loss of the cloud computing user caused by provider?