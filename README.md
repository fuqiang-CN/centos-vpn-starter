# centos-vpn-starter

## Install

```shell
yum install python-setuptools && easy_install pip
pip install shadowsocks
mkdir /etc/shdowsocks
cp config.json /etc/shdowsocks/config.json
nohup ssserver -c /etc/shadowsocks/config.json > /dev/null 2>&1 &
```
