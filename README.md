# Linux Common Stuff

Get git repo and link up
```
sudo apt install -y tmux sysstat gawk net-tools coreutils stow
git clone https://github.com/hans-olav/linux
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
cd linux && stow -v . && cd ~

tmux
```
prefix + I to install plugins


tailscale
```
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up --ssh
```
Remember: Disable key expiry.
