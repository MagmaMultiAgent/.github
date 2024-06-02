<p align="center">
    <img width="100%"  src="logo.png"/>
</p>

# MagMA - Scalable Distributed Reinforcement Learning in Multi-Agent Environments

This repository contains a thesis research exploring **Scalable Multi-Agent RL Solutions**, along with a partial submission and template for the Lux AI S2 competition.

Novel reinforcement learning algorithms often face scalability and compatibility issues in multi-agent environments, as they are primarily benchmarked and optimized for single-agent settings. The lack of a standardized method for adapting these algorithms to multi-agent contexts restricts their broader applicability. In multi-agent environments where the number of controllable entities can rapidly change over a short timeframe and can scale up to massive numbers, making the utilization of both monolithic and distributed architectures challenging to orchestrate. This complexity arises from the difficulty of credit assignment, extensive memory usage, and increased computational time, leading to slow, destabilized training and suboptimal resource utilization. In our work, we explore various methods to help alleviate such inefficiencies. We worked in a massively dynamic multi-agent, open-source environment featured in a Kaggle competition called Lux AI. For this setting, we study a novel implementation of a monolithic agent control method from the literature and demonstrate that a single-brain global outlook is insufficient for managing populous environments. We propose a `hybrid architecture`, combining the strengths of monolithic and distributed approaches, which led to a `30-times reduction in model size` compared to the best-performing reinforcement learning submission to the competition while still being able to learn basic skills needed in the environment `24 times faster in terms of training time` and with `600-times fewer examples of training data`. We also introduce a technique called trajectory separation to massively speed up convergence, yielding a `3-times speed increase in training speed` over our initial trials. Using our approach, we achieved a `5-times reduction in training epochs` needed to reach our designated milestone compared to the baseline model provided by the competition organizers while producing comparable results with `2-times less trainable parameters`.

Our project contains two repositories:

- **MagMA**: Contains the core code and implementation
- **MagMA-Viz**: Web-based visualization tool for training agents
- **MagMA-Viz-Client**: Client for the visualization tool

# Core Contributors

We would like to extend our heartfelt gratitude to [Gulyás László](https://github.com/lesIII) for their invaluable guidance and insightful mentorship throughout the course of this project.

We are also thankful to **Eötvös Loránd University** for providing the necessary resources and environment that facilitated the development of this project.
