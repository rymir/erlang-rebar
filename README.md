Erlang-Rebar
========

This role will install Erlang rebar from [rebar](https://github.com/rebar/rebar).

Requirements
------------

This role requires Ansible 1.4 or higher, and platform requirements are listed in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:

* `erlang_rebar_git`: location of the rebar git repository [default: `https://github.com/rebar/rebar.git`]
* `erlang_rebar_src_path`: where to clone the rebar git repository [default: `~/src/rebar`]
* `erlang_rebar_version`: rebar version to install [default: `2.2.0`]
* `erlang_rebar_bin_path`: where to store the rebar binary [default: `~/bin/rebar`]

Example Playbook
-------------------------

    - hosts: all
      roles:
         - { role: rymir.erlang-rebar, erlang_rebar_version: 2.2.0 }

Dependencies
------------

[Ansibles.erlang](https://galaxy.ansible.com/list#/roles/541)

License
-------

MIT

Author Information
------------------

rymir
