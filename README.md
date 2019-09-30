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
  Change director:  `cd Python-3.7.4 `
  </br>Now run the following command to run the configuration script:  `./configure `
  </br>Now is the time to install Python:  `make ` or `sudo apt-get make `
  </br>Also, run the following command for Python installation:  `sudo make install `
  </br>Check if successful:   `python3.7 -V `
  <li><b>Change From Current Version To Newest Version</b></li>
  If you check by: `python3 -V `
  </br>The result still be a 3.6 python version. So we need to upgarde it to the version we just installed.
  </br>Add python's alternatives (current version(mine was 3.6.8) and newest version (3.7.4))
  
  ```sh
  sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 1
  sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 2
  ```
  Then chose <i>"2"</i>.
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
