ANSIBLE-ROLE-BIND-CONFIG
========================

Ansible Role config bind in standalone

## Howto use this role?
This role need to be include in a playbook. 

Call this **Galaxy** role  like this:

````bash
ansible-galaxy install -r requirements.yml 
````

Inside requirements.yml
````yaml
# from GitHub, overriding the name and specifying a specific tag
- src: fcolinet.bind-config
````

More info => [Ansible Docs](https://docs.ansible.com/ansible-container/roles/access.html)

## Requirements

 * Ansible 2.9+


Role Variables
--------------

```yaml
---
# Put role variables
```

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

  - hosts: all
    roles:
      - { role: fcolinet.bind-config, tags: mytags }


Molecule testing framework
--------------------------

You can use molecule to test this role.
```bash
image=alpine tag="3.15" molecule converge 
image=alpine tag="3.15" molecule verify 
```