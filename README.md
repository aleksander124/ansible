---
There will be some info about this repo
---

Short introdiution (make sure you make all of these points)
1) Make sure you config your host file (/etc/ansible/hosts) properly
2) Add ssh keys to machines wou wanna work on
3) Run the ping module to make sure you have correctly configured the hosts (ansible all -m ping)
4) Before you run your playbook remember to check them with param --check for example (ansible-playbook /path_to_file/file.yaml --check)


---
Usefull commands

1) If u want to use ansible.posix module execute this command:
ansible-galaxy collection install ansible.posix

