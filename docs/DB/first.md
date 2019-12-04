---
layout: default
title: MongoDB
nav_order: 1
has_children: true
---

# Error system has not been booted with systemd as init system (pid 1). can't operate. mongodb || MongoDB service failed to start (unrecognized service ) || MongoDB – Failed to unlink socket file /tmp/mongodb-27017

**Useful Resource:** https://mithun.co/tips/init-script-for-mongodb-4-on-wsl-in-ubuntu-18-04/

### Steps:

- `sudo curl -o /etc/init.d/mongodb https://raw.githubusercontent.com/mongodb/mongo/master/debian/init.d`

- `chmod +x /etc/init.d/mongodb` || `chmod +x mongo`

- `sudo mongod --repair --dbpath`

- `sudo apt-get update`

- `sudo apt-get install -y mongodb-org`