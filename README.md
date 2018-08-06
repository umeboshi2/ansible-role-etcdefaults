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
but the jinja ```combine`` filter seems to be unable to do this.


Dependencies
------------

No dependencies.  This is a basic debian role, possibly useful for 
other debian based distributions.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

public domain

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
