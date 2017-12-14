# Bitzeny Miner Infrastructure

Automatic build Bitzeny miner machines by Ansible.

## Getting Started

### Preparing

- Prepare your machines with SSH connection (by root) settings.
  - Exchange your private keys with new machines.
  - Delete root password. (`passwd -d root`)

### Setup

```
$ cd /path/to/respository
$ /bin/sh setup.sh
```

- Edit `infrastructure/playbook/machines` with your machine connection settings.
- Edit `infrastructure/playbook/vars_files/common.yml` with fill your SSH public key.
  - The playbook create `miner` user with authorized key above. 

```
$ ansible-playbook -i machines miner.yml
```

### Start mining

Sorry. Mining is currently manual operation.

- Manualy login. and start tmux and start mining with `~/cpuminer/minerd`
  - Login user: `miner@YOUR-HOSTNAME`

## Donate

ZNY: `ZjreyuNjZnKLZM173tQ3DxiYb9ZJUEHUAV`
MONA: `MHYeVeMTjLeauhtvSETyBwZCFcVjzeHrNd`
