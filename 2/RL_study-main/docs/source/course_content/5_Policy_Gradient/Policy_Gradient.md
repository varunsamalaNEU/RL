# Policy Gradient methods for RL

This page contains the readings and homework assignments for the Unit 4: Policy Gradient with Pytorch

We will be following the content of the Deep RL course: [Unit 4 - Policy Gradient with Pytorch](https://huggingface.co/learn/deep-rl-course/unit4/introduction?fw=pt) on huggingface.co

Upon completing this unit, you should be able to understand the theory behind policy gradient methods, together with their advantages and disadvantages in their application. You should also be able to implement the Reinforce algorithm and train a policy on a pole balancing task.

1. Guided readings
    * Review the content in the sections of [Unit 4 - Policy Gradient with Pytorch](https://huggingface.co/learn/deep-rl-course/unit4/introduction?fw=pt)
        * Introduction
        * What are the policy-based methods?
        * The advantages and disadvantages of policy-gradient methods
        * Diving deeper into policy-gradient
        * The Policy Gradient Theorem
        * Glossary

2. Exercises:
    
    You will be implementing the Reinforce algorithm in the [Hands-on section](https://huggingface.co/learn/deep-rl-course/unit4/hands-on?fw=pt)
    * There will be some key differences in the implementation, since we are using the CPU version of Pytorch.
        * 'to(device)' lines are removed, since we are not using a GPU
        * Remember that env.reset() returns a list of outputs, instead of a single observation. Extract just the observations when resetting the environment with env.reset()[0].
    * If you get stuck anywhere in the tutorial, refer to the provided Jupyter notebook for the sample solution

3. Additional readings/videos:
    * Read Chapter 13 of the book (http://incompleteideas.net/book/RLbook2020.pdf)
    * [Spinning Up - Intro to Policy Optimization](https://spinningup.openai.com/en/latest/spinningup/rl_intro3.html#deriving-the-simplest-policy-gradient)
    * [Policy Gradients - Part 1](https://jonathan-hui.medium.com/rl-policy-gradients-explained-9b13b688b146)
    * [Policy Gradients - Part 2](https://jonathan-hui.medium.com/rl-policy-gradients-explained-advanced-topic-20c2b81a9a8b)