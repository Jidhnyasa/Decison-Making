# Assignment 2
## Part B
###   :Policy Iteration for MDP
Given : A 4x4 grid of the UAV perfroming reconnaissance
Actions=(north,south,east,west)
Probability of each action is 0.85
Reward: +1 for green circles, -1 for red circle, -0.05 for rest sectors.

### Calculating the policy iteration 
the discounted factor is 0.99
Ui+1(s) ← R(s) + γ sum s'(P(s'| s, πi(s))Ui(s'))
