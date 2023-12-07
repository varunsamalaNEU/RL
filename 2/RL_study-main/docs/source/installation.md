Let's get our systems set up by installing the following software below:
(Note: For Linux/Ubuntu users, you can skip directly to the step `Install an IDE`)

## (For Windows) Install WSL
For Win 11 users:
1. Open Windows PowerShell in Administrator mode (Right-click "Run as Administrator")
2. Install with "wsl --install" command
3. Go to Microsoft Store and select your Ubuntu version (22.04) for installation
More information about WSL installation can be found [here](https://learn.microsoft.com/en-us/windows/wsl/install).

For Win 10 users:
1. Check that you have Hyper-V Virtualization Support enabled. Use this [link](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v) for instructions on how to perform this check
2. Once you confirm you have Hyper-V Virtualization, open Windows Powershell in Administrator mode
3. Install WSL with "wsl --install" command
4. Go to Microsoft Store and select your Ubuntu version (22.04) for installation

Check your WSL installation:
1. On your Command Prompt, the command `wsl -l -v` should display an output of
``` bash
  NAME            STATE       Version
  Ubuntu-22.04    Running     2
```

## Install an IDE
* The IDE of choice in this study group is VScode, which you can download [here](https://code.visualstudio.com/)
* If you are on Windows, you would need to install the WSL extension to connect the Vscode IDE to your WSL
* The WSL extension can be installed using the VScode Extension marketplace on the sidebar, as shown in the image below:

<img width="600" alt="WSL_extension" src="https://github.com/elladyr/RL_study/blob/main/docs/source/images/WSL_extension.png?raw=true">


Your system should be able to run Ubuntu from the command line (or graphically, for those with Ubuntu systems). Front this point on, commands below will only be executed on Ubuntu

## Install Ubuntu dependencies
Install dependencies for visualization of the environment using Python OpenGL bindings. These bindings are mainly used in the Huggingface tutorials.
``` bash
  sudo apt-get update
  sudo apt-get install -y python3-opengl
  sudo apt install ffmpeg xvfb
```

## Set up SSH keys for your system.
* SSH keys are required to securely access your repositories on Github. Follow the instructions [here](https://medium.com/featurepreneur/setting-up-ssh-key-with-github-for-ubuntu-cd8f2fabf25b) to set up your SSH keys and test your SSH connection to Github

## Clone this repository
1. Once you have finished the steps `Install an IDE` and `Install Ubuntu dependencies`, create a folder and clone this repository. Select the SSH version of the link to clone, as shown below:

<img width="400" alt="CloneSSH" src="https://github.com/elladyr/RL_study/blob/main/docs/source/images/GitClone_SSH.png?raw=true">

2. Clone the repository with the command:

``` bash
  git clone git@github.com:elladyr/RL_study.git
```

## Install Ananconda
1. Download the latest Linux version of [Anaconda](https://www.anaconda.com/download#downloads)
2. Copy the downloaded .sh file over to your Ubuntu file system
3. Make the file executable with `chmod +x <<downloaded file name>>`
4. Install with `./<<downloaded file name>>`

## Set up your Anaconda environment
Go into the Github folder you just cloned and create an Anaconda environment with:

``` bash
  cd RL_study
  conda create --name rlstudy python=3.9
  conda activate rlstudy
  pip install -r requirements.txt
```
  
## Test your installation
Congratulations, if you have not encountered any error messages till this point, you would have successfully installed all the dependencies required for this study group.

1. Start Jupyter notebook from the terminal(either in the IDE or from the command line) and run
``` bash
	jupyter-notebook
```
You should see something like the screenshot below:

<img width="800" alt="token" src="https://github.com/elladyr/RL_study/blob/main/docs/source/images/Jupyter_token.png?raw=true">

2. Copy the token boxed in red and paste them to your browser

3. Navigate to the folder `Q_learning` and open the file 'Q_Learning_solution.ipynb'
4. From the top menubar, select "Cell" and "Run All"
5. You should see a successful run of the Q_learning algorithm and a short video visualizing the outputs of the policy should be generated in your folder
