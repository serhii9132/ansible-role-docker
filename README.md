ansible-docker
==============

An Ansible role for installing Docker.

Supported platfroms:
```
- Debian 12 (Bookworm)
- Debian 13 (Trixie)
- Ubuntu 22.04 (Jammy Jellyfish)
- Ubuntu 24.04 (Noble Numbat)
```

Docker daemon options:
---------------------

```json
"max-concurrent-uploads": 1,
"max-concurrent-downloads": 1,
"containerd-snapshotter": false
```

Requirements
------------

This role requires Ansible 2.19 or higher

Role Variables
--------------

```yaml
user: ""
```
A user to be added to the docker group

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  gather_facts: true
  roles:
    - serhii9132.docker
```

License
-------

MIT
