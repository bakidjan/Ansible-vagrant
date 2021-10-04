### visagesAnimes deployment on ngnix using ansible
------------
Deployer le projet visages animés avec ansible
![project](https://github.com/bakidjan/PL2_AI/blob/master/visagesAnimesjs/visagesAnimes.JPG)
------------
[install vagrant and up it for deploy hosts on virtualbox]<br>
vagrant up

- [first, modify /etc/ansible/hosts file to add the remote host @IP]<br>
[web]<br>
host1 ansible_host=192.168.201.11 ansible_user=vagrant ansible_password=vagarnt

- [requred tools on ansible host ]<br>
```
sudo apt install ansible 
```
sudo apt install ansible 
```
[for copy the ssh-key to remote host]<br> 
```
```
```
```
sudo apt install sshpass
```
- [generate ssh key and copy public key to remote host]<br>
```
sudo ssh-keygen
```
```
sudo ansible ssh-copy-id vagrant@192.168.201.11 <br>
```

- [ping to all to remote host]<br>
```
ansible all -m ping
```
- [apply ansible playbook]<br>
```
ansible-playbook visagesAnimesNginx.yml
```

