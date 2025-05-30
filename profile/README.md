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

... **it's time to introduce DECISION CONTRACTS to support further development of business processes,
just like it happened in non-blockchain systems!**

## Why bother with Decision Contracts on Cosmos chains?

- Cosmos chains are using **CosmWasm**, the first-class virtual machine for executing **Smart Contracts** written in Rust.
- **CosmWasm** is secure, transparent, auditable, reliable and cost-effective (in terms of execution).
- Utilizing **CosmWasm**, Cosmos blockchains can deliver first-class solutions for business process execution using **Smart Contracts**.
- Non-trivial **Smart Contracts** are not easy to develop, test and maintain, no-matter in which programming language are developed.
- There is a natural barrier of the complexity of the business process that can be effectively implemented using only **Smart Contracts**.
- In current Cosmos technology landscape there is a niche for introducing **Decision Contracts**, that would unlock the users to build blockchain solutions that address more complex real-life needs.
- A first class virtual machine for executing **Decision Contracts** could be a game changer in technologies that support complex business logic execution on blockchains, in such industries like:
  - agricultural supply chains,
  - open data registries,
  - international money transfers,
  - central bank digital currencies,
  - electricity contract selection and switching process,
  - electricity prosumers registries and clearing,
  - logistics,
  - and many others (think of any complex business processes executed by one central authority that could be moved to blockchain).

## Smart Contracts vs Decision Contracts

### In all seriousness

| Smart Contracts                                                | Decision Contracts                                                           |
|----------------------------------------------------------------|------------------------------------------------------------------------------|
| Are about _**automating**_ and _**executing**_ business logic. | Are about _**making choices**_ based on provided _**conditions**_.           |
| Are usually stateful (if do anything meaningful).              | Are always stateless, without side-effects (idempotent).                     |
| Can be perceived as _**Business Process Executor**_.           | Can be perceived as _**Decision Provider**_ for _Business Process Executor_. |

- The **concerns** and **responsibilities** of both types of contracts are clearly **separated**.
- **They do not compete**; instead, they collaborate to achieve a common goal: the successful completion of the business process executed on blockchain, meeting real-life needs and expectations.

### In a light-hearted manner

| Smart Contracts           | Decision Contracts                                                                          |
|---------------------------|---------------------------------------------------------------------------------------------|
| Usually are not so smart. | Always make a smart decision.                                                               |
| Are not contracts.        | Anytime you ask the same question, the answer (decision) will be the same. It's a contract. |

## What about the adoption of Decision Contracts?

Does anyone develop decision logic on blockchains today?

Yes, Smart Contract developers do it every day. They implement decision logic inside the Smart Contract,
right along with business process execution logic.

Why has nobody separated **Decision Contracts** from Smart Contracts yet?

Because it makes no sense to split the code into two artifacts without introducing a new **VALUE**.
Why have the hassle of two types of contracts, when the existing one - Smart Contract - does the job?
If adopting DMN could provide a new value in the designing decision logic, why it is not adopted yet?
It can be only speculated, but after successful article and presentation of Stephen Haarmann,
many people could start thinking about "translating" DMN to Smart Contract using programming languages like Solidity.
They have fallen in a trap we did. We were thinking about compiling DMN into WebAssembly when we have learned about CosmWasm.
But this is a dead-end.

DMN provides enormous **VALUE** but is complex to implement and will not fit into any Smart Contract known today...

... **so we need a flip, similar to this one:**

|                               Traditional                               |                            Flipped                             |
|:-----------------------------------------------------------------------:|:--------------------------------------------------------------:|
|                         ![before](./before.png)                         |                     ![after](./after.png)                      |
| Practical, always ready to use,<br/>but **leaves pepper** on the table. | Practical, always ready to use,<br/>and **keeps table clean**. |

## References

- [DMN Decision Execution on the Ethereum Blockchain][1] (article from 20 June 2018)
- [DMN supporting tools][10]

[1]: https://www.researchgate.net/publication/325174084_DMN_Decision_Execution_on_the_Ethereum_Blockchain
[10]: https://dmn-tck.github.io/tck 
