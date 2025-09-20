The implemented algorithm learns a hierarchical policy using SMDP Q-learning and intra-option 
Q-learning. The macro-policy first selects an option (one of the four color-coded subgoals) 
based on the Q-table for high-level decisions. Then, a sub-policy (trained Q-table for each 
option) guides the taxi to the respective destination. The learned policy effectively minimizes the 
steps taken by choosing the best available option for reaching the passenger and then dropping 
them at the destination. 
The Q-learning updates ensure that the taxi learns to navigate efficiently by iteratively updating 
the Q-values based on observed rewards. The final learned policy follows an optimal sequence 
of actions, first moving towards the passenger and then towards the destination while avoiding 
unnecessary movements. This algorithm was experimented in OpenAI Gym’s Taxi-v3 environment