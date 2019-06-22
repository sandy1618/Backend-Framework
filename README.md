[![Build Status](https://travis-ci.com/pingman-io/Backend-Framework.svg?branch=master)](https://travis-ci.com/pingman-io/Backend-Framework)

### Demo Site :

Heroku Hosted Demo Application. ```Link down. Site under construction.```

[Pingman.io](https://pingmanio.herokuapp.com/)

Site will be ready by 20.12.2020.

### Pingman Application

A cryptocurrency ```ticker``` cum ```ping``` application built on a ```Node.js``` backend.

### Install. 

Make sure you have ```Node.js```, ```Redis```, ```Visual Studio Code``` & ```MongoDB``` installed for your specific platform.

Visual Studio Code (Live Code Sharing) : [Installer-file-vscode](https://code.visualstudio.com/)

NodeSource : [Install instructions in details](https://github.com/nodesource/distributions)

Open up a terminal in your ```Linux``` machine. Windows users should ```SSH``` into Linux VM (VMWare).

```bash
$ sudo apt-get install curl
$ sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
$ sudo apt-get install -y nodejs
$ sudo apt-get install redis-server redis-cli
$ cd ~/Documents
$ sudo mkdir Pingman.io
$ cd Pingman.io
$ sudo git clone https://github.com/pingman-io/Pingman-Backend.git
$ sudo git clone https://github.com/pingman-io/Pingman-Datastore.git
```
This will create a folder ```Pingman.io``` in ```Documents``` folder and clone both the repositories there. :) 

Node.js Install : 

```bash
$ sudo apt-get install nodejs -y
$ sudo npm install
$ sudo npm install 
$ sudo npm start
```
Press ```Ctrl+C``` to stop/terminate Node.js application. ```Terminal -> Ctrl+C```.

MongoDB : [Install instructions in detail](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/#install-mongodb-community-edition-using-deb-packages)

```bash
$ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 9DA31620334BD75D9DCB49F368818C72E52529D4
$ echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.0.list

$ sudo apt-get update
$ sudo apt-get install -y mongodb-org
```

Run MongoDB : 

This will run ```mongod``` service in the background. 

```bash 
$ sudo service mongod start
```

MongoDB Error : /data/db not found. 

```bash
$ cd /
$ sudo mkdir data
$ cd data
$ sudo mkdir db
$ cd ..
$ sudo mongod --dbpath /data/db --port 27012
$ sudo service mongod start
```

### Running the Application : 

Open up a terminal in the cloned repository from above. 

```bash 
$ sudo apt-get install npm
$ sudo apt-get install yarn
$ sudo npm install 
$ sudo npm install react reactjs babel --save
$ sudo npm install angular angularjs --save
$ sudo npm install express-generator -g
$ sudo npm start
```
Open Chrome : [Pingman.io-local-link](http://localhost:3000)

### Application Specifics : 

```SSL Certificates are self signed and needs to be installed as Trusted Root Store. ```

1. Node.js [Node.js Install](https://nodejs.org/en/download/)

2. MySQL [MySQL Install](https://dev.mysql.com/downloads/)

3. MySQL Windows [MySQL Windows](https://dev.mysql.com/downloads/windows/)

4. REDIS [Redis Install](https://redis.io/download)

5. MongoDB [Mongo Install](https://www.mongodb.com/download-center/community)

### The Model. 

```1. Backend :  Works on Node.js, Express, Yarn backend. ```

```2. Datastore : API & WebSockets requests via XHR or rpc to Bittrex, Poloniex, Binance backend.```

```3. Frontend : Connects to Node.js backend and fires XHR every 100ms time for auto updation.```

```4. Website : To be hosted on VPS along with seperate backend data store. ```

### Diagram : 

![alt-tag](https://github.com/pingman-io/Backend-Framework/blob/master/public/images/CryptoPing.jpeg)


