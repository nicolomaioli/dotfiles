# dotfiles

Bootstrap a workstation using Ansible. Individual configurations are stored in
the following repos:

- [nicolomaioli/nvim](https://github.com/nicolomaioli/nvim)
- [nicolomaioli/tmux](https://github.com/nicolomaioli/tmux)
- [nicolomaioli/alacritty](https://github.com/nicolomaioli/alacritty)
- [nicolomaioli/i3](https://github.com/nicolomaioli/i3)

Prerequisites:

- ansible
- curl
- git:
  - git config --global user.email "alice@example.com"
  - git config --global user.name "Alice"
  - ssh-keygen -t ed25519 -C "alice@example.com"
  - add public key on Github

Clone this repo then run:

```
$ ansible-playbook -K local.yaml --tags dev
```

Available tags:

- dev
- i3

# Supported systems

- Fedora 36
