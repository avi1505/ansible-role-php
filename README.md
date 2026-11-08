# PHP-role

Installeren van PHP en Apache-PHP-module op Ubuntu 24.04.
PHP testpagina aanmaken in /var/www/html/index.php.

## Afhankelijkheid

Deze role gebruikt avi1505.apache.

## Standaardvariabelen

```yaml
php_packages:
  - php
  - libapache2-mod-php

site_title: "Apache en PHP via Ansible Galaxy"
deployment_environment: "demo"
```

## Voorbeeld

```yaml
---
- name: Apache en PHP installeren
  hosts: webservers
  become: true

  roles:
    - avi1505.php
```

## Licentie

MIT