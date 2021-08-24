# pyenv-use

* 安装 pyenv

git clone https://github.com/zhangfeng1105/pyenv.git  ~/.pyenv

* 安装 pyenv-virtualenv

  >将放入.pyenv/plugins下 

git clone https://github.com/zhangfeng1105/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv


* 配置环境变量 
```javascript
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
if command -v pyenv 1>/dev/null 2>&1; then
 eval "$(pyenv init -)"
fi
eval "$(pyenv virtualenv-init -)"
```

* pyenv使用 
```javascript
安装：pyenv install 3.6.6
卸载：pyenv uninstall
查看被 pyenv 托管的 python 版本：pyenv versions
创建虚拟环境：pyenv virtualenv 3.6.6 my-env
删除虚拟环境：pyenv virtualenv-delete
激活虚拟环境:pyenv activate my-env
###如果你关掉了终端，那么下次启动你又得重新激活一次了
###解决：在项目文件目录下执行：pyenv local my-env
###在项目文件目录下，有个隐藏文件 .python-version，其中只写了一句话 my-env，进入项目文件目录，就会自动激活虚拟环境

pyenv global // 配置当前用户的系统使用的 python 版本. 可以使用这个命令进行python版本的切换!
pyenv rehash //刷新环境
pyenv shelll // 配置当前 shell 的 python 版本，退出 shell 则失效
pyenv local // 配置所在项目（目录）的 python 版本
```



