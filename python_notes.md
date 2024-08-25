Create Virtual Env

 python3 -m venv virutalEnvs/practice

Activate virtual env .

source virutalEnvs/practice/bin/activate

Install Packages

python3 -m pip install pylance

Run package

python -m mypy python/typeCheck.py

Code guidelines

black - Proper formatting
mypy -
python -m flake8 headlines.py


Strict mypy 

python -m mypy --strict headlines.py
