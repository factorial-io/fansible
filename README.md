## Ansible playbook to install factorials magic haproxy docker container.

### Remote machine
1. Add your ssh key for SSH key based authentication on the remote machines.
2. Make sure python 2.5+ is installed.

### Control machine
0. Clone this repo and initialize submodules.
1. Install pip:  
```sudo easy_install pip```
2. Install ansible
``` sudo pip install ansible ```
3. Edit the inventory.ini and add your server IP’s.
4. Add your ssh key for key authentication on the remote machines and test connection:
```ansible all --inventory-file=inventory.ini --module-name ping -u rhizom```
5. Run the playbook.
```ansible-playbook playbook.yml -i inventory.ini -u YOUR_USER --ask-sudo-pass```
