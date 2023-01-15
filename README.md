ansible-role-docker-pi
=========

This is an ansible-playbook to setup an raspberry-pi with docker and docker-compose|


Example Playbook
----------------

```yaml
---
- hosts: raspberrypi

  roles:
    - role: 'babanomania.docker_pi'
```

Tests
-----

Below are the steps to test this role

1. Copy the file __test/example.inventory.ini__ to __tests/inventory.ini__
2. Change the ip and username in the __tests/inventory.ini__ file to your raspberry pi's ip and default ssh user.
3. Ensure passwordless ssh is setup between your host and the raspberry pi
4. Run the below command

```bash
ansible-playbook -i tests/inventory tests/test.yml
```

License
-------

MIT
