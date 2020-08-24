# Deep-Learning With MXNET

## Contents

## Installation

### 1. [Miniconda](https://conda.io/en/latest/miniconda.html)

```sh
sh Miniconda3-latest-Linux-x86_64.sh -b
~/miniconda3/bin/conda init
```
`conda create --name d2l -y`

### 2. Notebook of D2l

```sh
mkdir d2l-en && cd d2l-en
curl https://d2l.ai/d2l-en.zip -o d2l-en.zip
unzip d2l-en.zip && rm d2l-en.zip
conda activate d2l
```

### 3. Framework & D2l Lib

```sh
pip install mxnet-cu101==1.6.0
pip install -U d2l
```
