### MongoDB Linux (Ubuntu) Installation From Zip Archive
#### MongoDB Directory Structure
```sh
/opt/mongodb/
           - bin/
           - config/
           - data/
           - log/
           - snmp/
           - VERSION.txt
```
#### MongoDB Config File in ` config ` folder [mongod.cfg]
```sh
systemLog:
    destination: file
    path: /opt/mongodb/log/mongod.log
storage:
    dbPath: /opt/mongodb/data
```

#### MongoDB ` mongod ` command alias in ` ~/.bash_aliases ` File
```sh
export PATH="$PATH:/opt/mongodb/bin"
alias mongod='mongod --config "/opt/mongodb/config/mongod.cfg"'
```

#### Start MongoDB Daemon
```sh
mongod
```

#### Connect with mongod
```sh
mongo
````
