# ReinforcementLearning_Algos

# Project [PushBlock](https://github.com/PGCodehub/ReinforcementLearning_Algos/tree/main/RL_Agents_Projects/Assets/ML-Agents/Projects/PushBlock)




# Project [WallJump](https://github.com/PGCodehub/ReinforcementLearning_Algos/tree/main/RL_Agents_Projects/Assets/ML-Agents/Projects/WallJump)


![alt text]( "WallJump")


About Enviroment
Set-up: A platforming environment where the agent can jump over a wall.
Goal: The agent must use the block to scale the wall and reach the goal.
Agents: The environment contains one agent linked to two different Models. The Policy the agent is linked to changes depending on the height of the wall. The change of Policy is done in the WallJumpAgent class.

Agent Reward Function:

-0.0005 for every step.
+1.0 if the agent touches the goal.
-1.0 if the agent falls off the platform.
  
  
Behavior Parameters:
Vector Observation space: Size of 74, corresponding to 14 ray casts each detecting 4 possible objects. plus the global position of the agent and whether or not the agent is grounded.


Vector Action space: (Discrete) 4 Branches:

Forward Motion (3 possible actions: Forward, Backwards, No Action)
Rotation (3 possible actions: Rotate Left, Rotate Right, No Action)
Side Motion (3 possible actions: Left, Right, No Action)
Jump (2 possible actions: Jump, No Action)

Visual Observations: None
Float Properties: Four
Benchmark Mean Reward (Big & Small Wall): 0.8
