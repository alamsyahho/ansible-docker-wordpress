# Ansible Role: docker-wordpress

Ansible role to setup wordpress site using docker container

## Requirements

CentOS 7 Minimal Installation

## Sample Playbook

`playbook.yml`

    - hosts: wordpress-servers
      roles:
        - docker-wordpress
      become: true
      become_method: sudo

`hosts`

    [wordpress-servers]
    server.example.com

Running ansible playbook:

    ansible-playbook -i /path/to/your/ansible_hosts playbook.yml

## License

MIT
