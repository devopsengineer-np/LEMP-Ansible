[ansible](https://github.com/devopsengineer-np/LEMP-Ansible)

ansible-playbook lemp.yml
ansible-playbook -i inventory lemp.yml
#add these as default
/etc/ansible/ansible.cfg
[defaults]
inventory = /etc/ansible/hosts
remote_user = ec2-user
private_key_file = ~/.ssh/id_rsa
ansible_python_interpreter= /usr/bin/python3

/etc/anisble/hosts
[node1] #name group for server
x.x.x.x #IP
[node2]
x.x.x.x
