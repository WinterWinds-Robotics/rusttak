# rusttak
A Rust Implementation of TakServer

Currently - this readme helps setup and configure a Centralized TAK Server.


To set up an FTS Server, which is the fully featured federated TAK server. Follow the following steps.

There are two gotchas. 

1. python3 must resolve to python3.8.10 via aliasing or symlinking. The install script for installing the server assumes it can do a "python3 -m pip install and it install libraries relevant to Python3.8.
2. ports must be created in the firewall for the following services.
3. API =
4. SSL =
5. TCP = 
6. Webserver = 
7. 

# Instructions for setting up FreeTakServer on a brand new Ubuntu 20.04 server.

first we will ensure that when the freetakserver script called python3 it resolves to python3.8. I intend to use pyenv in the future or docker.
sudo apt update
sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev wget libbz2-dev
sudo apt-get install build-essential checkinstall
sudo apt autoremove
sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev zlib1g-dev
cd /opt
sudo wget https://www.python.org/ftp/python/3.8.10/Python-3.8.10.tgz
sudo tar xzf Python-3.8.10.tgz
ls -la
sudo rm -f Python-3.8.10.tgz
cd Python-3.8.10
sudo ./configure --enable-optimizations
sudo make altinstall
python3.8 -V

sudo nano ~/.bashrc
alias python3.8=python3

# run install script. 

This script will install all sorts of components like nodered and murmur that we may not want later but I don't have any reason to exclude these components presently.

wget -qO - bit.ly/ftszerotouch | sudo bash



