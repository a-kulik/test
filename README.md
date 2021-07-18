### How to spin up Jenkins Master: 

#### All files for one click deployment are stored in Jenkins-Master folder, this folder contains of:
 - `template` folder with jinja templates.
 - `vars` folder with the file `vars.yml` where you can configure some Jenkins parameters.
 - `inventory` with IP of target instance.
 - `jenkins-playbook.yml` playbook to build and deploy Jenkins docker image.
 - `target_key` ssh key to connect to target host
 - `ansible.cfg` configuration file for Ansible

#### Command to run playbook:
`ansible-playbook jenkins-playbook.yml -i ./inventory`

> ansible  --version                                                                                                                                                            INT х
ansible [core 2.11.2]
config file = /Users/kulik/Downloads/anton/Jenkins-Master/ansible.cfg
configured module search path = ['/Users/kulik/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
ansible python module location = /usr/local/lib/python3.9/site-packages/ansible
ansible collection location = /Users/kulik/.ansible/collections:/usr/share/ansible/collections
executable location = /usr/local/bin/ansible
python version = 3.9.6 (default, Jun 29 2021, 05:25:02) [Clang 12.0.5 (clang-1205.0.22.9)]
jinja version = 3.0.1
> libyaml = True
