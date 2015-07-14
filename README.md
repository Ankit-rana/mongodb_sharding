# mongodb_sharding


#setup each system
vi /etc/yum.repos.d/mongodb-org-3.0.repo

[mongodb-org-3.0]<br>
name=MongoDB Repository<br>
baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/3.0/x86_64/<br>
gpgcheck=0<br>
enabled=1<br>

sudo yum install -y mongodb-org

yum install -y policycoreutils-python

semanage port -a -t mongod_port_t -p tcp 27017

