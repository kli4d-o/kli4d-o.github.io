---
title: "Enabling Massive Amounts of AI Agents"
use_math: true
excerpt: "
![status: ongoing](https://img.shields.io/badge/status-ongoing-blue.svg)
![target: 02/2026](https://img.shields.io/badge/target-06/2026-yellow.svg)<br/>
A project to improve compute resource utilisation by agents while enabling development of massive amounts of agents.
"
collection: portfolio
---

![status: ongoing](https://img.shields.io/badge/status-ongoing-blue.svg)
![target: 02/2026](https://img.shields.io/badge/target-06/2026-yellow.svg)

Most agent frameworks are usually built around a specific abstraction (LangChain uses chains, LangGraph uses graphs, etc). Most of these abstractions exist to enable creation of workflows, where data flows from one agent to another along sequential pre-defined paths. These abstractions influence the flexibility of the interaction that agents can have within a multi-agent architecture, and thus the complexity of developing multi-agent systems using these frameworks.

Before the rise of LLMs, agent frameworks such as [SPADE](https://spadeagents.eu/) existed, and they still persist to date. Most of these classical agent frameworks use [agent-oriented programming](https://en.wikipedia.org/wiki/Agent-oriented_programming) principles, as opposed to using workflow-based abstractions such as graphs. In this paradigm, a discovery service builds a directory of agents within an environment. An agent can then read the directory to obtain a recipient agent's id. The sending agent uses the recipient agent's id to send it a message directly. An agent can also broadcast a message to a topic for agents that have subscribed to the topic to read. Agents can even be assigned roles, such that only agents with a certain role are allowed to subscribe to specific topics. This way, recipients of broadcasted messages can be confined to agents having specific roles. Due to this heavy reliance on message passing, standards such as [FIPA](http://ieeexplore.ieee.org/document/773093/) [1] have been developed to enable standardised agent communication, even between agents deveoped using different frameworks.

In spite of all these advances, improvements can still be made to enable massive amounts of agents. Several frameworks exist that enable agent interaction in a distributed computing setup, and therefore the aim of this project is not to enable distributed multi-agent systems. Rather, this project aims to improve the efficiency of agents within a single computing node. The end goal is to have a single computing node that is able to run a far much higher number of agents concurrently while efficiently utilising the computing node's resources (working memory and processor clock cycles). The resultant framework arising from this project will also support swarm agents natively, disentangle itself from the limitation of sequential data flow observed in workflow-based frameworks, and will not rely on an agent discovery service or direct message passing from one agent to another as seen in many frameworks using the agent-oriented programming paradigm.

---

[1] H. Suguri, "A standardization effort for agent technologies: The Foundation for Intelligent Physical Agents and its activities," Proceedings of the 32nd Annual Hawaii International Conference on Systems Sciences. 1999. HICSS-32. Abstracts and CD-ROM of Full Papers, Maui, HI, USA, 1999, pp. 10 pp.-, doi: 10.1109/HICSS.1999.773093.
