MySQL DB
=========

Role installs and set password for MySQL database in Centos.
Post installation create a database and one username/password with full access to the database.
Creates a table and insert data in to the same.

Requirements
------------

python and MySQL-python must be installed.

Role Variables
--------------

root_db_user: root
root_db_pass: <password for root user>
db_name: <database to be created>
db_user: <normal database username>
db_pass: <normal database user password>

Dependencies
------------

ansible-galaxy collection install community.mysql

Example Playbook
----------------

    - hosts: servers
      roles:
         - mysql_db

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
