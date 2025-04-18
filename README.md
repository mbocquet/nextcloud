# nextcloud

Ansible role to install and configure Nextcloud.

## Requirements

On the target :
* php-fpm
* nginx

Available from target :
* A nextcloud compatible database (ex: mysql / mariadb / pgsql)

## Role Variables

Many. See defaults/main.yml.

If php_version is set somewhere (group_vars / host_vars / inline) it will be
used in Nextcloud's cron job.

Ex: php_version: "8.3"

## Dependencies

None.

## Install this role as submodule of an existing GIT repository

`git submodule add https://git.sekoya.org/mb/nextcloud.git roles/nextcloud`

## Example Playbook

    - hosts: servers
      roles:
         - nextcloud


    - hosts: servers
      roles:
         - { role: nextcloud, x: 42 }

if any variables comes in the future for this role.

## License

GPLv3

## Author Information

<a href="http://www.sekoya.org" target="new">http://www.sekoya.org</a>
