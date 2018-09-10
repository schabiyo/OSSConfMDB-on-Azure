# MongoDB Atlas on Azure 

The intend of this repository is to demonstrate the followin:


Step 1: Deploy MongoDB 

Step 2: Create a Cluster on Azure using MongoDB Atlas

Step 3: Migrate the data to Atlas


The full workflow looks like this:

![Overview](/imgs/overview.png "Overview")


## Pre-requisite

- Ubuntu VM
- MongoDB Atlas account 


## Deploy MongoDB 

Here, we will assume a deployment of the OSS version of MongoDB on Ubuntu. 
After connection to your VM, follow the instruction below to install MongoDB.

* link:step1/README.adoc[deploy MongoDB]



* Import the public key used by the package management system.


* Create a list file for MongoDB


* Reload local package database.


* Install the MongoDB packages


* Start MongoDB


* Verify that MongoDB has started successfully


The complete instruction can be found [HERE](https://docs.mongodb.com/v3.6/tutorial/install-mongodb-on-ubuntu/)


For other plaform, please see installation instruction [here](https://docs.mongodb.com/v3.6/administration/install-community/) 
