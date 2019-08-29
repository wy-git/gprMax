# Install conda
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh -b -p $HOME/miniconda
echo "export PATH="$HOME/miniconda/bin:$PATH" && source $HOME/miniconda/bin/activate" >> $HOME/.bashrc
. .bashrc
```

# If server in China
```
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --set show_channel_urls yes
```

# Install gprMax
```
conda env create -f conda_env.yml
conda activate gprMax
python setup.py build
python setup.py install
```

# If have gpu
```
pip install pycuda
```
