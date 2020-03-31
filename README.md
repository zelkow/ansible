# Ansible

# add repo
sudo apt-add-repository ppa:ansible/ansible

# update
sudo apt-get update


# install
apt-get install ansible -y


ssh-keygen -t rsa
ssh sdgo@artur-pc  mkdir -p .ssh
cat /home/sdgo/.ssh/id_rsa.pub|ssh sdgo@artur-pc  'cat >> .ssh/authorized_keys'

