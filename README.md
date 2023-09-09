Vector-role
=========

This role install and configure vector on target host(s).

Requirements
------------

For correct configuring vector, ansible must provide following variables:

| VarName  | Description                                          |
|----------|------------------------------------------------------|
| db_name  | The name of the database that vector will connect to |
| db_table | The table name in database                           |
| db_user  | User name for database connection                    |
| db_pass  | User password                                        |

Role Variables
--------------

| VarName        | Description                                                      |
|----------------|------------------------------------------------------------------|
| vector_version | Required version of vector to be install                         |
| vector_log_dir | Path to directory where vector search *.log files for monitoring |

Example Playbook
----------------

    - hosts: servers
      roles:
         - vector-role 

License
-------

MIT

Author Information
------------------

Sergey Zhukov 
(beatljs@mail.ru)
