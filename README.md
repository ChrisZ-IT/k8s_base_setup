Role Name
=========

This role will do base config setup to prep a linux server (debian based only currently) to be use in a k8s cluster. 

Requirements
------------

At least 1 linux server (ubuntu was used for testing)

Role Variables
--------------

desired_k8s_version: latest(default)

Dependencies
------------

n/a

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      gather_facts: true
      vars_prompt:
      - name: desired_k8s_version
        prompt: Enter the Kubernetes version to install
        default: latest
        private: no
      roles:
         - k8s_base_setup

Then just point this playbook to your inventory holding your k8s nodes

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
