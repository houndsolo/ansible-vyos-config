ansible config for my home network

```
for i in ss lm ar ; do
for j in main backup ; do
ansible-playbook -i hosts.yml --vault-password-file=vyos-vault.pw playbook.yml -e node=${i}_${j}
done
done

```
