---
layout: default
title: Connect github in WSL
---

To connect GitHub with the Windows Subsystem for Linux (WSL), you can follow these general steps. 
This assumes that you have WSL installed on your Windows machine.

### Install Git on WSL:
````
sudo apt install git
````

### Generate SSH Key:
````
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
````
Follow this:
````
~$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/home/codebind/.ssh/id_rsa): (Enter for default location ./ssh/id_rsa)
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in id_rsa
Your public key has been saved in id_rsa.pub
````
  Note: .ssh/id_rsa folder should have id_rsa.pub, else copy and paste here.

### Add SSH Key to SSH Agent:

  Start the SSH agent: 
````
eval "$(ssh-agent -s)"
````
  Add your private key to the SSH agent: 
````
ssh-add ~/.ssh/id_rsa
````

### Copy SSH Key to GitHub:

  Display your public key: 
````
cat ~/.ssh/id_rsa.pub
````
  Copy the output.
  Go to your GitHub account settings, navigate to "SSH and GPG keys," and add a new SSH key. Paste the copied key into the key field.

### Test SSH Connection:

  Test your SSH connection to GitHub: 
````
ssh -T git@github.com
````
  You should see a message indicating successful authentication.

### Configure Git with Your Identity:

  Configure Git with your GitHub username and email:
````
git config --global user.name "Your GitHub Username"
git config --global user.email "your_email@example.com"
````

### Clone a Repository:
````
git clone git@github.com:username/repository.git
````

  Replace username with your GitHub username and repository with the name of the repository you want to clone.


Now, your WSL environment should be configured to work with GitHub using SSH. You can use Git commands in the WSL terminal to interact with GitHub repositories seamlessly.

- FAQ:
Remember that you only need to perform these steps once, and subsequent Git commands in WSL should use the configured SSH key for authentication. 
If you encounter any issues, double-check the SSH key setup and make sure you've added the correct key to your GitHub account.
