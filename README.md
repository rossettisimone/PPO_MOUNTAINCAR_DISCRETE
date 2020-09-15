# PPO_MOUNTAINCAR_DISCRETE
Proximal Policy Optimization Algorithm applied to MountainCar in discrete environment.

[![Watch the video](/media/mount.gif)](/media/video.mp4)

**Author:**

*Simone Rossetti, Roma, January 2020*

**Framework:** 

PyTorch

**Abstract:** 

PPO algorithm is a new kind of policy gradient method for reinforcement learning, in which this kind of methods are an appealing approach because they directly optimize the cumulative reward and can straightforwardly be used with nonlinear function approximators such as neural networks.
PPO alternates between sampling data through interaction with the environment, and optimizing a surrogate objective function using stochastic gradient ascendent.
The algorithm shown in the picture below is a generic representation of a proximal policy optimization method.
Whereas standard policy gradient methods perform one gradient update per data sample, it proposes a different objective function that enables multiple epochs of mini-batch updates.

**Environment**

MountainCar environment is very simple, for each step where the car does not reach the goal, located at position 0.5, the environment returns a reward of -1. So the aim is to reach the goal in less time, as to maximize the reward. Possible actions are ‘right’ +1, ‘stay’ 0, ‘left’ -1. Performing one of each action separately does not allow the agent to reach the goal. Instead, the model should learn such policy that permits the agent to exploit the required inertia to reach the top of the mountain.

**Top reward:**

Best Reward -96.200 in 420 epochs (mean on 10 tests each 10 epochs)

<p align="center" width="100%">
<img src="/media/res.png" alt="" width= '50%'/>
</p>
