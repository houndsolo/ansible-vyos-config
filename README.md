ansible config for my home network

```
ansible-playbook -i hosts.yml --vault-password-file=vyos-vault.pw playbook.yml -lvyos-ss-backup-bash -e node=ss-backup
```
