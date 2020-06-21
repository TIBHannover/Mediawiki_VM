# Mediawiki VM
Fork of [semantic-mediawiki-box](https://github.com/TIBHannover/semantic-mediawiki-box), by [Mirjan Hoffmann](https://github.com/mirjan-hoffmann)

Changes:
* using Mediawiki v. 1.34
* restricted to Debian/Buster OS
* using Apache2 instead of Nginx
* installation of extensions
    * MW bundled
    * Composer extensions:

# How to:

## bring up VM
`vagrant up`

## run ansible playbook to create VM
`ansible-playbook ansible/system.yml`.

## Once Mediawiki VM is created:
* URL: http://192.168.60.10/mediawiki/

* MW user: adminpwd
* MW user passwd: adminpwd

## Variables' locations
* MW & MariaDB vars: `ansible/roles/mediawiki/defaults/main.yml`
* MW extensions: `ansible/roles/mediawiki/vars/extensions.yml`
