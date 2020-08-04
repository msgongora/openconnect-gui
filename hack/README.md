
1. Copy OpenConnect-GUI.app to /Applications/
2. Copy custom `vpnc-script` to the location needed by the built-in script (OpenConnect-GUI.app/Contents/Resources/vpnc-script)
```
sudo cp -r etc/vpnc /etc
```
3. Add the destination ip you want to route through VPN: variable `extra_addrs`
```
sudo vim /etc/vpnc/connect.d/add-routes

```
