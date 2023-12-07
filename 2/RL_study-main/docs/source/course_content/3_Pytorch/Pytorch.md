# Understanding Pytorch

This page contains the readings and homework assignments for the Unit: Deep Q-learning

We will be following the contents of the DQN tutorial on pytorch.org

By the end of this unit, you should be familiar with concepts of tensors and gradient calculations. You will also gain an understanding of the functions provide by Pytorch to build your own neural networks.

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

2. Guided readings / Exercises:
    * Understand the basic Pytorch functions. Please go through the videos and code each section below. Create your own Jupyter notebooks to run these tutorials:
        * [Introduction](https://pytorch.org/tutorials/beginner/introyt/introyt1_tutorial.html)
        * [Tensors](https://pytorch.org/tutorials/beginner/introyt/tensors_deeper_tutorial.html)
        * [Gradient calculations with Autograd](https://pytorch.org/tutorials/beginner/introyt/autogradyt_tutorial.html)
        * [Building Models with neurons and layer](https://pytorch.org/tutorials/beginner/introyt/modelsyt_tutorial.html)
        * [Model training](https://pytorch.org/tutorials/beginner/introyt/trainingyt.html)
        * [Explaining your Models](https://pytorch.org/tutorials/beginner/introyt/captumyt.html)
        * [Visualization with Tensorboard](https://pytorch.org/tutorials/beginner/introyt/tensorboardyt_tutorial.html)