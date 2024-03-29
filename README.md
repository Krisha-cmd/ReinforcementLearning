# ReinforcementLearning
Teaching agents through trial and error,
an agent learns on the basis of the reward it gets. (Utility Agents)

Agent: The actor/operator within an environment governed by a rule (ml model or a person)

Environment: the world in which agent can operate

Action: the agent can make these moves to interact with the environment

Reward and observation: In return for an action and the perception of a changed environment after the action


Applications of Reinforcement Learning:
- Autonomous driving
- Openworld Environments
- Securities Trading
- Neural network architecture
- Simulated Training of Robots
- Gaming

Limitations and considerations
- overkill for simple problems
- assumes the environment is markovian (future state is based on current state, no random changes, completely deterministic world)
- training can take a long time

# Project

## dependencies
- stable-baselines3[extra] reinforcement learning library for model free algorithms

- OpenAI gym for simulated environments https://gym.openai.con/docs/

## Load and Understand Environment

- openAI spaces to represent gymn environments

1. Box- continuous range Box(0,1,shape=(3,3))
2. Discrete- set of items Discrete(3)
3. Tuple - tuple of different spaces Tuple((Discrete(2), Box(0,100,shape=(1,)))) but stable-baselines doesn't support tuple
4. Dict dictionary of spaces Dict(('height':Discrete(2),"speed":Box(0,100,shaoe=(1,))))
5. MultiBinary - one hot encoded bin values MultiBinary(4) 0000, 0001, 0010....
6. Multidiscrete - Multidiscrete([5,2,2]) 000,100,200,300,400,010,001,011,110,101,111,.....


## Train RL model

## Evaluation

## Testing

## Logging

## Training Callback

## Changing policies

## Algorithms