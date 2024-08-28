
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



Run package

python -m mypy python/typeCheck.py

Code guidelines

black - Proper formatting
mypy -
python -m flake8 headlines.py


Strict mypy 

python -m mypy --strict headlines.py




