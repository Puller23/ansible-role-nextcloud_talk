Ansible Role: nextcloud talk
=========

Install nextcloud talk using ansible.

Requirements
------------

- Ansible >= 2.7

Role Variables
--------------

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) and are listed in the table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `hpb_customer_id` | "" | Credentials for HPB Download |
| `hpb_proxy` | false | Set this value within the host_vars for the relevant hosts.|
| `hpb_signaling` | false | Set this value within the host_vars for the relevant hosts |
| `hpb_turnserver` | false | Set this value within the host_vars for the relevant hosts |
| `turn_install_from_source` | false | Set thies to true, if you want to install coturn from source |


Dependencies
------------

none

Example Playbook
----------------

Use it in a playbook as follows:
```yaml
- hosts: all
  roles:
    - puller23.nextcloud_talk
```

License
-------

BSD

Author Information
------------------

This role was created in 2021 by Gregor Bartels.