ENVIRONMENT SETUP:

1-Enviroment creation in Python though Anaconda:
    Command: conda create -n <env_name> python=3.8

2-Activate the environment:
    Command: conda activate <env_name>

3-Connect enviroment to VS Code:
    Command: conda install ipykernel
    Command: python -m ipykernel install --user --name <env_name> --display-name "<env_name>"
    Command: Open VS Code: install Python extension and select the created environment from the bottom left corner.

4-Install the required packages:
    Command: pip install FiftyOne pandas opencv numpy matplotlib scikit scikit-image= seaborn tqdm cvat    

After the set up of the steps mentioned above, you can start to work in VS Code with the created environment and the installed packages. 
Make sure to check the versions of the installed packages to ensure compatibility with your project requirements.