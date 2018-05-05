# Deploy Kubernetes with Ansible

---
## How to use this

### Clone this repository
```
git clone git@github.com:ChoiSD/k8s-playbook.git
cd k8s-playbook
```

### Edit configuration files
```
cd config
```
  * config.yaml - all setting parameters are in this file
  * hosts - definition for the nodes in k8s cluster
  * ssh_key - SSH private key that is used to communicate with other nodes (you can use ansible_ssh_pass instead of this)

### Run playbook
```
cd ..
ansible-playbook -e @config/config.yaml site.yaml
```
