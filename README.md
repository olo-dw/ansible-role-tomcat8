# Ansible Role Tomcat8
Ansible role to install tomcat8

## Prerequisites

* Java 7+
* libservlet3.1-java

## Usage

    http://<server>:<port>/
    http://localhost:8080

## Example Playbook

    - name: Tomcat servers installation
      hosts: tomcat-servers
      roles:
      - role: ansible-role-tomcat8
        tomcat_extra_packages:
        - openjdk-8-jdk
        - libservlet3.1-java

## Advanced Options

**tomcat_extra_packages**: If you want to add some extra packages, especially libservlet3.1-java.

**tomcat_cache_valid_time**: 3600 - Update the apt cache if its older than this value in seconds.

## License

MIT

## Author Information

This role was created in 2018 by Olivier Locard on the behalf of Deveryware.
