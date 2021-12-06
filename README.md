# icinga_playground

## Description

An ansible playbook ran by Vagrant to setup a debian box running icinga2.

## Usage:

First clone the git repo:

    git clone https://github.com/kevinwaro/icinga_playground.git && cd icinga_playground.

Then let Vagrant play the music:

    vagrant up

### Icingaweb2 dashboard

Once Vagrant has been ran, you can open your browser at the address http://192.168.200.10/icingaweb2 to access icinga. The default
admin credential can be found in the [main.yml](roles/icinga2/vars/main.yml) file of the vars folder.

### Access to the boxes:

You can log into the boxes by running the following commands:

    vagrant ssh

## Credits:

* author: kevinwaro
* contact: kevinwaro@yahoo.fr

## Licence

This project is licensed under the GNU GPLv3 License - see the [License.md](License.md) file for details
