Vector-role
=========

This role install and configure `vector` on target host(s).

Role Variables
--------------

| VarName        | Description                                                      |
|----------------|------------------------------------------------------------------|
| vector_version | Required version of vector to be install                         |
| vector_log_dir | Path to directory where vector search *.log files for monitoring |

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - vector-role 
```

License
-------

MIT

Author Information
------------------

Sergey Zhukov (beatljs@mail.ru)

DevOps-32
