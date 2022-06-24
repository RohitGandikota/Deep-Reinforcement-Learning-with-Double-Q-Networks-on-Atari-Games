## Deep-Reinforcement-Learning-with-Double-Q-Networks-on-Atari-Games
This project uses deep RL to train an agent that can play Atari game named Space Invaders. 
### Deep Reinforcement Learning
With deep reinforcement learning, we use deep neural networks to estimate the q-values that are used to take an action (used in policy). In many practical decision making problems, the states s {\displaystyle s} s of the MDP are high-dimensional (eg. images from a camera or the raw sensor stream from a robot) and cannot be solved by traditional RL algorithms. Deep reinforcement learning algorithms incorporate deep learning to solve such Maps a, often representing the policy π ( a | s ) or other learned functions as a neural network, and developing specialized algorithms that perform well in this setting.

## Installations

The following steps can be considered before installing gym and atari-py in Windows Anaconda. [Linux Installation is straight forward]

Step 1: Create a new environment in anaconda: 
```
conda create -n <env_name> python=3.9
conda activate <env_name?
```

Step 2: [Depends on Visual Studio]. If Visual Studio is not present please download and install
   - Download VS build tools [here](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16)
   - Run the VS build setup and select "C++ build tools" and install it.

Step 3: Packages Installation in the created environment [Using Pip]
```
pip install tensorflow
pip install cmake
pip install atari-py
pip install gym
pip install gym[atari]
pip install keras-rl2
```

Step 4: With the latest atari-py verions, only `Tetris` game is available. To get all the games:
   - Download the ROMS from [this link](http://www.atarimania.com/rom_collection_archive_atari_2600_roms.html)
   - Unrar the folder at any location
   - Run the below code in the conda prompt
```
python -m atari_py.import_roms <path to folder where ROMS are unrared>
```

Step 5: Enjoy Coding !!!
