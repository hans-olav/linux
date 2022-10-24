# Linux Common Stuff

Github auth
```
curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo dd of=/usr/share/keyrings/githubcli-archive-keyring.gpg
sudo chmod go+r /usr/share/keyrings/githubcli-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null
sudo apt update
sudo apt install -y gh
gh auth login
```

Get git repo and link up
```
git config --global user.email hansolav@hansolav.net
git config --global user.name "Hans Olav Norheim"

sudo apt install -y tmux sysstat gawk net-tools coreutils
git clone https://github.com/hans-olav/linux
ln -s linux/.tmux.conf
ln -s linux/.nanorc
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
tmux
```
