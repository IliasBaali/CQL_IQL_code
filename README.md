# Conservative Q-Learning - Implicit Q-Learning

In this folder, we provide two notebook implementations of CQL and IQL to solve the Mujoco Hopper environment.
These implementations follow the work detailed the recommendations and algorithms detailed in the original papers introducing [CQL](https://arxiv.org/abs/2006.04779) and [IQL](https://arxiv.org/abs/2110.06169).

#### Installation instructions 

These two notebooks can be run using the environment that was used in HW2. Since the code uses Mujoco for the environment, it is not supported on Windows setups. However, PACE and/or Google Collab should work fine.

If you need to recreate the environment, you can do so as follows:

1. Create the environment & install the dependencies
```console
conda env create -f env.yaml
```

2. Activate the environment
```console
conda activate cs8803drl_hw2
```

3. Install Mujoco<br />
This is the most annoying part, as issues are common with Mujoco installation. 
Installation instructions for Mac and Linux can be found [here](https://github.com/openai/mujoco-py?tab=readme-ov-file#install-mujoco). You only need to do stuff in the section named 'Install MuJoCo'. 
For Windows users, we recommend either running with Google Colab or PACE.

4. (Optional) Depending on where you create your environment, you might need to link it to a Jupyter kernel. You can do so by running:
```console
pip install notebook ipykernel
```
```console
python -m ipykernel install --user --name=venv --display-name "Python (IQL_CQL_env)"
```
You will then need to select the kernel named "Python (IQL_CQL_env)" in Jupyter.
