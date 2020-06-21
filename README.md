## bring up VM
`vagrant up`

## run ansible playbook
`ansible-playbook ansible/system.yml`.

## Once Mediawiki VM is created:
* http://192.168.60.10/mediawiki/

* MW user: adminpwd
* MW user passwd: adminpwd

## Variables' locations
* MW & MariaDB vars: `ansible/roles/mediawiki/defaults/main.yml`
* MW extensions: `ansible/roles/mediawiki/vars/extensions.yml`
