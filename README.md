# nginx-box

| License | Versioning | Build |
| ------- | ---------- | ----- |
| [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release) | [![Build status](https://ci.appveyor.com/api/projects/status/equ3u3hfqtrllnj4/branch/master?svg=true)](https://ci.appveyor.com/project/nikAizuddin/nginx-box/branch/master) |

Developer box for [NGINX](https://www.nginx.com/).


## Creating Vagrant Box

Copy example pillar file NGINX. Optionally you may want to edit the values in the `nginx.sls`:
```
$ cp -v salt/roots/pillar/zabbix-agent.sls.example salt/roots/pillar/zabbix-agent.sls
$ cp -v salt/roots/pillar/filebeat.sls.example salt/roots/pillar/filebeat.sls
$ cp -v salt/roots/pillar/nginx.sls.example salt/roots/pillar/nginx.sls
$ cp -v salt/roots/formulas/nginx-formula/nginx/files/https.conf.example salt/roots/formulas/nginx-formula/nginx/files/https.conf
```

Copy vagrant file from `vagrant/examples/` and then create the vagrant box (you can change to `--provider=libvirt` if you want to use Libvirt provider):
```
$ cp -v vagrant/examples/Vagrantfile.nginx-box.fedora-33.x86_64.example vagrant/Vagrantfile.nginx-box
$ vagrant up --provider=virtualbox
```

Provision the vagrant box:
```
$ vagrant ssh nginx-box -- sudo salt-call state.highstate
```

Deploy NGINX with self-signed certificate:
```
$ vagrant ssh nginx-box -- sudo salt-call state.sls nginx,nginx.service
```
