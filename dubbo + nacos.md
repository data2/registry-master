# registry-master
a compare at nacos eureka consul zk, maybe etcd

1、nacos 

阿里巴巴将通过Dubbo + Nacos以及一系列开源项目打造服务发现、服务及流量管理、服务共享平台。
https://yq.aliyun.com/articles/604028

阿里巴巴为什么不用 ZooKeeper 做服务发现？
https://yq.aliyun.com/articles/601745?spm=a2c4e.11153940.0.0.6daf38dfssnNvF

2、为什么开源 Nacos?

围绕着Service为中心的分布式基础设施正在变的越来越重要
https://cdn.yuque.com/lark/0/2018/png/15914/1530077340492-513a25c0-51d0-494f-b39d-6f615d7e3915.png

“服务治理，服务沉淀、服务共享和服务的可持续发展”是“共享服务体系”的核心价值主张
https://cdn.yuque.com/lark/0/2018/png/15914/1530077444757-d36f344d-d3ae-4df0-808f-8500b4320e8d.png

阿里巴巴将通过Dubbo + Nacos以及一系列开源项目打造服务发现、服务及流量管理、服务共享平台
https://cdn.yuque.com/lark/0/2018/png/15914/1530077476468-4ce30dd9-0da7-414a-875d-acc151739c1d.png

3、Nacos的特性？

https://cdn.yuque.com/lark/0/2018/png/15914/1530077784470-27f0e268-8d1f-443a-b1a5-3d59e15ab8f4.png

4、Nacos 与 主流开源生态的关系？

a、Nacos 不会是个封闭的体系，除了对于阿里开源生态体系如Dubbo等自身的支持，也非常强调融入其它的开源生态，这里就包括Java的微服务生态体系Spring Cloud，Kubernetes/CNCF云原生生态体系

b、Dubbo + Nacos， 专为Dubbo而生的注册中心与配置中心
https://cdn.yuque.com/lark/0/2018/png/15914/1530077613925-04d767fd-ec95-4fe2-8249-ce8650fbe372.png

c、Nacos 会完全兼容Spring Cloud

d、Nacos 支持Kubernetes DNS-based Service Discovery

服务发现的未来一定是基于标准的DNS协议做，而不是像Eureka或者像ZooKeeper这样的私有API或者协议做, 同时在云上，在服务发现场景中，注册中心更关注的是可用性而不是数据一致性，所以Nacos会首推DNS-based Servcie Discovery，并优先关注可用性，而这也正是Nacos可以无缝融合进Kubernetes服务发现体系的原因所在

e、Nacos 会填补Spring Cloud 体系与 Kubernetes 体系的鸿沟

未来会有越来越多java生态的用户会选择 Kubernetes+Spring Cloud 组合，但不幸的是，在服务发现和配置管理的解决方案上，这2个体系都采用了完全不同的方案，这给同时采用2个体系的用户在注册中心和配置中心的需求上带来了非常大的不必要的复杂性。Nacos会尝试填补2者的鸿沟，以便在2套体系下可以采用同一套服务发现和配置管理的解决方案，这将大大的简化使用和维护的成本。


