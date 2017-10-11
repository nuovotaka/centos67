Setup local development environment.  Installs Apache, PHP, MySQL, Ruby and Node.js.  See main.yml for more details.

```
mkdir mycentos && cd mycentos
vagrant init bento/centos-6.7
vi Vagrantfile # IP編集
vagrant up
vagrant ssh
sudo yum -y install git
git clone https://github.com/nuovotaka/centos67.git
cd centos67
./run.sh
exec $SHELL -l
```

If you need to update the script, please follow the instruction below.

```
cd
git clone https://github.com/nuovotaka/centos67.git
cd centos67
./run.sh
```

Attention
Apache Only IP address
localhost, 127,0,0,1 , 192,168,xxx,xxx
