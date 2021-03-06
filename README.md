
# There will be some info about this repo


Short introdiution (make sure you make all of these points)
1) Make sure you config your host file (/etc/ansible/hosts) properly
2) Add ssh keys to machines wou wanna work on
3) Run the ping module to make sure you have correctly configured the hosts (ansible all -m ping)
4) Before you run your playbook remember to check them with param --check for example (ansible-playbook /path_to_file/file.yaml --check)


---
## Usefull commands



1) If u want to use ansible.posix module execute this command:
```
ansible-galaxy collection install ansible.posix
```

2) Install collection localy for database - mariadb
```
ansible-galaxy collection install community.mysql
```

3) Shutdown all hosts (only for lab)
```
ansible all -m shell -a "shutdown -h now"
```

4) If u want use ansible packages just install this collection (I use it in alpine repo)
```
ansible-galaxy collection install community.general
```

---
## Git aliases 
To define a Git alias, use the ```git config``` command with the alias and the command you want to substitute.
For example, to create the alias p for push:
```
git config --global alias.p 'push'
```
So now you can easily use the abbreviated version of this command
```
git p 
```
To see all your aliases, list your configuration with ```git``` config:
```
git config --global -l
```

The gl alias makes it easier to list all user configurations:
```
 git config --global alias.gl 'config --global -l'
```
> https://opensource.com/article/20/11/git-aliases