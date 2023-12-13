---
layout: page
permalink: /community_roles
---

# Notes on Community Roles

This page collects and notes on using community Ansible roles with RHEL9.

So far, testing has been pretty cursory - confirming roles run successfully and basic functionality works. 

* [Geerlingguy.apache](https://github.com/geerlingguy/ansible-role-apache)
  * Requires that ssl.conf be modified to remove default virtualhost
* [Geerlingguy.php](https://github.com/geerlingguy/ansible-role-php)
  * Must specify desired php packages in vars - default set includes php-xmlrpc which isn’t available on RHEL9
* [Geerlingguy.certbot](https://github.com/geerlingguy/ansible-role-certbot)
  * No issues
* [Geerlingguy.nginx](https://github.com/geerlingguy/ansible-role-nginx)
  * No issues, sample config from readme doesn’t have the correct php-fpm path (should be /var/run/php-fpm/www.sock)
* [Geerlingguy.ruby](https://github.com/geerlingguy/ansible-role-ruby)
  * No issues
* [Geerlingguy.nodejs](https://github.com/geerlingguy/ansible-role-nodejs)
  * No issues
* [Geerlingguy.redis](https://github.com/geerlingguy/ansible-role-redis)
  * No issues

Existing UMN Roles
* [UMN Sectigo Role](https://github.com/umn-ansible/umn_sectigo_role)
  * No issues

Potentially Needed Roles
* Puma
  * Can't find a good community role which is just puma
  * Would likely build one with nginx as a dep?


