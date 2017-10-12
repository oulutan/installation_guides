1 - Update and Install the basic tools

sudo apt-get update

sudo apt-get upgrade 

sudo apt-get install htop vim tmux 

2 - Setup pip without sudo

Download https://bootstrap.pypa.io/get-pip.py

Run python get-pip.py --user

It will install it into \~/.local/

Add PATH=$PATH:~/.local/bin to bashrc or bash_profile

3 - Setup python tools

pip install virtualenv numpy scipy ipython pdbpp tqdm scikit-learn scikit-image six wheel pandas matplotlib pdbpp sympy nose

4 - 
