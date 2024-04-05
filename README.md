Role Name
=========

Simple docker setup for ubuntu 20.04 or later

Requirements

-


Role Variables
--------------

      docker_packages:
        - apt-transport-https
        - ca-certificates
        - curl
        - software-properties-common
        - docker-ce
        - docker-ce-cli
        - containerd.io
        - python3-docker
      docker_repo: https://download.docker.com/linux/{{ ansible_distribution|lower }} {{ ansible_distribution_release }} stable
      docker_repo_key: https://download.docker.com/linux/ubuntu/gpg
      docker_repo_key_id: 0EBFCD88


Dependencies
------------

-

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible_docker }

License
-------

BSD

Author Information
------------------

Aleksandr Ivanov (avic.ivanov@gmail.com)
