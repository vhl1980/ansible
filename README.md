# ansible
Take on ansible molecule


```
sudo apt update && sudo apt upgrade -y
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.9
sudo apt install python3.9-distutils
sudo apt-get install python3.9-dev python3.9-venv
python3.9 -m pip install --upgrade pip

python3.9 -m venv molecule
source molecule/bin/activate
python3.9 -m pip install --upgrade pip
# don't need to install ansible because molecule install it
python3.9 -m pip install "molecule"
python3.9 -m pip install "molecule[lint]"
python3.9 -m pip install "molecule[docker]"
ansible-galaxy collection install community.docker
ansible-galaxy collection install ansible.posix

deactivate
```
