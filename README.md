# Ansible-Application
Collection of ansible playbooks for automating project deployment

# Table of Contents

* [Description](https://github.com/ejson03/Ansible-Application#description)
* [Dependencies](https://github.com/ejson03/Ansible-Application#dependencies)
* [Installation](https://github.com/ejson03/Ansible-Application#installation)
  * [Prerequisites](https://github.com/ejson03/Ansible-Application#prerequisites)
  * [Instructions](https://github.com/ejson03/Ansible-Application#instructions)
* [Usage](https://github.com/ejson03/Ansible-Application#usage)

# Description

Ansible solves the problem for efficient distribution of projects developed. The playbooks can be used to generate an environment suitable for the application to be deployed into. Also project distribution and control can be efficiently managed in multi nodal enviornment. Distribution of loads across nodes enhances the overall performance of the application.

This repository involves playbooks for :
* LAMP Stack Flask WebApp
* Owncloud Setup
* Deploying Computer Vision Models

# Dependencies

* [Ansible](https://www.ansible.com/)
* [Vagrant](https://www.vagrantup.com/)
* [Python](https://www.python.org/)
* [VirtualBox](https://www.virtualbox.org/)

# Installation

### Prerequisites

Ansible can only run on Linux Distributed Operating Systems

If you already possess either of the above operating system platforms you can skip the below procedure

* Setup Vagrant Environment
  1. Install Vagrant and virtualbox
  2. [Vagrantfile](https://github.com/ejson03/Ansible-Application/blob/master/Vagrantfile) use this vagrantfile to setup your virtual            machine
  ```
  vagrant up [hostname]  Enable all virtual machines or specify any one to enable
  vagrant ssh hostname
  ```

### Instructions

1. Setup Ansible hosts in /etc/ansible/hosts
2. Setup Ansible config in /etc/ansible/ansible.cfg
```
ansible-playbook all <play-name>
```

# License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[MIT License Link](https://github.com/ejson03/Ansible-Application/blob/master/LICENSE)
