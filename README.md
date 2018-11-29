# apache

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-apache.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for apache

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.apache`

# Default settings

```

apache_listen_port: 80
apache_listen_ssl: true
apache_disable_modules:
  - mpm_event

apache_enable_modules:
  - rewrite
  - vhost_alias
  - headers
  - expires
  - mpm_prefork
  - filter
  - ssl

apache_user_public_keys: []

apache_group: www-data
apache_user: www-data

apache_security_server_tokens: "Prod"
apache_security_server_signature: "Off"
apache_security_trace_enabled: "Off"
apache_security_headers_x_content_type_options: "nosniff"
apache_security_headers_x_frame_options: "sameorigin"

```
