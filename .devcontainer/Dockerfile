FROM mcr.microsoft.com/vscode/devcontainers/base:0-buster

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
     && apt-get -y install --no-install-recommends python3 python3-pip python3-setuptools ipython3
RUN python3 -m pip install --upgrade pip
RUN pip3 install virtualenv eth-brownie pytest black

RUN apt-get install curl



RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash \
     && . /root/.nvm/nvm.sh \
     && nvm install node \
     && nvm alias default node \
     && nvm use default \
     && npm install -g ganache
 
 
