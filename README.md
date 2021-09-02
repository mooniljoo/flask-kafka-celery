### Tutorial for setting up a basic Flask REST APIs only application

#### Install dependencies
```
$ virtualenv .pyenv
$ source .pyenv/bin/activate
$ pip install -r requirements/base.txt
```

#### Run

```
$ python run.py
* Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
* Restarting with stat
```

Now hit `http://localhost:5000/v1/api/users` in your browser
Now hit `http://localhost:5000/v1/api/customers` in your browser

# 필요한 패키지 설치
```
yum update
yum install yum-utils
yum groupinstall development
yum install zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel openssl-devel xz xz-devel libffi-devel findutils
```

# pyenv 설치
```
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bash_profile
```
source ~/.bash_profile

# pyenv virtualenv 설치
```
git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bash_profile
source ~/.bash_profile
```

# 가상환경 만들기
```
pyenv install 3.6.4
pyenv virtualenv 3.6.4 celery
pyenv activate celery
```
