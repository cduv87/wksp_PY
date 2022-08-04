


# install system python3 pip package

sudo apt-get install python3-pip

# create virtual environment without pip and with access to system site packages

python3 -m venv myvenv --without-pip --system-site-packages


# You can use system pip module to install python packages into your virtual environment now.

# Instead of 

pip install Django 

# you have to use explicit

myvenv/bin/python3 -m pip install Django

# or you may activate your virtual environment first

source myvenv/bin/activate 
python3 -m pip install Django

# .

python3 -m pip --version 

# may comes handy to see which python environment is used.

* source : https://askubuntu.com/questions/879437/ensurepip-is-disabled-in-debian-ubuntu-for-the-system-python *