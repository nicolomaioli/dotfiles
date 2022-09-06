# Dotfiles

Bootstrap a workstation using Ansible.

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
