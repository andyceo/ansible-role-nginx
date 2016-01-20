# Ansible Role: nginx

Install nginx (naxsi version), add virtual hosts and provide ability to set settings for them.

Every task in this role have to be executed under root privileges, so use `become: yes` (Ansible 2.x) or `sudo: yes` (Ansible 1.x) on playbook level.

This role can manage most popular nginx usage scenarios:

1. Nginx as main server, no requests send to any backends nor dynamic content generated. Nginx just serve static content
2. Nginx as main server with php-fpm backend,
3. Nginx as main server with apache2 backend, works as proxy

Below every scenario will be explained in details.

## Nginx as static main server

**Prerequisites:**

- Site should be already installed in some folder on your server.

1. Disable any upstreams
2. Setup virtual host

## Nginx as main server with php-fpm as backend

1. Leave only php-fpm upstream
2. Setup virtual host as folloing:

## Nginx as main server proxy with apache2 backend

## Requirements

Ubuntu 14.04
