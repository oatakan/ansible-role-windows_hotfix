# windows_template_build
This repo contains an Ansible role that installs hotfix on Windows.

> **_Note:_** This role is provided as an example only. Do not use this in production. You can fork/clone and add/remove steps for your environment based on your organization's security and operational requirements.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
        hotfix:
          - kb: KB12345
            file: kb_file.msu
            url: http://example.com/kb_file.msu

      roles:
         - role: oatakan.windows_hotfix
           hotfix: "{{ hotfix }}"

License
-------

MIT

Author Information
------------------

Orcun Atakan

