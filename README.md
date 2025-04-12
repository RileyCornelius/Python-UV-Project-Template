# Project

## VSCode Setup

### Install Python Extension
There are several Python extensions recommended in the `.vscode/extensions.json` file. You will be prompted to install them when you open the project in VSCode. If you are not prompted, you can install them manually later.

### Install UV Python Manager
UV is a Python package manager that helps manage virtual environments and dependencies. The following command will install UV globally on your system.

1. Open a new terminal `ctrl + shift + ~`
2. Install uv on Windows with `powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"`
3. To update uv run `uv self update`

### Create a Virtual Environment and Update Dependencies
Create a virtual environment and install the dependencies listed in the `pyproject.toml` can be done with the following command `uv sync`.
This command will create a virtual environment in the `.venv` folder and install the dependencies listed in the `pyproject.toml` file. The same command can be used to update the dependencies in the virtual environment.

#### Task
1. Open the command palette `ctrl + shift + p`
2. Type `Run Task`
3. Select `uv sync` 

#### Terminal
1. Open a new terminal `ctrl + shift + ~`
2. Run `uv sync` 

### Run
Once the virtual environment is created and the dependencies are installed, you can run the project using the virtual environment. VSCode will automatically detect the virtual environment and use it when running the project.

#### VSCode
1. Open the main.py file
2. Press the play button at the top right of VSCode
 
#### Terminal
1. Open a new terminal `ctrl + shift + ~` this will activate the virtual environment 
2. Run `python src/main.py` or `uv run src/main.py`