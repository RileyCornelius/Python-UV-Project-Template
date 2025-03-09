# Project

## VSCode Setup

### Install UV Python Manager
1. Open a new terminal `ctrl + shift + ~`
2. Install uv on Windows with `powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"`
3. To update uv run `uv self update`

### Create a virtual environment or Update Dependencies

#### Task
1. Open the command palette `ctrl + shift + p`
2. Type `Run Task`
3. Select `uv sync` 

#### Terminal
1. Open a new terminal `ctrl + shift + ~`
2. Execute `uv sync` 

### Run

#### VSCode
1. Open the main.py file
2. Press the play button at the top right of VSCode
 
#### Terminal
1. Open a new terminal `ctrl + shift + ~` this will activate the virtual environment 
2. Execute `python src/main.py` or `uv run src/main.py`