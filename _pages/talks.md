---
layout: page
permalink: /talks/
title: Invited Talks
description: 
nav: true
nav_order: 2
---


{% include bib_search.liquid %}

<div class="publications">

{% talkbib %}

</div>



<!-- >## 2024

<details>
    <summary><h2 style="display:inline-block"> Towards Agent-based Autonomous Network Security</h2> </summary> 

    Abstract:
    Security of cyber-physical network systems, such as 5G/6G communication networks, vehicular networks, and the Internet of Things, has become increasingly critical nowadays. Traditional security mechanisms rely primarily on manual operations, which can be slow, expensive, and ineffective in the face of the dynamic landscape of adversarial threats. This problem will only be exacerbated as attackers leverage artificial intelligence (AI) to automate their workflows. As a countermeasure, safeguarding critical network systems also calls for autonomous defensive operations that delegate security decisions to AI agents. This talk presents our agent-based framework for autonomous attack detection and response using reinforcement learning (RL) and large language models (LLM). To address conventional RL's reactive nature, we propose a new RL paradigm, conjectural online RL (coRL), to equip the security agent with predictive power when dealing with the agent's epistemic uncertainty over the attacker's presence and actions. The intuition of coRL is to endogenize the epistemic uncertainty as part of the RL process: the agent maintains an internal world model as a conjecture of the uncertainty, and the learned conjecture produces valid predictions consistent with environment feedback induced by epistemic uncertainty. To mitigate the RL agent's reliance on stylized modeling and textual data pre-processing, we further incorporate LLMs into the agentic framework to deliver end-to-end autonomous cyber operations. We finally conclude the talk by discussing the path ahead to building fully autonomous security agents. 

    References:
    1. K. Hammar, T. Li, R. Stadler, and Q. Zhu, "Automating security strategies through online learning with adaptive conjectures,"  IEEE Transactions on Information Forensics and Security, 2025, to appear. 

    2. T. Li, K. Hammar, R. Stadler, and Q. Zhu, "Conjectural online learning with first-order beliefs in asymmetric information stochastic games," in 63rd IEEE Conference on Decision and Control (CDC 2024), Milan, Italy, Dec. 2024.
</details> 

*IEEE COMSOC TCCN Rising Star Symposium Series, Stevens Institute of Technology, NJ, Nov. 21.*   



<details>
    <summary><h2 style="display:inline-block"> Online Optimization Meets Urban Transportation </h2> </summary> 

    Abstract:
    Urban transportation networks are inherently complex and dynamic, characterized by intricate road connections and diverse network structures coupled with time-variant traffic demands and frequent traffic incidents. Hence, offline planning or designing alone cannot guarantee real-time operational control and management of urban transportation systems, which may fail when physical attacks, unforeseen conditions, or unanticipated use places the system outside the design envelope. A desired real-time operation mechanism must adapt to the dynamic environment and determine management decisions to be executed while a system is running; i.e., input data arising over time have to be processed, and decisions have to be made before all input data are known. Such a decision-making process falls within the realm of online optimization or online learning. 

    Motivated by several intelligent transportation applications from our past research projects, this tutorial aims to provide a gentle introduction to online optimization methods with much emphasis on the intuitive insights and relevance to transportation applications. The tutorial starts with gradient descent algorithms in conventional convex optimization and then moves to online gradient descent in online optimization problems. Extending from the single-agent online optimization, we briefly touch upon multi-agent online learning and associated equilibrium convergence. We conclude the tutorial by discussing the openings and challenges when deploying online optimization in urban transportation systems. 

    References:
    1. T. Li, Z. Bian, H. Lei, F. Zuo, Y-T. Yang, Q. Zhu, Z. Li, Z. Chen, and K. Ozbay, ``Digital twin-based driver risk-aware intelligent mobility analytics for urban transportation management,'' IEEE Transactions on  Intelligent Transportation Systems, 2024, to appear.

    2. T. Li, Z. Bian, H. Lei, F. Zuo, Y-T. Yang, Q. Zhu, Z. Li, and K. Ozbay, “Multi-level traffic-responsive tilt camera surveillance through predictive correlated online learning,”  Transportation Research Part C: Emerging Technologies, vol. 167, 2024.


</details>    

*NYU C2SMARTER, Tier 1 University Transportation Center, NY, Nov. 8.*


