# Quick start

- Setup new emtpy vagrant box
- Install ansible both in host machine and managed hosts:
  - host: homebrew/pip
  - managed node: pip
  
- Setup SSH access so that you can:
  - `ssh vagrant@hostname -i private_key`
  - `ssh vagrant@hostname` - via SSH config file
  
- Setup ansible inventory file ([inventory](inventory))
  - be explicit about ssh connection/user and key to use

# Hello world

```bash
$ ansible -vvvv -i inventory all -m ping
```
