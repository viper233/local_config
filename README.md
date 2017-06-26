A playbook collection to help configure my local desktop system

To run

```
ansible-galaxy install -r requirements.yml -p roles
ansible-playbook desktop.yml -K -i hosts -c local --sudo
```
