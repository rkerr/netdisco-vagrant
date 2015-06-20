
## netdisco-vagrant

Install and run the latest version of Netdisco inside an Ubuntu 14.04 Vagrant VM using Ansible.

## Requirements:

* Vagrant > 1.6
* Ansible > 1.6
* VirtualBox

## Usage

```
$ vagrant up
```

If you're not a fan of ASCII art cows you may want to `export ANSIBLE_NOCOWS=1` before running.

The first run will take some time to download and install all the dependencies, subsequent runs should be quicker.

Once `vagrant up` Vagrant box will now be running Netdisco, with the web interface mapped through to localhost:5000.

The default web interface user/password is: `netdisco/netdisco`

The `deployment.yml` file is mapped from the host into the VM - any changes made (eg community strings) should be automatically picked up by Netdisco.

To update to a later Netdisco version rerun provisioning:

```
$ vagrant provision
```
