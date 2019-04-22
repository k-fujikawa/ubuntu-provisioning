# Ubuntu provisioning

## Install Ansible

```
sudo apt-get update -y && apt-get install -y software-properties-common
sudo apt-add-repository -y ppa:ansible/ansible
sudo apt-get update -y && apt-get install -y ansible
```

## Clone this repository

```
mkdir -p $HOME/git/github.com/k-fujikawa
git clone git@github.com:k-fujikawa/ubuntu-provisioning.git $HOME/git/github.com/k-fujikawa/ubuntu-provisioning
cd $HOME/git/github.com/k-fujikawa/ubuntu-provisioning
```

## Run Ansible playbooks

```
ansible-galaxy install -r requirements.yml
sudo ansible-playbook site.yml
```
