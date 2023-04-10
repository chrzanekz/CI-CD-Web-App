# CI-CD-Web-App

This playbook does the following:

Installs Apache, PHP, and MySQL using the apt module.
Downloads and extracts the latest version of WordPress to the web root directory using the get_url and unarchive modules.
Creates a MySQL database for WordPress and sets up a user with privileges to access the database using the mysql_db and mysql_user modules.
Configures WordPress by generating a wp-config.php file using a Jinja2 template and the template module.
Sets file permissions on the WordPress directory and its contents using the file module.
Sets up an Apache virtual host for the WordPress site using a Jinja2 template and the template module, and restarts the Apache service using the service module.
Note that this playbook assumes that you have a Debian-based system and that you have installed Ansible on your local machine. You'll also need to create the necessary Jinja2 templates for the wp-config.php file and the Apache virtual host configuration.
