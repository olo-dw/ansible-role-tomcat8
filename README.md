# Ansible Role Tomcat8
Ansible role to install tomcat8

## Prerequisites

* Java 7+

## Usage

    http://<server>:<port>/
    http://localhost:8080

## Example Playbook

    - name: Tomcat servers installation
      hosts: tomcat-servers
      roles:
      - role: ansible-role-java
        java_packages:
        - openjdk-8-jdk
      - role: ansible-role-tomcat8

## License

MIT

## Author Information

This role was created in 2018 by Olivier Locard on the behalf of Deveryware.
