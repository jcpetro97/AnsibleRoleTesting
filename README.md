# Ansible Role Testing Template

## Requirements

* Ansible (installed on development computer)
* Vagrant 
* a testing directory needs to exist inside the role directory structure.  If the role was initialized with `ansible-galaxy init <role name>` then the test directory will already be there
* add or remove ( if desired ) OS types to test against.  ( jcpetro97/os name can be swapped for any box hosted at vagrant cloud)

Example:

`{ :name => "rolename-debian10", :box => "geerlingguy/debian10" }`


## Setup

* Copy Vagrantfile to the role/test directory.
* Create a playbook to test the role functionality
* Edit Vagrantfile
  * Change `template` to the name of the role ( this is to avoid conflicts in virtalbox)
  * change `test.yml` to the name of the playbook that was written
