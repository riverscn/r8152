FROM ubuntu:bionic
LABEL Name=r8152 Version=0.0.1
# RUN sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list && \
# sed -i 's/security.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list && \
apt-get update && \
apt-get install -y git \
cifs-utils \
python \
python-pip \
python3 \
python3-pip
RUN mkdir -p /toolkit && \
cd /toolkit && \
git clone https://github.com/SynologyOpenSource/pkgscripts-ng
# cd /toolkit/pkgscripts-ng/ && \
# git checkout DSM7.0 && \
# ./EnvDeploy -v 7.0 -p avoton # for DSM7.0
## CMD ["sh", "-c", "/usr/games/fortune -a | cowsay"]
