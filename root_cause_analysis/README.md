# Root cause analysis in distributed system

## Trace

- [22_Fudan_Enjoy your observability: an industrial survey of microservice tracing and analysis](https://link.springer.com/article/10.1007/s10664-021-10063-9)

This paper presents a industrial survey on microservice tracing and analysis through interviewing developers and operation engineers of microservice systems from ten companies.

![Research Procedure of Interview](./figures/industrial_trace.jpg)

## Log
- [21_ISSTA_Faster, Deeper, Easier: Crowdsourcing Diagnosis of Microservice Kernel Failure from User Space](https://dl.acm.org/doi/abs/10.1145/3460319.3464805)

[[code]](https://github.com/PanYicheng/dycause_rca)

In this paper, log is first transformed into metric by `linear interpolation`. Then `SPOT` algorithm is used to do anomaly detection. A new causal inference method combining two methods, `Granger causality test`  and `Granger causal intervals`, is proposed in the anomaly interval to construct anomaly propagation links, and then a service dependency graph is constructed by fusing multiple links. Finally, a `backward breadth-first algorithm `is done on the service dependency graph for root cause localization.

![Dycause](./figures/dycause.jpg)