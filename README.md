# README.md
# Ansible Role: Django deployment using uwsgi and nginx
Deploys django project to the server, uses uwsgi, nginx and supervisord.

# Requirements
server: ubuntu-14.04-x86_64

# Variables
vassals_dir: /etc/uwsgi/vassals
supervisor_conf_dir: /etc/supervisor/conf.d
mysql_server_password:

nginx_dir: "/etc/nginx"
nginx_conf_dir: "{{nginx_dir}}/sites-available"
nginx_sites_dir: "{{nginx_dir}}/sites-enabled"
nginx_access_log: "/home/{{project_name}}/logs/access.log"
nginx_error_log: "/home/{{project_name}}/logs/error.log"
