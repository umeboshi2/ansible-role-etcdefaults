Role Name
=========

Set values for the various files in ```/etc/default/``` in debian 
based systems.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Look at the defaults for the variables.  For the variables, the top level
name is ```etcdefaults```.  The ```default_etcdefaults``` defined 
in ```defaults/main.yml``` are combined into a ```combined_etcdefaults``` 
variable.  It would be preferable to be able to redefine ```etcdefaults```,
but the jinja ```combine``` filter seems to be unable to do this.

The ```etcdefaults_files``` variable contains the list of files that are 
handled by this role.  If the file doesn't exist on the target machine, it 
will NOT be created.


Dependencies
------------

No dependencies.  This is a basic debian role, possibly useful for 
other debian based distributions.

Example Playbook
----------------

TODO: make a better example

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

public domain

Author Information
------------------

[Author](https://github.com/umeboshi2)
