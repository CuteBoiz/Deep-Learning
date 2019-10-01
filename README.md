# Deep-Learning With Keras And TensorFlow On Ubuntu Mate
<h2>I.Install Environment For Deep Learning </h2>
<h3>1. Install Python</h3>
<ul>
  <li><b>Get Lastest Python Version </b></li>
  Go to: https://www.python.org/downloads/source/ to get the lastest version's source
  
  ```sh
  $ wget https://www.python.org/ftp/python/3.7.4/Python-3.7.4.tgz
  ```
  Extract the source: `$ tar -xvf Python-3.7.4.tgz `
  <li><b>Install Prerequistes</b></li>
  
  ```sh
  $ sudo apt-get install gcc
  $ sudo apt install zlib1g-dev 
  $ sudo apt-get install libffi-dev libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev
  ```
  <li><b>Install</b></li>
  
  ```sh
  $ cd Python-3.7.4
  $ ./configure
  $ sudo make && make install
  $ python3.7 -V
  ```
  <li><b>Change From Current Version To Newest Version</b></li>

  ```sh
  $ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 1
  $ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 2
  $ sudo update-alternatives --config python3
  $ 2
  ```
  </br><b>Enjoy The Result!</b>
</ul>

<h3>2. Setup Virtual Programming Environment for Python3 </h3>
<ul>
  <li><b>Install Prerequistes</b></li>
  
  ```sh
  $ sudo apt-get install build-essential libssl-dev libffi-dev python-dev
  $ sudo apt-get update
  $ sudo pip3 install --upgrade pip 
  $ sudo apt install python3-pip
  $ sudo apt install -y python3-venv
  ```
  <li><b>Create Virtual Environment Thourgh Python3-venv</b></li>
  
  ```sh
  $ python3 -m venv [project_name]
  ```
  <li><b> Activate the Python Virtual Environment</b></li>
  
  ```sh
  $ source [project_name]/bin/activate
  ```
  <li><b>Exit Virtual Environment </b></li>
  
  ```sh
  $ deactivate
  ```
</ul>
<h3>3. Install Anaconda</h3>

```sh
$ wget https://repo.anaconda.com/archive/Anaconda3-2019.07-Linux-x86_64.sh
$ sha256sum Anaconda3-2019.03-Linux-x86_64.sh
$ bash Anaconda3-2019.03-Linux-x86_64.sh
$ conda create --name my_env python=3
$ conda activate my_env
```
<h3>4. Install Keras and Tensoflow</h3>

```sh
$ pip install tensorflow
$ pip install keras
```

```sh
$ pip show tensorflow
$ pip show keras 
```

<h3>5. Install Jupyter NoteBook</h3>

```sh
$ pip install jupyter notebook
$ jupyter notebook
```
Then open your web browser at: http://localhost:8888/








