\#\# Upgrade from 6.x to 7.x

\#\#\# Mongo DB

The steps needed to install MongoDB are:

- Download the archive for your operating system

- Untar/uncompress files and move them to their definitive location

- Edit the configuration file

- Start the database

\#\#\#\# Useful commands

Create a dump of the old database

cd /

chown -R devopsroot:devopsroot opt

sudo chown -R devopsroot:devopsroot opt

cd opt/

mkdir install

cd install/

curl -O https://fastdl.mongodb.org/linux/mongodb-linux-x86\_64-rhel70-3.4.14.tgz

tar -xvzf mongodb-linux-x86\_64-rhel70-3.4.14.tgz 

chown -R devopsroot:devopsroot opt

sudo chown -R devopsroot:devopsroot opt

mkdir mongo

cd mongo/

ls

cp -Rf ../install/mongodb-linux-x86\_64-rhel70-3.4.14/\* .

mkdir data

ls

pwd

ls

cd data/

tar -xzvf mrhe-10-april.tar.gz 

mkdir mrhe

mkdir dump

mv -f ../opt/clarive/clarive/dump/\* .

vi .bash\_profile 

export MONGO\_DB=/opt/mongo

export PATH="$MONGO\_DB:$PATH"

mongod -version

vi mongod.conf

mongorestore -d mrhe /opt/mongo/data/dump/mrhe

mongod -f /opt/mongo/config/mongod.conf 

ps aux \| grep mongo

cd /usr/lib/systemd/system/

sudo touch mongod.service

sudo vi mongod.service 

sudo systemctl enable mongod.service

ps aux \| grep mongo

sudo kill -9 69599

sudo systemctl start mongod

mongo --host 10.100.90.6

systemctl status mongod.service 

systemctl stop mongod.service 

sudo systemctl stop mongod.service 

sudo systemctl start mongod.service 

sudo systemctl status mongod

