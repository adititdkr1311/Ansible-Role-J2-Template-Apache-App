# Ansible-Role-J2-Template-Apache-App

 Steps

# Default ansible installation path  
cd /etc/ansible
ls
ansible.cfg hosts roles

# Change path to home
cd /home/ansiuser
mkdir roles
cd roles

# Create role apache
ansible-galaxy init apache

# Install package tree
sudo apt-get install tree -y
ls

# On host node we will update below config files using j2 template
cd /etc/apache2
ls
 - ports.conf  ### we will update port number using j2 template

cd /etc/apache2/sites-enabled
ls
 - 000-default.cong  ### we will update port number and default html path (/var/www/html) using j2 template



=====================================================
# Execute the role

ansible-playbook playbook-roles.yml
