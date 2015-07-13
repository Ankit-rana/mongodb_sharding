# mongodb_sharding


#setup each system
vi /etc/yum.repos.d/mongodb-org-3.0.repo

[mongodb-org-3.0]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/3.0/x86_64/
gpgcheck=0
enabled=1

sudo yum install -y mongodb-org

yum install -y policycoreutils

semanage port -a -t mongod_port_t -p tcp 27017

