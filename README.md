# AI-Paper-Reading
Papers on AI

## 强化学习 & RL
[Practical_RL](https://github.com/yandexdataschool/Practical_RL/blob/master/week10_planning/seminar_MCTS.ipynb)
[Berkeley Policy Gradients](https://rail.eecs.berkeley.edu/deeprlcourse/static/slides/lec-5.pdf)
[Berkeley Actor-Critic Algorithms](https://rail.eecs.berkeley.edu/deeprlcourse/static/slides/lec-6.pdf)
(资料比较丰富，大量公式，额外启发）
[CS285](https://rail.eecs.berkeley.edu/deeprlcourse/)
[Optimal Control and Planning](https://rail.eecs.berkeley.edu/deeprlcourse/deeprlcourse/static/slides/lec-10.pdf)
[Deep RL Bootcamp](https://sites.google.com/view/deep-rl-bootcamp/lectures)

```
Core Lecture 1 Intro to MDPs and Exact Solution Methods -- Pieter Abbeel  (video | slides)
Core Lecture 2 Sample-based Approximations and Fitted Learning -- Rocky Duan  (video | slides)
Core Lecture 3 DQN + Variants -- Vlad Mnih  (video | slides)
Core Lecture 4a Policy Gradients and Actor Critic -- Pieter Abbeel (video | slides)
Core Lecture 4b Pong from Pixels -- Andrej Karpathy  (video | slides)
Core Lecture 5 Natural Policy Gradients, TRPO, and PPO -- John Schulman (video | slides)
Core Lecture 6 Nuts and Bolts of Deep RL Experimentation  -- John Schulman  (video | slides)
Core Lecture 7 SVG, DDPG, and Stochastic Computation Graphs -- John Schulman  (video | slides)
Core Lecture 8 Derivative-free Methods -- Peter Chen (video | slides)
Core Lecture 9 Model-based RL -- Chelsea Finn (video | slides)
Core Lecture 10a Utilities  -- Pieter Abbeel (video | slides)
Core Lecture 10b Inverse RL -- Chelsea Finn (video | slides)
Frontiers Lecture I: Recent Advances, Frontiers and Future of Deep RL -- Vlad Mnih (video | slides)
Frontiers Lecture II: Recent Advances, Frontiers and Future of Deep RL -- Sergey Levine (video | slides)
TAs Research Overviews (video | slides)
```

### 奖励函数 Reward-Shaping
https://zhuanlan.zhihu.com/p/139911579
http://luthuli.cs.uiuc.edu/~daf/courses/games/AIpapers/ng99policy.pdf

### GAE
[HIGH-DIMENSIONAL CONTINUOUS CONTROL USING GENERALIZED ADVANTAGE ESTIMATION](https://arxiv.org/pdf/1506.02438)
[Generalized Advantage Estimator](https://github.com/yandexdataschool/Practical_RL/blob/master/week09_policy_II/ppo.ipynb)
[Generalized Advantage Estimator知乎](https://zhuanlan.zhihu.com/p/139097326)

### Variance
[Variance Reduction in Policy gradient methods](https://www.reddit.com/r/reinforcementlearning/comments/kimtbn/variance_reduction_in_policy_gradient_methods/?utm_source=share&utm_medium=ios_app&utm_name=iossmf)
[Beyond variance reduction: Understanding the true impact of baselines on policy optimization](https://arxiv.org/abs/2008.13773)

### PPO
[RL — Proximal Policy Optimization (PPO) Explained](https://jonathan-hui.medium.com/rl-proximal-policy-optimization-ppo-explained-77f014ec3f12)
[Part 1 of 3 — Proximal Policy Optimization Implementation: 11 Core Implementation Details](https://www.youtube.com/watch?v=MEt6rrxH8W4)

A quote from the PPO paper:

```
Q-learning (with function approximation) fails on many simple problems and is poorly understood, vanilla policy gradient methods have poor data efficiency and robustness; and trust region policy optimization (TRPO) is relatively complicated, and is not compatible with architectures that include noise (such as dropout) or parameter sharing (between the policy and value function, or with auxiliary tasks).
```
PPO adds a soft constraint that can be optimized by a first-order optimizer. We may make some bad decisions once a while but it strikes a good balance on the speed of the optimization. Experimental results prove that this kind of balance achieves the best performance with the most simplicity.


## Agent

### Relexion
[Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/pdf/2303.11366)
[Reflexion](https://github.com/noahshinn/reflexion)
[Reflecting on Reflexion](https://nanothoughts.substack.com/p/reflecting-on-reflexion)

[A hard gym for programming](https://github.com/GammaTauAI/leetcode-hard-gym)
[ReAct](https://arxiv.org/pdf/2210.03629)

[Decoupling Reasoning from Observations for Efficient Augmented Language Models](https://github.com/billxbf/ReWOO)
[Reasoning without Observation](https://langchain-ai.github.io/langgraph/tutorials/rewoo/rewoo/)


### Language Agent Tree Search (LATS)
[Language Agent Tree Search (LATS)](https://langchain-ai.github.io/langgraph/tutorials/lats/lats/)

### Self-Discover Agent
[Self-Discover](https://langchain-ai.github.io/langgraph/tutorials/self-discover/self-discover/)

### memgpt
[memgpt](https://memgpt.ai/)
[code](https://github.com/cpacker/MemGPT)

### Others
- [CODE GENERATION WITH GENERATED TESTS](https://arxiv.org/pdf/2207.10397)
- [*code*](https://github.com/microsoft/CodeT)

## Tools
[tavily](https://tavily.com/)

## ClearML
https://clear.ml/docs/latest/docs/
