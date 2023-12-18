# A3C-Learning-Learning-Kung-Fu

# Description
You are a Kung-Fu Master fighting your way through the Evil Wizard’s temple. Your goal is to rescue the Princess, defeating various enemies along the way.

# Actions
KungFuMaster has the action space of Discrete(14) with the table below listing the meaning of each action’s meanings. To enable all 18 possible actions that can be performed on an Atari 2600, specify full_action_space=True during initialization or by passing full_action_space=True to gymnasium.make.

![Capture 1](https://github.com/Mandar13022/A3C-Learning-Learning-Kung-Fu/assets/112116535/d1e840ea-ed11-4ddf-9d62-9a073629cef3)

# Observations
Atari environments have three possible observation types: "rgb", "grayscale" and "ram".
obs_type="rgb" -> observation_space=Box(0, 255, (210, 160, 3), np.uint8)
obs_type="ram" -> observation_space=Box(0, 255, (128,), np.uint8)
obs_type="grayscale" -> Box(0, 255, (210, 160), np.uint8), a grayscale version of the “rgb” type
See variants section for the type of observation used by each environment id by default.

# Variants
KungFuMaster has the following variants of the environment id which have the following differences in observation, the number of frame-skips and the repeat action probability.

![Capture2](https://github.com/Mandar13022/A3C-Learning-Learning-Kung-Fu/assets/112116535/055cae41-7b15-47f7-af92-f095342d834e)

# Difficulty and modes
It is possible to specify various flavors of the environment via the keyword arguments difficulty and mode. A flavor is a combination of a game mode and a difficulty setting. The table below lists the possible difficulty and mode values along with the default values.

![Capture3](https://github.com/Mandar13022/A3C-Learning-Learning-Kung-Fu/assets/112116535/4fc623b4-33be-4152-b0c2-25580e9f158c)
