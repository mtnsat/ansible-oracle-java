# Ansible Role: Oracle Java [![Build Status](https://travis-ci.org/mtnsat/ansible-oracle-java.svg?branch=master)](https://travis-ci.org/mtnsat/ansible-oracle-java)

Installs the Oracle Java JDK using a package provided by http://www.webupd8.org on Debian/Ubuntu Linux servers. See also my [blog](https://www.dev-eth0.de/blog/2016/11/15/ansible_oracle_java.html)

## Installation

You can either use ansible-galaxy to install this role:

    ansible-galaxy install deveth0.oracle-java

Or checkout this git-repository to your roles directory:

    git clone https://github.com/mtnsat/ansible-oracle-java.git roles/mtnsat.oracle-java


## Role Variables

Available variables are listed below, along with the default values:

You can configure which java-version to use:

    oracle_java_version: 8

By default the Java environment variables are set:

    oracle_java_set_default: True

Set the package state to 'latest' to upgrade, or 'absent' to remove

    oracle_java_state: present


## Dependencies

No dependencies required

## Example Playbook

    - hosts: foo
      roles:
        - role: mtnsat.oracle-java
          oracle_java_version: 7


## License

Apache License 2.0

## Author Information

This Role was created by [Alex Muthmann](http://dev-eth0.de).
