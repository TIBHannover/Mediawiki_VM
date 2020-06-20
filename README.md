## bring up VM
`vagrant up`

## run ansible playbook
`ansible-playbook ansible/system.yml`.

## Ansible structure
```
├── roles
│   ├── git
│   │   └── tasks
│   │       └── main.yml
│   ├── mariadb
│   │   ├── files
│   │   │   └── mysql.cnf    - db configuration file
│   │   ├── localvm_vars.yml
│   │   └── tasks
│   │       └── main.yml
│   ├── mediawiki
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── tasks
│   │   │   ├── composer.yml
│   │   │   ├── main.yml
│   │   │   └── mysql.yml
│   │   └── templates
│   │       └── mediawiki.nginx.conf.jinja2
│   ├── php
│   │   ├── handlers
│   │   │   └── main.yml
│   │   └── tasks
│   │       └── main.yml
│   └── semantic
│       └── tasks
│           └── main.yml
└── system.yml
```