Role Name
=========

This role creates a user and attaches the policy defined in templates folder.

Policy details:
full access to the ec2 and deny access to cloud trail

Requirements
------------

Have access to AWS and have the security and access tokens.

and this role assumes, a iam group is already present.

run the test.yml like this

 ` ansible-playbook test.yml -e "aws_access_key=<> aws_secret_key=<>  iam_group=<> iam_password=<>" `

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: pb-ansible-aws-iam }

License
-------

BSD

Author Information
------------------

Satish Gummadelli
