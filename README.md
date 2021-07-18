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

#### My local versions of Ansible, python3, jinja:
```
ansible  --version                                                                                                                                                            INT х
ansible [core 2.11.2]
python version = 3.9.6 
jinja version = 3.0.1
```

