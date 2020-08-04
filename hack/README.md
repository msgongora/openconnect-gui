# Using openconnect-gui from brew
```
brew cask install openconnect-gui
sudo mkdir -p /etc/vpnc/connect.d/
curl -s https://raw.githubusercontent.com/msgongora/openconnect-gui/mrsg/hack/add-routes |\
    sudo tee /etc/vpnc/connect.d/add-routes
sudo chmod +x /etc/vpnc/connect.d/add-routes
# update add-routes file
```

# Using release package
1. Copy OpenConnect-GUI.app to /Applications/
2. Copy custom `vpnc-script` to the location needed by the built-in script (OpenConnect-GUI.app/Contents/Resources/vpnc-script)
```
sudo cp -r etc/vpnc /etc
```
3. Add the destination ip you want to route through VPN: variable `extra_addrs`
```
sudo vim /etc/vpnc/connect.d/add-routes

```
