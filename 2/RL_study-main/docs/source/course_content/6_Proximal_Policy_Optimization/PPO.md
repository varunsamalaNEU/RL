# Proximal Policy Optimization (PPO)

This page contains the readings and homework assignments for Proximal Policy Optimization

We will be following the contents of the PPO tutorial on pytorch.org

1. If Pytorch has not been installed, use the installation instructions below:
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
    * You should get an output similar to:
    ```
        tensor([[0.3380, 0.3845, 0.3217],
                [0.8337, 0.9050, 0.2650],
                [0.2979, 0.7141, 0.9069],
                [0.1449, 0.1132, 0.1375],
                [0.4675, 0.3947, 0.1426]])
    ```

2. Guided readings
    * Review the content in the sections in [Unit 8 - Part 1 Proximal Policy Optimization (PPO)](https://huggingface.co/learn/deep-rl-course/unit8/intuition-behind-ppo?fw=pt)
        * The intuition behind PPO
        * Introducing the Clipped Surrogate Objective Function
        * Visualize the Clipped Surrogate Objective Function

3. Exercises:
    You will be implementing PPO following the sample codes of [Reinforcement Learning (PPO) with TorchRL](https://pytorch.org/tutorials/intermediate/reinforcement_ppo.html).
    * The PPO version you will be implementing is the continuous version of PPO. Take note of this as there will be implementation differences in the different versions
    * Capture some performance metrics during training and evaluation to evaluate your policy.
        * Reward per episode
        * Episode duration

4. Additional readings/videos:
    * Watch the video [TROP and PPO (Foundations of Deep RL Series)](https://youtu.be/KjWF8VIMGiY)
    * Compiled PPO [implementation tips](https://iclr-blog-track.github.io/2022/03/25/ppo-implementation-details/)

5. Optional Homework:
    * As a challenge, consider training a policy with PPO to solve the [MountainCar environment](https://gymnasium.farama.org/environments/classic_control/mountain_car_continuous/). Be sure to use the continuous version of the Mountain Car.
    * Questions to ponder:
        * What kind of changes did you have to make for a successful training?
        * How do the performance metrics compare with the Inverted DOuble Pendulum environment?
        * What are the differences in the properties of the environment that would affect the policy
