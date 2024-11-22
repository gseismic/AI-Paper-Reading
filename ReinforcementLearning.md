

## Papers
- [Addressing Function Approximation Error in Actor-Critic Methods](https://arxiv.org/pdf/1802.09477)
- [Time Limits in Reinforcement Learning](https://arxiv.org/pdf/1712.00378)

## Topics
### Time Limits
- [Time Limits in Reinforcement Learning](https://arxiv.org/pdf/1712.00378)
- [Filtering out artificial terminal states in time-limited RL](https://github.com/hill-a/stable-baselines/issues/863)
- [PPO Implementation Ignores Time Limits](https://github.com/luchris429/purejaxrl/issues/20)
- [When should TimeFeatureWrapper be used](https://github.com/araffin/rl-baselines-zoo/issues/79)
- [Enabling agents to keep bootstraping in the last step per episode](https://github.com/hill-a/stable-baselines/issues/1004)

### Exploration
- [Smooth Exploration for Robotic Reinforcement Learning](https://arxiv.org/pdf/2005.05719)

### Gradient
- [Gradient accumulation](https://github.com/huggingface/trl/issues/2175)

## Links
- [Awesome Reinforcement Learning](https://github.com/aikorea/awesome-rl)
- [cleanrl](https://github.com/vwxyzjn/cleanrl)
- [gymnasium](https://gymnasium.farama.org/main/introduction/migration_guide/)
- [gymnasium-v1](https://github.com/Farama-Foundation/Gymnasium/releases/tag/v1.0.0)
- [gym.multi-agent](https://shimmy.farama.org/environments/dm_multi/)
- [gym.lab](https://shimmy.farama.org/environments/dm_lab/)
- [mujoco](https://github.com/google-deepmind/mujoco)

## Code
[stable-baselines3](https://stable-baselines3.readthedocs.io/en/master/guide/examples.html)
[PPO-cleanrl](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo.py)
[ppo-implementation-details](https://github.com/vwxyzjn/ppo-implementation-details)
[ppo-impl2](https://iclr-blog-track.github.io/2022/03/25/ppo-implementation-details/)


### PPO
- [The 37 Implementation Details of Proximal Policy Optimization](https://github.com/vwxyzjn/ppo-implementation-details?tab=readme-ov-file)
    - [blog](https://iclr-blog-track.github.io/2022/03/25/ppo-implementation-details/)
- [RL — Proximal Policy Optimization (PPO) Explained](https://jonathan-hui.medium.com/rl-proximal-policy-optimization-ppo-explained-77f014ec3f12)
[Part 1 of 3 — Proximal Policy Optimization Implementation: 11 Core Implementation Details](https://www.youtube.com/watch?v=MEt6rrxH8W4)
[spinningup.openai](https://spinningup.openai.com/en/latest/algorithms/ppo.html#id3)
[What Matters In On-Policy Reinforcement Learning? A Large-Scale Empirical Study](https://arxiv.org/abs/2006.05990)
    - [blog](https://vitalab.github.io/article/2020/07/02/What_Matters_in_RL.html)
    - [paper](https://arxiv.org/abs/2006.05990)
[Robust Policy Optimization (RPO)](https://arxiv.org/pdf/2212.07536)
    - [detail](https://docs.cleanrl.dev/rl-algorithms/rpo/#implemented-variants)

A quote from the PPO paper:

```
Q-learning (with function approximation) fails on many simple problems and is poorly understood, vanilla policy gradient methods have poor data efficiency and robustness; and trust region policy optimization (TRPO) is relatively complicated, and is not compatible with architectures that include noise (such as dropout) or parameter sharing (between the policy and value function, or with auxiliary tasks).
```
PPO adds a soft constraint that can be optimized by a first-order optimizer. We may make some bad decisions once a while but it strikes a good balance on the speed of the optimization. Experimental results prove that this kind of balance achieves the best performance with the most simplicity.
