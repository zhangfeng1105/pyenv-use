# pyenv-use

* 安装 pyenv

git clone https://github.com/zhangfeng1105/pyenv.git  ~/.pyenv

* 安装 pyenv-virtualenv

*将放入.pyenv/plugins下 *

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
