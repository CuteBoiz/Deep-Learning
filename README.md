# Deep-Learning With Keras And TensorFlow
<h2>I.Install Environment For Deep Learning </h2>
<h3>1. Install Python</h3>
<ul>
  <li><b>Get Lastest Python Version </b></li>
  Go to: https://www.python.org/downloads/source/ to get the lastest version's source
  
  ```sh
  wget https://www.python.org/ftp/python/3.7.4/Python-3.7.4.tgz
  ```
  Extract the source: `tar -xvf Python-3.7.4.tgz `
  <li><b>Install Prerequiste</b></li>
  
  ```sh
  sudo apt-get install gcc
  sudo apt install zlib1g-dev 
  sudo apt-get install libffi-dev
  ```
  <li><b>Install</b></li>
  
  ```sh
  cd Python-3.7.4
  ./configure
  make 
  sudo make install
  python3.7 -V
  ```
  <li><b>Change From Current Version To Newest Version</b></li>

  ```sh
  sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 1
  sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 2
  2
  ```
  
  </br><b>Enjoy The Result!</b>
</ul>

<h3>2.Install Virtualenv </h3>
<ul>
  <li><b>Install </b></li>
  
  `pip install virtualenv` 
  
  `sudo /usr/bin/easy_install virtualenv`
  <li><b>Create Virtual Environment </b></li>
  
`virtualenv -p /usr/bin/python3 [project_name]`
  <li><b>Active Virtual Environment </b></li>
  
`source [project_name]/bin/activate`
  <li><b>Exit Virtual Environment </b></li>
  
`deactivate`
</ul>
<h3>b.Install Keras and Tensoflow</h3>
