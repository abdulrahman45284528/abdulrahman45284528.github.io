---
layout: default
title: Communication System
---

# SSH: Secure Shell or Secure Socket Shell
- Encrypted connection between two hosts over the internet
- SSH key pair: 
1. Public Key : id_<algorithm>.pub  eg. id_rsa.pub
2. Private Key: id_<algorithm>

Q. How to generate an SSH Key pair?
- Use any one algorithm below: 
```
$ ssh-keygen -t rsa -b 4096
$ ssh-keygen -t ecdsa -b 521
$ ssh-keygen -t ed25519
```
- Select the default location and filename. (or, you can choose your own) : eg. .ssh/id_rsa.pub
- You are then prompted to enter a passphrase. (Choose a strong one) (Dont want a passphrase? => Just press ENTER)
- Now, copy the public key to the server! Thats it!

- Note: 1. If you change the default name of the key pair, then you have to explicitly specify that this key should be used for connecting to a specific host.
        $ ssh -i ~/<path-to-keys>/<keyname> username@servername
       2. For frequent users, you can configure ssh.
        $ ~/.ssh/config
       3. If error, debug using:
        $ ssh -v
