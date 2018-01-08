### MongoDB Windows Configuration
#### MongoDB Directory Structure
```sh
C:\database\mongodb\
             - bin\
             - config\
             - data\
             - log\
             - VERSION.txt
```
#### MongoDB Config File [mongod.cfg]
```sh
systemLog:
    destination: file
    path: C:\database\mongodb\log\mongod.log
storage:
    dbPath: C:\database\mongodb\data
```

#### MongoDB Service Installation
```sh
"C:\database\mongodb\bin\mongod.exe" --config "C:\database\mongodb\config\mongod.cfg" --install
```

#### Start Stop MongoDB Service
```sh
net start mongodb
net stop mongodb
```

#### Remove MongoDB Service
```sh
"C:\database\mongodb\bin\mongod.exe" --remove
````
