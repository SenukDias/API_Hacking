# API Hacking Tools & Tutorials

## Postman Installation
### Option A: Install via Snap (simplest)
```bash
sudo snap install postman
```

### Option B: Manual install (tar.gz) and terminal access
1. Download Postman for Linux (tar.gz): `https://www.postman.com/downloads/`
2. Extract and move to `/opt`:
```bash
cd ~/Downloads
tar -xzf Postman-linux-x64*.tar.gz
sudo mv Postman /opt/Postman
```
3. Add a symlink so `postman` works in the terminal:
```bash
sudo ln -sf /opt/Postman/Postman /usr/local/bin/postman
```
4. Run Postman:
```bash
postman
```

Optional: Add a desktop launcher (shows in app menu)
```bash
cat <<'EOF' | sudo tee /usr/share/applications/postman.desktop >/dev/null
[Desktop Entry]
Name=Postman
GenericName=API Client
Comment=Postman API Platform
Exec=/usr/local/bin/postman %U
Icon=/opt/Postman/app/resources/app/assets/icon.png
Terminal=false
Type=Application
Categories=Development;Utility;Network;
EOF
```

Update Postman later (manual install):
```bash
cd ~/Downloads
tar -xzf Postman-linux-x64*.tar.gz
sudo rm -rf /opt/Postman
sudo mv Postman /opt/Postman
```

 ---
 ## Mitmproxy2swagger Installation

 ```bash
cd /opt
sudo pip3 install mitmproxy2swagger
```

