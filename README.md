# **Ansible-Docker**

Ansible-Docker is an Ansible role for installing and configuring Docker.

## **Requirements**

At the moment this role is being written for Debian based distributions e.g. Debian/Ubuntu. It may evolve to include other major distributions.

## **Role Variables**

  - `DOCKER_PREREQUISITES` - Pre-requisites for installing Docker.
  - `DOCKER_PKG` - Package name of Docker. Use this to install specific version of Docker. Helpful when you have to setup Kubernetes.

## **Dependencies**

This role doesn't depends on any other role for execution.

## **Example Playbook**

Facts gathering must be enabled.

An example of running the role is as follows:
```yaml
- hosts: servers
  gather_facts: True
  roles:
      - Ansible-Docker
```

## **License**

This playbook is licensed under MIT License (See the LICENSE file).

## **Author**

[Saad Ali](https://github.com/nixknight)
