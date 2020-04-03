# Config from https://linuxhint.com/ansible-tutorial-beginners/
# Ansible

# add repo
sudo apt-add-repository ppa:ansible/ansible

# update
sudo apt-get update


# install
apt-get install ansible -y


# ssh password less
ssh-keygen -t rsa

ssh sdgo@artur-pc  mkdir -p .ssh
cat /home/sdgo/.ssh/id_rsa.pub|ssh sdgo@artur-pc  'cat >> .ssh/authorized_keys'


ssh sdgo@aleks-pc  mkdir -p .ssh
cat /home/sdgo/.ssh/id_rsa.pub|ssh sdgo@aleks-pc  'cat >> .ssh/authorized_keys'

ansible-playbook playbooks/python.yml --ask-become-pass
