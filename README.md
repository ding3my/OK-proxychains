# OK-proxychains
One key for proxychains
# Environment tested
```
4.5.5-300.fc24.x86_64
```
# Installation
```
sudo dnf install proxychains-ng -y
sudo sed -E 's|socks4 \t127.0.0.1 9050|socks5 \t127.0.0.1 1080|g' /etc/proxychains.conf -i
```
```
# testing after connecting ss server
proxychains4 curl ip.gs
```
# Problems known
Running `proxychains4 git clone` with ssh protocol
# Ref
google proxychains 配置
http://shawnelee88.github.io/2015/07/10/proxychains-shadowsocks%E7%A5%9E%E5%99%A8/
google proxychains git clone
https://www.52os.net/articles/proxychains-ng-redirect-tcp-to-proxy.html
proxychains4  -q /bin/bash
