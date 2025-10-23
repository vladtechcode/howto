# How to setup Git and Github 


### Set your identity (use the email associated with your GitHub account):
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

### Set default branch name to 'main'
git config --global init.defaultBranch main

### Enable colored output
git config --global color.ui auto
Ss
### Generate SSH key
ssh-keygen -t ed25519 -C "your.email@example.com"

### Start SSH agent and add key
eval "$(ssh-agent -s)"
ssh-add --apple-use-keychain ~/.ssh/id_ed25519

### Copy your public key
pbcopy < ~/.ssh/id_ed25519.pub

### Add to gihub SSH

### Test connection
ssh -T git@github.com

### You need to installed GitHub CLI

# Authenticate with Github
gh auth login

# Select GitHub.com
# Select SSH 
# Upload your SSH public key
# Select title for SSH key. Example: mypc
# Proceed with authentication

# Checks authorization status on Github
gh auth status



