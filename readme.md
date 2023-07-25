# Server
This repository contains scripts and guides that are applicable to my server.

## Initial Setup of New Server
* Add new user
```console
$ useradd -m -s /bin/bash <username>
$ passwd <username>
```
* Allow sudo for the newly created user by adding to sudo group:
```
# Allow <username> to use sudo
<username>     ALL=(ALL:ALL) ALL
```
* Login with the newly created user and add SSH public key
```
$ mkdir .ssh && cd .ssh
$ vi authorized_keys
$ chmod 700 authorized_keys
$ chmod 700 .ssh
```
* Execute steps described in [SSH](/ssh) directory

## Maintenance
* Update
```
$ sudo apt update
$ sudo apt upgrade
```

## Misc
* Generate SSH key
