# lamp-stack-using-ansible
deploying lamp-stack using ansible playbook
### Ansible role for :

- installing PHP version 7.3 Dependences  and some other packages Needed for installation Latest Wordpress version
- Installing and configuring MariaDB and MariaDB-client
- Creating wordpress DataBase and DBUser for WordPress
- Removing the Annonymous user and Test DataBase to secure the Database Server
- Installing and Configuring httpd WebServer
- Downloading and Extracting The WordPress files
- Using Jinja2 Templates for creating and configuring `wp-config.php`
## Changing The Default Database Vraiables
#### I've already set the Role Vars to default values,If you want to change them
#### edit in `vars/main.yml`
```yml
##Password for MariaDB Root user
mysql_root_password: "123456789"
## WordPress-DatBase Name:
wordpress_db: "wordpress"
##Wordpress DataBase UserName:
wordpress_dbuser: "wordpress"
## WordPress DataBase Password
wordpress_dbpass: "123456789"
## WordPress Database hostname
host: "localhost"
```
