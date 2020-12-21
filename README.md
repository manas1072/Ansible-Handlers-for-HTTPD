# Ansible-Handlers-for-HTTPD

Restarting HTTPD Service is not idempotence in nature and also consume more resources suggest a way to rectify this challenge in Ansible playbook. 

So here we are using Ansible Handlers module to restart the service only when there is any change in the configuration file. The template module which is copying the configuration file in the target node have the notify keyword which notifies handler if there is any change done in the Configuration file.
