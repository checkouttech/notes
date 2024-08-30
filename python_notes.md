
Install Python ( using brew ) 

   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
   export PATH="/usr/local/opt/python/libexec/bin:$PATH"
 
   brew reinstall python


Install tools 
   python3 -m pip install --upgrade setuptools
   python3 -m pip install --upgrade pip


pip install --upgrade setuptools

Install virtual env
  pip3 install virtualenv


Create Virtual Env
  python3 -m venv virutalEnvs/practice

Activate virtual env .
  source virutalEnvs/practice/bin/activate

Update pip 
  python3 -m pip install --upgrade pip
  python -m pip install pip==21.3.1  # if a particular version needs to be installed 

Check pip version 
  python3 -m pip --version

Install Packages
  python3 -m pip install "package-name"
  pip3 install "package-name"  # this one works for sure 

 python3 -m  pip install mypy pytype pylint pyright flake8  pylance black pyflakes



*Type Checking*

   python -m mypy --strict  [PY-SCRIPT]  
   python3 -m ruff check  [PY-SCRIPT]  

*Code Linter and Formatters*
   python3 -m ruff format [PY-SCRIPT] 
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




