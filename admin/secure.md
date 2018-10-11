## Normally Connect to Database with Robomongo

## If You want to drop user admin
```sh
use admin;
db.dropUser('admin')
```

## Create user admin
```sh
use admin
db.createUser(
  {
    user: "admin",
    pwd: "nopass",
    roles: [ { role: "userAdminAnyDatabase", db: "admin" }, "readWriteAnyDatabase" ]
  }
)
```

## Edit /etc/mongodb.conf
```sh
auth = true
```

## Connect with this authentication
```sh
mongo -u "admin" -p "nopass" --authenticationDatabase "admin"
```

## Or Connect Normally with ` mongo ` command and use authentication
```sh
db.auth('admin', 'nopass');
```
