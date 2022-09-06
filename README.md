# Install

Prerequisites:

- ansible
- git
- git config --global user.email "alice@example.com"
- git config --global user.name "Alice Foo"
- ssh-keygen -t ed25519 -C "alice@example.com"
- add public key on Github

Clone repo then run:

```
$ ansible-playbook -K local.yaml --tags dev
```

Available tags:

- dev
- i3

# Supported systems

- Fedora 36
