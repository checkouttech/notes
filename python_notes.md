Install uv:

    Curl:
    curl -LsSf https://astral.sh/uv/install.sh | sh

    pip: 
    pip install uv

    # Update uv to latest
    uv self update 

Install Python:

    uv : 

        Download from python.org and install manually 
    
        To list all instances of python
            uv python list
            uv python list --only-installed

        To install a Python version at a specific version:
            uv python install 3.12.3


    Brew :
 
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
        export PATH="/usr/local/opt/python/libexec/bin:$PATH"
 
        brew reinstall python


       
Create Virtual Env:

    uv : 
        
        To create a specific version of Venv
        uv venv  --python 3.12.5   virutalEnvs/uvExample3.12.5

    classic :

        python3 -m venv virutalEnvs/practice


Activate virutal env:

    source virutalEnvs/practice/bin/activate


Install Packages

    uv : 
        # install packages
        uv pip install <module>
        uv add django requests "pandas>=2.3"

        # To remove a package 
        uv remove django

        # To install modules from pyproject 
        uv pip install -r pyproject.toml

        # To install modules from requirement.txt  
        uv pip install -r requirement.txt    

    classic :
    
        python3 -m pip install "package-name"
        pip3 install "package-name"  # this one works for sure 



Get list of installed Packages

    uv pip freeze 
    uv pip list --format <format>   ( columns, freeze, or json ) 
         
    # To generate requirements.txt  from a pyproject.toml 
    uv pip compile pyproject.toml -o requirements.txt

    # To sync an existing environment with a requirements.txt or pyproject file :
    uv pip sync pyproject.toml
    uv pip sync requirements.txt

    ## see pkg dependency tree
    uv tree


Type Checking:

    python -m mypy --strict  [PY-SCRIPT]  

    python3 -m ruff check  [PY-SCRIPT]  


Code Linter and Formatters:

    python3 -m ruff format [PY-SCRIPT] 
    
    python3 -m ruff format --line-length 200 [PY-SCRIPT]

    python -m ruff format --diff [PY-SCRIPT]    # to auto fix 


To create project:

    uv init —name uv-tutorial


Run a python script directly w/o starting venv

    uv run main.py



Start a new project and pin it to Python 3.12:

    uv init myproject
    uv python pin 3.12
    uv add django
    uv run main.py (will automatically install py3.12 and django into venv)


Install tools: 

    python3 -m pip install --upgrade setuptools
    python3 -m pip install --upgrade pip


Update pip:

    python3 -m pip install --upgrade pip
    python -m pip install pip==21.3.1  # if a particular version needs to be installed 

Check pip version 

    python3 -m pip --version

      
   Other options 
      black - Proper formatting
      flake8  


Type checking --- 
 python3 -m pyright    [PY-SCRIPT]  
 python3 -m pylint    [PY-SCRIPT]  
 python3 -m pyflakes  [PY-SCRIPT]  




Type Checkers
mypy, the reference implementation for type checkers.
pyre, a type checker written in OCaml and optimized for performance.
pyright, a type checker that emphasizes speed.
pytype, a type checker that checks and infers types for unannotated code.




Install virtual env
  pip3 install virtualenv



run a cli tool like Ruff:

    uv run tool ruff (or uvx ruff)


To update dependencies in the lock file:

    uv lock —upgrade

