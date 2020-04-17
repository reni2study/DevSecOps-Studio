# Ansible Role: Inspec 

[![Build Status](https://travis-ci.org/secfigo/ansible-role-inspec.svg?branch=master)](https://travis-ci.org/secfigo/ansible-role-inspec)

Installs Chef's [Inspec](https://www.inspec.io/), a tool to do compliance as code 

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    inspec_version: "4.18.104"

The Packer version to install.

    inspec_arch: "amd64"

The location where the Packer binary will be installed (should be in system `$PATH`).

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - secfigo.inspec

## Testing it locally using Vagrant

```bash
virtualenv --python python3 env
source env/bin/activate
pip3 install ansible 
vagrant up 
or 
vagrant provision
```

## License

MIT

## Author Information

This role was created in 2020 by [Mohammed A. Imran](https://www.secfigo.com/), author of [Practical DevSecOps Course](https://www.practical-devsecops.com/).
