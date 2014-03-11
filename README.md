Rails Common
========

Install ruby and associated DBs

Requirements
------------

None

Role Variables
--------------

skip_ruby: default(false) - Don't bother with ruby install
ruby_version: default(ruby2.0) - for shadowkobolt.ruby
rails_postgresql_db_name - used as base for db names (_develpment and _test are added to dbs.  This is also used as username and pwd for postgresql)

Dependencies
------------

shadowkobolt.ruby
shadowkobolt.postgresql

Example Playbook
-------------------------

    - hosts: default
      vars:
        - ruby_version: ruby2.0
        - rails_postgresql_db: appname
      roles:
        - shadowkobolt.rails-common

License
-------

BSD

Author Information
------------------

None
