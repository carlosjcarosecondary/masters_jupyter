# jupyter
Installation of Jupyter in AWS
====

1. Deploying an EC2 intance with a public IP

2. Server commands:
* sudo apt-get install -y
* sudo apt-get install python3-pip
* sudo pip3 install jupyter
* export PATH=$PATH:~/.local/bin
* nohup jupyter notebook --ip=0.0.0.0 &

3. AWS Security Group must allow communication through the specified port

4. Installing conda
* cd /tmp
* curl -O https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh
* bash Anaconda3-2020.02-Linux-x86_64.sh
* export PATH=$PATH:/home/ubuntu/anaconda3/bin
* conda install nb_conda
* pip3 install ipykernel

5. Creating a virtual environment
* conda create -n training_env python=3.6
* python3 -m ipykernel install --user --name=training                     //adding the new env to Jupyter menu
* source ~/anaconda3/etc/profile.d/conda.sh
* conda activate env_name
* pip3 install -r requirements.txt

6. Other commands
* Getting list of packages: pip freeze -> file.txt



