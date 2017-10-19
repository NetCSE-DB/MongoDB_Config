### MongoDB Windows Configuration
#### MongoDB Directory Structure
```sh
C:\DB\MongoDB
             - bin
             - config
             - data
             - log
             VERSION.txt
```
#### MongoDB Config File [mongod.cfg]
```sh
systemLog:
    destination: file
    path: C:\DB\MongoDB\log\mongod.log
storage:
    dbPath: C:\DB\MongoDB\data
```

#### MongoDB Service Installation
```sh
"C:\DB\MongoDB\bin\mongod.exe" --config "C:\DB\MongoDB\config\mongod.cfg" --install
```

#### Start Stop MongoDB Service
```sh
net start MongoDB
net stop MongoDB
```

#### Remove MongoDB Service
```sh
"C:\DB\MongoDB\bin\mongod.exe" --remove
````
