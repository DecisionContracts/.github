# Decision Contracts

**Smarter contracts make decisions**

---

## Why bother with Decision Contracts on blockchains?

### Introduction

As an introduction, we would like to cite an excerpt from Stephan Haarmann's [article][1]:

> _"Recently blockchain technology has been introduced to **execute interacting business
> processes** in a secure and transparent way. While the foundations for process
> enactment on blockchain have been researched, the execution of decisions on
> blockchain has not been addressed yet. In this paper we argue that **decisions are an
> essential aspect of interacting business processes**, and, therefore, also need to be
> executed on blockchain. The **immutable** representation of decision logic can be used by
> the interacting processes, so that decision taking will be more **secure**, more
> *transparent**, and better **auditable**."_

### Key takeaways

- Business processes are already executed on blockchains as **Smart Contracts**.
- Non-trivial **business processes** need non-trivial **decisions** during their execution.
- Decisions are **essential** for interacting business processes.
- Decision logic must be **immutable** to be **secure**, **transparent** and **auditable**.
- Decisions should be separated from the business process logic as **Decision Contracts**. 

### Milestones in the history of blockchain, BPMN and DMN

| Year | Non-blockchain | Blockchain | Comments                                                                                                                                                              |
|:----:|:--------------:|:----------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2007 |    BPMN 1.0    |            | Early adoption in the industry, every company wanted to have automated business processes.                                                                            | 
| 2008 |                |  Bitcoin   | No business process support.                                                                                                                                          | 
| 2010 |    BPMN 2.0    |            | Automating business processes is already widely adopted.                                                                                                              | 
| 2014 |                |  Ethereum  | Business processes can be supported by **Smart Contracts**.                                                                                                           | 
| 2014 |                | Tendermint | Jae Kwon invents Tendermint.                                                                                                                                          | 
| 2015 |    DMN 1.0     |            | Early adoption in the industry. Effect of real life experience using BPMN.                                                                                            | 
| 2016 |                |   Cosmos   | Cosmos Whitepaper published.                                                                                                                                          | 
| 2018 |    DMN 1.1     |  Ethereum  | Stephan Haarmann writes his [article][1] about executing DMN models on Ethereum.                                                                                      | 
| 2024 |    DMN 1.5     |  **???**   | DMN is widely adopted in the industry [10], tools created by Trisotech, Oracle, RedHat, Camunda, Engos Software and others.</br>**STILL NO ADOPTION IN BLOCKCHAINS**. | 

## Where is the analogy?

Before 2007, transaction systems were implementing business processes, although there
was no precise specification. There was a need for such specification to be able to discover,
design, deploy, test, govern and optimize business processes in standarized way in different industries.

The same happened on Ethereum. There was simply a need for executing business
processes. And although there is no BPM execution engine run on blockchain,
**Smart Contracts** written by hand do the job. So all blockchains have adopted a concept
of Smart Contracts to be able to run business processes. 

After almost a decade of developing business processes using BPMN, the industry have
discovered a need of introducing DMN to tackle with continuously increasing complexity of
those processes and decision logic needed to meet real-life expectations.

Ethereum is almost a decade in use, and hundreds of other blockchains run business processes
using Smart Contracts...

> ... it's time to introduce **Decision Contracts** to support their further development
> just like it happened in non-blockchain systems!

## References

- [DMN Decision Execution on the Ethereum Blockchain][1] (article from 20 June 2018)
- [DMN supporting tools][10]

[1]: https://www.researchgate.net/publication/325174084_DMN_Decision_Execution_on_the_Ethereum_Blockchain
[10]: https://dmn-tck.github.io/tck 
