Ansible Role: Perl(src)
================================================================================
Build and install the specified version of Perl from a source code into /usr/local

- Build and install Perl (default is v5.24.1)
- Install Perl core modules
- Install cpanm into /usr/local/bin

Requirements
--------------------------------------------------------------------------------
None

Role Variables
--------------------------------------------------------------------------------
These variables are defined in defaults/main.yml file.
```yaml
perl:
  rebuild: false
  version: 5.24.1
  install: /usr/local
  workingdir: /usr/local/src

```

Dependencies
--------------------------------------------------------------------------------
None

Example Playbook
--------------------------------------------------------------------------------
```yaml
- hosts: servers
  roles:
     - { role: azumakuniyuki.ar-perl-src, perl.version: "5.24.0" }
```

License
--------------------------------------------------------------------------------
BSD

Author Information
--------------------------------------------------------------------------------
[azumakuniyuki](http://nyaan.jp)

