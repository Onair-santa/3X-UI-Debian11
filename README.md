## <a href="#"><img src="https://github.com/vpnhood/VpnHood/wiki/images/logo-linux.png" width="32" height="32"></a>(Debian11, Ubuntu20) 3X-UI Debian11
### 3X-UI - Xray panel supporting multi-protocol multi-user expire day & traffic & IP limit (Vmess & Vless & Trojan & ShadowSocks & Wireguard)

#### 💠  Ensure that the `sudo` and `wget` packages are installed on your system:

```
apt install -y sudo wget
```

#### 💠 Root Access is Required. If the user is not root, first run:

```
sudo -i
```

#### 💠 Then:

```
wget https://github.com/Onair-santa/3X-UI-Debian11/releases/download/2.4.1/x-ui-linux-amd64.tar.gz
cd /root/
rm -rf x-ui/ /usr/local/x-ui/ /usr/bin/x-ui
tar zxvf x-ui-linux-amd64.tar.gz
chmod +x x-ui/x-ui x-ui/bin/xray-linux-* x-ui/x-ui.sh
cp x-ui/x-ui.sh /usr/bin/x-ui
cp -f x-ui/x-ui.service /etc/systemd/system/
mv x-ui/ /usr/local/
systemctl daemon-reload
systemctl enable x-ui
systemctl restart x-ui
```
URL
- `http://ip:port/`
