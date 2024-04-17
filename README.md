# Software Installation
## Installing Miniconda
### Windows
1. [Download the installer ](https://docs.anaconda.com/free/miniconda/)
2. Double-click the .exe file.
3. Follow the instructions on the screen. If you are unsure about any setting, accept the defaults. You can change them later.
4. When the installation finishes, from the Start menu, open Anaconda Prompt.
5. Test your installation by running `conda list`. If conda has been installed correctly, a list of installed packages appears.

### macOS
1. [Download the installer ](https://docs.anaconda.com/free/miniconda/)
2. Double-click the .pkg file.
3. Follow the instructions on the screen. If you are unsure about any setting, accept the defaults. You can change them later.
4. When the installation finishes, open your terminal application.
5. Test your installation by running `conda list`. If conda has been installed correctly, a list of installed packages appears.

### Linux
1. [Download the installer ](https://docs.anaconda.com/free/miniconda/)
2. In your terminal, run the following command, replacing `filename` with the path to your installer.
```
bash filename
```
3. Follow the prompts on the installer screens. If you are unsure about any setting, accept the defaults. You can change them later.
4. To make the changes take effect, close and then re-open your terminal window.
5. Test your installation by running `conda list`. If conda has been installed correctly, a list of installed packages appears.

## Creating Conda environment
You can maintain separate environments for various versions of Python on the same computer without worrying about the programs interacting with each other. Switching to an environment is called activating it.
1. Create an environment named llmfs
```
conda create --name llmfs
```
2. To work in the `llmfs` environment, activate it by running the following command:
```
conda activate llmfs
```
It is best practice to deactivate your environment when you are finished working in it. To deactivate your active environment, run the following command:
```
conda deactivate
```

## Installing JupyterLab
1. Open Anaconda Prompt.
2. Add conda-forge repository by running the following command in the terminal:
```
conda config --append channels conda-forge
```
3. Activate the `llmfs` environment by running the following command:
```
conda activate llmfs
```
4. Install JupyterLab by running the following command:
```
conda install jupyterlab
```
5. Once installed, launch JupyterLab with:
```
jupyter lab
```

## Installing PyTorch
### Windows
1. Open Anaconda Prompt.
2. Activate the `llmfs` environment by running the following command:
```
conda activate llmfs
```
3. Install PyTorch by running the following command:
```
conda install pytorch torchvision torchaudio cpuonly -c pytorch
```

### macOS
1. Open Anaconda Prompt.
2. Activate the `llmfs` environment by running the following command:
```
conda activate llmfs
```
3. Install PyTorch by running the following command:
```
conda install pytorch::pytorch torchvision torchaudio -c pytorch
```

### Linux
1. Open Anaconda Prompt.
2. Activate the `llmfs` environment by running the following command:
```
conda activate llmfs
```
3. Install PyTorch by running the following command:
```
conda install pytorch torchvision torchaudio cpuonly -c pytorch
```