<details> 
    <summary><h2 style="display: inline-block"> Conjectural Online Learning in Asymmetric Information Stochastic Games </h2></summary>

    Astract: 
    Modern socio-technical network systems powered by artificial intelligence (AI) technologies feature sophisticated interactions among humans, AI agents, and system entities. Asymmetric information stochastic games (AISG) provide principled mathematical modeling for such interactions, leading to game-theoretical mechanisms for network management. However, existing computational and learning methods in asymmetric information stochastic games (AISG) are primarily offline without adaptability to online nonstationarity, which falls short of proactive intelligence for resilient network management. To address these limitations, we propose conjectural online learning (COL), an online learning framework for generic AISGs. COL uses a forecaster-actor-critic (FAC) architecture, where the forecaster conjectures the other agents' strategies and system dynamics within a look-ahead horizon, representing the agent's subjective (mis)perception of the AISG. Based on these subjective perceptions, COL employs online rollout (actor-critic) to improve the policy. Bayesian learning is then used to calibrate the conjectures using information feedback. We establish that the conjectures produced by COL are asymptotically consistent with the information feedback in the sense of a relaxed Bayesian consistency. We deploy COL in a nonstationary IT infrastructure digital twin, which delivers online adaptable defense against advanced persistent threats compared with benchmark reinforcement learning techniques. 

    References:
    1. K. Hammar, T. Li, R. Stadler, and Q. Zhu, "Automating security strategies through online learning with adaptive conjectures,"  IEEE Transactions on Information Forensics and Security, 2024, to appear. 

    2. T. Li, K. Hammar, R. Stadler, and Q. Zhu, "Conjectural online learning with first-order beliefs in asymmetric information stochastic games," in 63rd IEEE Conference on Decision and Control (CDC 2024), Milan, Italy, Dec. 2024.

    3. T. Li, J. Guevara, X. Xie, and Q. Zhu, "Self-confirming transformer for locally consistent online adaptation in multi-agent reinforcement learning," arXiv preprint, 2023, arXiv: 2310.04579.
    

</details>

*Systems Engineering Department Seminar, City University of Hongkong, HK, Oct. 7.*

## Agent of Agents: Meta LLM-Agent for Autonomous Security Operations
*NSF Workshop on Large Language Models for Network Security, NY, Oct. 2.*

## Conjectural Online Learning with First-order Beliefs in Stochastic Games
*Coordinated Science Laboratory, University of Illinois Urbana-Champaign, IL, Aug. 13*



<details>
    <summary><h2 style="display: inline-block"> Automated Security Response Through Conjectural Online Learning under Information Asymmetry </h2></summary>

    Abstract:
    Stochastic games arise in many complex socio-technical systems, particularly in security contexts, where the defender and the attacker interact under asymmetric information feedback. Existing computational
    methods for asymmetric information stochastic games (AISGs) are primarily offline and can not adapt to equilibrium deviations. The resulting defense strategies are inadequate when facing online nonstationary attacks. To address these limitations, we propose conjectural online learning (COL), an online learning algorithm for generic AISGs. COL uses a forecaster-actor-critic (FAC) architecture, where subjective forecasts are used to conjecture the opponents' strategies within a lookahead horizon, and Bayesian learning is used to calibrate the conjectures. To adapt strategies to nonstationary environments, COL relies on online rollout with cost function approximation (actor-critic). We prove that the conjectures produced by COL are asymptotically consistent with the information feedback in the sense of a relaxed Bayesian consistency. We also prove that the empirical strategy profile induced by COL converges to the Berk-Nash equilibrium, a recently popularized solution concept in misspecified learning. We evaluate our method in a simulated IT infrastructure through an advanced persistent threat use case. COL produces effective security strategies adapting to a changing environment and enjoys faster convergence than current reinforcement learning techniques.

    References:
    1. K. Hammar, T. Li, R. Stadler, and Q. Zhu, "Automating security strategies through online learning with adaptive conjectures,"  IEEE Transactions on Information Forensics and Security, 2024, to appear. 

    2. T. Li, K. Hammar, R. Stadler, and Q. Zhu, "Conjectural online learning with first-order beliefs in asymmetric information stochastic games," in 63rd IEEE Conference on Decision and Control (CDC 2024), Milan, Italy, Dec. 2024.

</details>

*Autonomous Robotics and Control Lab, California Institute of Technology, CA, Jun. 21*

## Multi-level Traffic-responsive Tilt Camera Surveillance through Predictive Correlated Online Learning
*NYU Urban Research Day, NY, Mar. 6*

> ## Before 2024


### On the Role of Information Structures in Multi-agent Learning
*Invited Session, International Conference on Game Theory, Stony Brook, NY, Jul. 21, 2022.*

### Informationally Mosaic Reinforcement Learning
*Special Session on Markov Descision Processes, SIAM 2022 Annual Meeting, Pittsburgh, PA, Jul. 12, 2022.*

### Multi-Agent Correlated Learning over Networks
*INFORMS Annual Meeting, Workshop on Multi-agent Learning, Online, Nov. 16, 2020.*

### Directional Framelets and its Application in Medical Imaging
*PIMS-AMI Workshop on Applied Harmonic Analysis, University of Alberta, Canada, Aug. 2017.* -->