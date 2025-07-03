---
layout: default
title: "Offline RL Overview"
categories: [offline-rl]
tags: [offline-rl, mopo, conservative-rl, batch-rl]
---

In offline RL, the agent learns **only from a fixed dataset**, without interacting with the environment.

Here is the objective function of MOPO:

$$
\eta^{\hat{M}}(\pi) = \mathbb{E}_{(s, a) \sim \rho^{\hat{T}}_\pi} \left[ G^{\hat{M}}_\pi(s, a) \right]
$$

Offline RL can be broadly categorized into:

- **Model-based Offline RL** (e.g. MOPO, COMBO)
- **Model-free Conservative Methods** (e.g. CQL, IQL)
