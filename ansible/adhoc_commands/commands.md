# Ansible AD HOC Commands

### Shell module to check disk space

>  Shell is almost exactly like the command module but runs the command through a shell (/bin/sh) on the remote node.
```bash
ansible web -m shell -a "df -h"
```

### Command module to check server uptime

> The command(s) will not be processed through the shell, so variables like $HOME and operations like "<", ">", "|", ";" and "&" will not work. Use the shell module if you need these features.

```bash
ansible web -m command -a uptime
```

### Ansible gater_facts
> Ansible facts are data gathered about target nodes (host nodes to be configured) and returned back to controller nodes. Ansible facts are stored in JSON format and are used to make important decisions about tasks based on their statistics. Facts are in an ansible_facts variable, which is managed by Ansible Engine. Ansible facts play a major role in syncing with hosts in accordance with real-time data.

```bash
ansible all -m setup

Here, all means all hosts in the inventory/hosts file.

ansible localhost -m setup


```
