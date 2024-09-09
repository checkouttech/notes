
Install Python:
    uv : 
    
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


Activate virutal env :

  source virutalEnvs/practice/bin/activate


Install Packages

    uv pip install <module >

    python3 -m pip install "package-name"
    pip3 install "package-name"  # this one works for sure 






To install using .toml
    uv pip install -r pyproject.toml

To create project
    uv init —name uv-tutorial






Install tools 
   python3 -m pip install --upgrade setuptools
   python3 -m pip install --upgrade pip


pip install --upgrade setuptools

Install virtual env
  pip3 install virtualenv

Update pip 
  python3 -m pip install --upgrade pip
  python -m pip install pip==21.3.1  # if a particular version needs to be installed 

Check pip version 
  python3 -m pip --version



*Type Checking*

   python -m mypy --strict  [PY-SCRIPT]  
   python3 -m ruff check  [PY-SCRIPT]  

*Code Linter and Formatters*
   python3 -m ruff format [PY-SCRIPT] 
   python3 -m ruff format --line-length 200 [PY-SCRIPT]

   python -m ruff format --diff [PY-SCRIPT]    # to auto fix 

      
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




