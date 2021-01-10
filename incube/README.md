# Tech Challenge - Automation

## Prerequisites
- CentOS 7
- ansible 2.10 or above

## Folder structure

``` sh
└── incube
    ├── README.md
    ├── group_vars
    │   └── all
    ├── hosts
    ├── main.yml
    └── roles
        ├── database
        │   ├── files
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── templates
        │   └── vars
        │       └── main.yml
        ├── firewall
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── templates
        │   └── vars
        │       └── main.yml
        ├── install-pkg
        │   ├── files
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   └── templates
        ├── ntp-server
        │   ├── files
        │   │   └── ntp.conf
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   └── templates
        ├── ssh-user
        │   ├── files
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── templates
        │   └── vars
        │       └── main.yml
        ├── webserver
        │   ├── files
        │   │   ├── default.conf
        │   │   └── www.conf
        │   ├── handlers
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   └── templates
        └── wordpress
            └── tasks
                └── main.yml
```
        
## Example command
- execute the command inside the incube folder
  
  `ansible-playbook main.yml -i hosts --ask-pass -K`
  
