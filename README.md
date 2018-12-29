# centos-vpn-starter

## Config.json

```json
{
    "server":"0.0.0.0",
    "server_port":8388,
    "local_port":1080,
    "password":"yourpassword",
    "timeout":600,
    "method":"aes-256-cfb"
}
```

## Install

```shell
yum install python-setuptools && easy_install pip
pip install shadowsocks
mkdir /etc/shdowsocks
cp config.json /etc/shdowsocks/config.json
nohup ssserver -c /etc/shadowsocks/config.json > /dev/null 2>&1 &
```
