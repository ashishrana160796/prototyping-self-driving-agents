## liveProject: Reinforcement Learning for self driving vehicles

This github repository contains implementations of _liveProject: Reinforcement Learning for self driving vehicles_ for reference purposes. This repository includes two different types of implementations. First, containing agent implementations from scratch and second approach uses `stable-baselines` or `rl-agents` like packages to directly import algorithms for fast prototyping to evaluate the performance of the models.

In this liveProject we explore the tools, techniques and methodologies used by AI researchers to quantify the performance of an agent in a given environment to achieve a given task. The use-case that we explore is navigating and performing different tasks across multiple driving environments. We explore different basic and abstract driving environments for prototyping some RL algorithm implementations in this beginner centered `up-for-grabs` liveProject.

## Agent implementations for milestones

This liveProject is analyzed based on three simple working principles in AI: optimize, explore & simplify. The practical applications of these concepts are elaborated over from Milestone Two, Three & Four. Also, we have an introduction Milestone that focuses primarily on visualization techniques.

### Milestone One: Visualization

* __Milestone One:__ **Visualization** in Reinforcement Learning for problem & result analysis.
  * Getting started with Google Colab environments & notebooks with OpenAI.
  * Introduction to RL with _Value Iteration_ and _Policy Iteration_ algorithms in simple environments.
    * Limitations for _Value Iteration_ and _Policy Iteration_ algorithms even in `taxi-v3` scenario.
    * Value function approximation implementation with Q-table and exploration for OpenAI's `MountainCar-v0` environment.
  * Developing _Value Iteration_, _Policy Iteration_ & _Q-Learning_ for MDP based driving scenarios in `highway-env` package.
  * __Deliverable One:__ Comparative result **Visualizations** for discussed algorithms in MDP based driving scenarios.
  
### Milestone Two: Optimize

<p align="center">
  <img src="milestone-two/assets/reward-threshold-0.2.gif" width="276" />
  <img src="milestone-two/assets/reward-threshold-0.22.gif" width="276" />
</p>
<p align="center">
<b>Figure 2:</b> Reward Shaping approach output <em>(Middle)</em> & its Optimized Iteration output <em>(Right)</em> respectively.
</p>

* __Milestone Two:__ **Optimizing** a given agent's performance to its fullest potential.
  * Setting up Google Colab notebooks for rendering OpenAI environments outputs.
  * Handling sparse rewards scenarios in goal based environments like `MountainCar-v0` environment.
  * __Deliverable Two:__ Evaluating & documenting variations in agent behavior for our hand-built reward functions to develop the most **optimized** agent in `MountainCar-v0` for this approach.

### Milestone Three: Explore

<p align="center">
  <img src="milestone-three/assets/deliverable-two-graph-output.png"/>
</p>
<p align="center">
<b>Figure 3:</b> Mean average reward plot for performance evaluation of SAC, TD3 & DDPG equipped with HER.
</p>

* __Milestone Three:__ **Exploring** new algorithms for achieving better performance in goal based driving tasks.
  * _State–action–reward–state–action (SARSA lambda)_ agent implementation for `MountainCar-v0` environment to learn agent designing concepts. [Colab Implementation Link](https://colab.research.google.com/drive/1wwjP-Rr8GmvLO9P39scbjUOamVBv_6Nx?usp=sharing)
  * **Exploring** new RL algorithms for goal based parking task on `highway-env` package with _HER_ and _SAC_ from `stable-baselines3` RL algorithms package. [Colab Implementation Link](https://colab.research.google.com/drive/1vQnslmenp5c95jVAwVEl7xXspgc3IPqx?usp=sharing)
  * __Deliverable Three:__ Implementation, Analysis and Documentation of _HER_ supported algorithms like _DDPG, TD3 and SAC_ for parking task on third party _highway-env_ package in `parking-v0` environment.

Also, we provide the rendering alternative implementation reference implementation as well as part of this milestone to get you started with `highway-env` package on Colab. [Colab Implementation Link](https://colab.research.google.com/drive/1zWn1Cm2bOAud26wSpcXt3ewUB6R5tF6z?usp=sharing)

Additionally, if you are interested in reviewing the code base of a stable-baselines package and you have background only in Tensorflow. You can refer to the tensorflow backend based implementation of HER based SAC agent as well, just to see turnarounds required for running stable-baselines with Tensorflow. [Colab Implementation Link](https://colab.research.google.com/drive/1RHxj9WOcZ8XjlQXGu46RKVG6T-jA2dU-?usp=sharing)

### Milestone Four: Simplify

* __Milestone Four:__ Designing plan oriented agents that use searching capabilities to navigate across optimal paths in an environment.
  * _Monte Carlo Tree Search (MCTS)_ Implementation for Toy Text `Taxi-v3` environments.
  * Introduction to navigation environments in `highway-env` package and MCTS agent prototyping for all these navigation based tasks with `rl-agents` package.
  * __Deliverable 3:__ Creating a MCTS learning and evaluation functional structure to evaluate the agent performance for different environments present in `highway-env` package.
    * The current generic implementation doesn't work optimally for these different environments in `highway-env` package. You can skip the optimization and performance analysis part.

### Certification Test

* __Certification Test:__ Final certification test checks the understanding developed by you during the liveProject.

<p align="center">
  <img src="certification-test/assets/mcts-agent.gif" width="250" />
  <img src="certification-test/assets/mcts-gape-agent.gif" width="250" />
  <img src="certification-test/assets/mcts-opd-agent.gif" width="250" />
</p>
<p align="center"><b>Figure 4:</b> Outputs of different trained MCTS agents with same parameters that are under evaluation in certification test.</p>

### Building Your Own Environment

This is a supplementary section that covers an additional topic of making a custom environment as per one's need.

* __Building Custom Environments__ In this notebook we create a sample environment for _highway-env_ package and use the _rl-agent_ package to create a baseline planner agent corresponding to that environment. [Colab Implementation Link](https://colab.research.google.com/drive/1PoSbv_o1I9tkCIsCRn3lBYzcRGH_qVAu?usp=sharing)

<p align="center">
  <img src="building-custom-environments/assets/mcts-agent.gif" width="276" />
  <img src="building-custom-environments/assets/deterministic-agent.gif" width="276" />
</p>
<p align="center"><b>Figure 5:</b> U-Turn environment baseline agents namely MCTS Agent <i>(Left)</i> and Deterministic Agent <i>(Right)</i>.</p>

## Acknowledgements

* Thank you to ![@Edouard Leurent](https://github.com/eleurent) for providing and maintaining the ![`highway-env`](https://github.com/eleurent/highway-env) and ![`rl-agent`](https://github.com/eleurent/rl-agents) packages.
* Thanks to ![`stable-baselines`](https://github.com/DLR-RM/stable-baselines3) team and  ![@Ashley Hill ](https://github.com/hill-a) for providing efficient and well documented implementations of RL algorithms in a single ![package](https://github.com/DLR-RM/stable-baselines3).
* Also, thanking  ![@Ashok Tankala](https://github.com/tankala) for an interesting implementation use-case of reward shaping.
