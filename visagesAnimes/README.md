### visagesAnimes deployment on ngnix using ansible
------------
Deployer le projet visages animés avec ansible
![project](https://github.com/bakidjan/PL2_AI/blob/master/visagesAnimesjs/visagesAnimes.JPG)
------------
[install vagrant and up it for deploy hosts on virtualbox]
- vagrant up

- [first, modify /etc/ansible/hosts file to add the remote host @IP]
[web]
host1 ansible_host=192.168.201.11 ansible_user=vagrant ansible_password=vagarnt

- [requred tools on ansible host ]
sudo apt install ansible <br>
- [for copy the ssh-key to remote host]
sudo apt install sshpass <br>
- [generate ssh key and copy public key to remote host]
sudo ssh-keygen <br>
sudo ansible ssh-copy-id vagrant@192.168.201.11 <br>
- [ping to all to remote host]
ansible all -m ping

