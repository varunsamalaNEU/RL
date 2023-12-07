# Deep Q-learning

This page contains the readings and homework assignments for the Unit: Deep Q-learning

We will be following the contents of the DQN tutorial on pytorch.org

By the end of this unit, you should be able to write a Deep Q-Learning policy and train it to perform a pole balancing task. You should be able to understand the concepts underlying the use of neural networks to approximate the Q-table.

You should have already installed Pytorch in the previous Unit (Unit 3: Understanding Pytorch). If not, you can follow the installation instructions below

1. Additional Installation instructions
   * Install Pytorch with:
    ```
        conda install pytorch torchvision torchaudio cpuonly -c pytorch
    ```
    * For those with a NVIDIA GPU, you can install the version with GPU support to speed up training:
    ```
        conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
    ```
    * Verify that your Pytorch installation is correct with:
    ```
        import torch
        x = torch.rand(5, 3)
        print(x)
    ```
    * You should get an output like
    ```
        tensor([[0.3380, 0.3845, 0.3217],
                [0.8337, 0.9050, 0.2650],
                [0.2979, 0.7141, 0.9069],
                [0.1449, 0.1132, 0.1375],
                [0.4675, 0.3947, 0.1426]])
    ```

2. Guided readings
    * Read the sections in [huggingface.co - Unit 3](https://huggingface.co/learn/deep-rl-course/unit3/introduction?fw=pt)
        * Introduction
        * From Q-learning to Deep Q-Learning
        * The Deep Q-Network (DQN)
        * The Deep Q Algorithm
        * Glossary

3. Exercises:
    Deep Q-Learning exercise is adapted from this Pytorch [tutorial](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
    1. Enable your Anaconda environment and run the Jupyter kernel with:
    ```
        conda activate rlstudy
        jupyter-notebook
    ```
    2. Copy the generated link to the token to any web browser to run 
    3. Create a new .ipynb in your folder
    4. Follow the Pytorch tutorial to implement the Deep Q-network and train it on the Cartpole environment

4. Additional readings/videos
    * Watch the video on [Deep Q-learning](https://youtu.be/Psrhxy88zww?t=1552)