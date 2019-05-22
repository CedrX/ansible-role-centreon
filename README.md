# centreon_ansible_role


Role Ansible pour ajouter ou supprimer une machine dans centreon



## Fonctionnement

Authentification (extra_vars attendues)
- cent_host (url)
- cent_password
- cent_username
- cent_template
- cent_hostgroup



Extra vars attendues:


Actions (valeurs possibles de la variable action à inclure avec l'ajout du role)
- add_host
- remove_host



Exemple playbook
```
- hosts: localhost
  roles:
    - { role: 'centreon', tache: 'add_host' }
```
