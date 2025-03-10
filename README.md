Vector role
=========

Deploy Vector to host

Requirements
------------
Centos 7

Role Variables & default values
--------------

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `vector_version` | 0.42.0 | vector version that you need to install |
| `vector_install_dir` | /opt/vector | directory to download and unarchive vector package |
| `vector_service_file` | /etc/systemd/system/vector.service | *DO NOT CHANGE* need to register vector as a service |
| `vector_config_file` | /opt/vector/vector.toml | location to save your vector config *IF YOU CHANGE vector_install_dir YOU NEED TO CHANGE THIS TOO* |
| `vector_address` | EMPTY | address for your machine |
| `vector_config_path` | template/vector_template.toml.j2 | local path to vector config file |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - src: git@github.com:DaddyMorlan/vector-role.git
    scm: git
    version: "1.0"
    name: vector 

License
-------

Morlan

Author Information
------------------

DaddyMorlan
