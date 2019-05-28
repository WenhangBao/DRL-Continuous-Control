### Report
## RL algorithm

For this problem I use Deep Deterministic Policy Gradient (DDPG) algorithm. I use 20-agent environment. These agent share the same replay buffer and has no other kinds of information sharing during the training process. 

The actor network has 2 hidden layers, both fully connected and with 400 and 300 neurons respectively. The network use ReLu as non-linear activation function. THe output layers use Tanh as the activation function and return a vector of length 4. 

The critic Network has 2 hidden layers with the same model atchitecture. The only difference is that Critic network return a scaler which is the estimated Q-value.

USe Adam optimized to optimize both Actor and Critic Network.

Hyperparameters:
BUFFER_SIZE = int(1e5)  # replay buffer size
BATCH_SIZE = 128        # minibatch size
GAMMA = 0.99            # discount factor
TAU = 1e-3              # for soft update of target parameters
LR_ACTOR = 1e-4         # learning rate of the actor 
LR_CRITIC = 1e-3        # learning rate of the critic
WEIGHT_DECAY = 0        # L2 weight decay

## Results

This environment is condiderd 
