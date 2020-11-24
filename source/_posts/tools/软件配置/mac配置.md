### 1. 安装 Homebrew & Git
```bash
/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
```
### 2. 研发环境配置
#### 2.1 Golang环境配置

```bash
# 下载 golang1.15.2.darwin-amd64.tar.gz
vim ~/.bash_profile
    export GOROOT=/usr/local/go
    export PATH=$GOROOT/bin:$PATH
    
go version
```

#### 2.2 安装 Anaconda及[升级](https://www.jianshu.com/p/8f97c4a77367)

```bash
# 1. 下载 Anaconda-2020.02.sh
bash ～/Download/Anaconda-2020.02.sh

# 2. 配置环境变量
vim ~/.bash_profile
# Anaconda
export ANACONDA_HOME=/Users/liangchao/anaconda3/bin
export PATH=$ANACONDA_HOME:$PATH:

# 3. 安装 TensorFlow
pip install tensorflow

# 4. 升级Anaconda，要先升级conda
conda update conda

# 5. 升级Anaconda
conda update Anaconda

# 6. 升级python
conda update python

# 7. 查看安装的库
pip list       #查看库
conda list     #查看库及版本

# 8. 安装/更新单个库（scipy）
pip install scipy
pip install scipy --upgrade

conda install scipy
conda update scipy

# 9. 安装/更新所有库
conda update --all
```

#### 2.3 安装Julia

```shell
# 1. 下载 julia-1.5.2-mac64.dmg，点击安装，拖入Application目录
# 2. 创建命令软连接
ln -s /Applications/Julia-1.5.app/Contents/Resources/julia/bin/julia  /usr/local/bin/julia
# 3. 新打开一个终端，输入 julia 即可
# 4. 卸载：删除Julia.app，并删除包目录 ~/.julia
```



