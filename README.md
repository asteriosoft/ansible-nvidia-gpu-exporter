nvidia-gpu-exporter
=========

Role for prometheus nvidia gpu exporter in docker compose environment.

Role Variables
--------------

To do

Example Playbook
----------------
```
- hosts: servers
  become: yes
  gather_facts: yes

  vars:
  
  roles:
    - nvidia-gpu-exporter
```