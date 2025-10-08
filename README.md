# API Hacking Tools & Tutorials

## Postman Installation
- ```snap install postman ```

- 1. ```Download postman zip package ```
- 2. ```https://www.postman.com/downloads/ ```

- 3. Extract and Move to /Opt Folder
``` bash
cd ~/Downloads

tar -xzf Postman-linux-x64*.tar.gz

sudo mv Postman /opt/Postman
```

- 4. Create Link to local folder
```bash
sudo ln -sf /opt/Postman/Postman /usr/local/bin/postman


 ```
 - 5. Run postman using Terminal
 ```bash
postman
 ```

 ---
 ## Mitmproxy2swagger Installation

 ```bash

└─$ cd /opt
└─$ sudo pip3 install mitmproxy2swagger
```