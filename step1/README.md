# Deploy MongoDB 

Here, we will assume a deployment of the OSS version of MongoDB on Ubuntu. 
After connection to your VM, follow the instruction below to install MongoDB.

* Import the public key used by the package management system.

```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
```

* Create a list file for MongoDB

```
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.6 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.6.list
```

* Reload local package database.

```
sudo apt-get update
```


* Install the MongoDB packages

```
sudo apt-get install -y mongodb-org=3.6.7 mongodb-org-server=3.6.7 mongodb-org-shell=3.6.7 mongodb-org-mongos=3.6.7 mongodb-org-tools=3.6.7
```

* Start MongoDB

```
sudo service mongod start
```


* Verify that MongoDB has started successfully

Verify that the mongod process has started successfully by checking the contents of the log file at /var/log/mongodb/mongod.log for a line reading

```
[initandlisten] waiting for connections on port 27017
```

The complete instruction can be found [HERE](https://docs.mongodb.com/v3.6/tutorial/install-mongodb-on-ubuntu/)

* Load the sample data

From inside the VM, run the following command:

```
mongoimport   
```

For other plaform, please see installation instruction [here](https://docs.mongodb.com/v3.6/administration/install-community/) 
