Yacy
=========

YaCy is a distributed Web Search Engine, based on a peer-to-peer network. (https://yacy.net/)

Default port is: 8090


For more documentation, see: https://yacy.net/download_installation/  (ex. Setting password)

Role Variables
--------------

| Parameter           | Default           | Description                                                                                                           |
|---------------------|-------------------|-----------------------------------------------------------------------------------------------------------------------|
| yacy_service        | yacy              | Name of the systemd service                                                                                           |
| yacy_version_major  | 1.924             | Major version of YaCy                                                                                                 |
| yacy_version_minor  | 20210209_10069    | Minor version of YaCy                                                                                                 |
| yacy_user           | yacy              | User YaCy runs with                                                                                                   |
| yacy_user_shell     | /usr/sbin/nologin | User shell                                                                                                            |
| yacy_group          | yacy              | User group                                                                                                            |
| yacy_install_dir    | /opt/yacy         | Where to install YaCy                                                                                                 |
| yacy_admin_password |                   | The admin password for YaCy UI <br/>(default none - so you will get an error if you are trying to access it remotely) |


Dependencies
------------

No other Ansible dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: pmoscode.yacy

License
-------

MIT
