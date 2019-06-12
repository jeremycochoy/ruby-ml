# Machine learning in ruby

## Jupyter lab

### Install jupyter lab
First, instal jupyter lab to run ruby notebooks.

To do so, download and install anaconda from [https://www.anaconda.com/distribution/].
You may have to set your path in your `~/.bashrc` or `~/.zshrc` with
```bash
export PATH=$PATH":"$HOME/anaconda3/bin/
```

Type `conda` in a terminal to know if the install is completed.

To work on a project, open a directory in a terminal and `jupyter notebook` (or `jupyter lab` if you need a more powerfull interface).

### Install ruby kernel

Jupyter lab was developped to run python script through a python kernel (i.e. a binary runing python code).
You have to install and configure a ruby binary. On mac, type :
```
brew install automake gmp libtool wget
brew install zeromq --HEAD
brew install czmq --HEAD

set -x LIBZMQ_PATH (brew --prefix zeromq)/lib
set -x LIBCZMQ_PATH (brew --prefix czmq)/lib

gem install cztop
gem install iruby --pre
iruby register --force
```
