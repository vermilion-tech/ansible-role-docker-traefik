Role Name
=========
`$ ansible-galaxy install vermilion_tech.ansible_role_docker_traefik`

Installs Traefik as a Docker Container.

Requirements
------------

Requires Python

Role Variables
--------------

- `path` path to store traefik conf and acme.json in
- `traefik.version` traefik docker image tag
- `docker.network` network for traefik to listen on
- `acme.staging` use acme staging server?

See `defaults/main.yml`

Dependencies
------------

- geerlingguy.docker
- geerlingguy.pip
  - installs `docker` by default

Example Playbook
----------------
`$ ansible-galaxy install vermilion_tech.ansible_role_docker_traefik`
    - hosts: all
      roles:
         - { role: vermilion_tech.ansible_role_docker_traefik }

License
-------

BSD

Author Information
------------------

Kaden Nelson
`kaden@vermilion.tech`
vermilion.tech
