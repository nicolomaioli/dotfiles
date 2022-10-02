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
- git

Clone this repo then run:

```sh
$ ansible-playbook -K local.yml --tags dev
```

Available tags:

- dev
- i3
- sway

## Git Protocol

Note that repos are cloned using ssh by default, so you need to configure git
and add an ssh key to Github. You can change this behaviour by setting the
`git.protocol` variable, i.e.:

```sh
$ ansible-playbook -K local.yml --tags dev --extra-vars '{"git": {"protocol":
"https"}}'
```

# Supported systems

- Fedora 36
