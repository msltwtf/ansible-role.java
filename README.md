Ansible Role: java
=========

[![CI](https://github.com/msltwtf/ansible-role.java/actions/workflows/ci.yml/badge.svg)](https://github.com/msltwtf/ansible-role.java/actions/workflows/ci.yml)

An ansible role that installs openjdk-jre and optionally openjdk-jdk on RedHat/CentOS or Debian/Ubuntu.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values from `defaults/main.yml`

| Variable           | Default | Comment                    |
| :----------------- | :------ | :------------------------- |
| `java_version`     | `11`    | Java version to install    |
| `java_install_jdk` | `False` | Install or not install jdk |

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  vars:
    java_install_jdk: True
  roles:
    - msltwtf.java
```

License
-------

BSD
