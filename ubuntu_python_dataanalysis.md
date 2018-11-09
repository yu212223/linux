echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial main restricted" > /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial-updates main restricted" >> /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial universe" >> /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial-updates universe" >> /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial multiverse" >> /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial-updates multiverse" >> /etc/apt/sources.list
echo "deb http://mirrors.ustc.edu.cn/ubuntu/ xenial-backports main restricted universe multiverse" >> /etc/apt/sources.list
echo "deb http://security.ubuntu.com/ubuntu/ xenial-security main restricted" >> /etc/apt/sources.list
echo "deb http://security.ubuntu.com/ubuntu/ xenial-security universe" >> /etc/apt/sources.list
echo "deb http://security.ubuntu.com/ubuntu/ xenial-security multiverse" >> /etc/apt/sources.list

apt-get update
apt-get -y upgrade
apt-get install -y vim wget net-tools iputils-ping


apt autoremove python3