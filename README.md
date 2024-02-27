#Maze Environment for Reinforcement Learning
This repository contains Python code implementing a maze environment for reinforcement learning tasks. The environment is designed to be used with OpenAI Gym.

Setup
Before using the code, make sure to install the required dependencies:
```
pip install gym==0.23.0
```
Usage
Initializing the Environment
To initialize the maze environment, use the following code:
```
from maze_environment import Maze

# Initialize the environment
env = Maze()
```

Interacting with the Environment
The maze environment follows the OpenAI Gym API. You can interact with the environment using typical Gym functions such as reset() and step():

```
# Reset the environment
initial_state = env.reset()

# Take a step in the environment
next_state, reward, done, info = env.step(action)
```
Rendering the Environment
You can visualize the environment using the render() function:
```
# Render the environment
observation = env.render(mode='human')
```
Policy Iteration
The code also includes implementations of policy iteration algorithms. You can train and test policies using functions like policy_iteration() and test_agent():
```
# Perform policy iteration
policy_iteration(policy_probs, state_values)

# Test the trained agent
test_agent(env, policy)
```
Example
An example notebook demonstrating the usage of the maze environment and policy iteration algorithms is provided in example_notebook.ipynb.

Dependencies
Python 3.x
Gym (0.23.0)

Author
Suvodeep Chowdhury

License
This project is licensed under the MIT License.


