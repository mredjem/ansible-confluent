# tests

**Prerequisites:**

 - Vagrant

## Install

Create the Vagrant virtual machines with:

```sh
$ vagrant up
```

This should create 2 virtual machines:

```sh
$ vagrant status

Current machine states:

kafka                     running (virtualbox)
zookeeper                 running (virtualbox)
```

## (Re)Provision

The Ansible playbook can be played at will with:

```sh
$ vagrant up --provision
```

## Cleanup

Destroy the Vagrant virtual machines with:

```sh
$ vagrant destroy -f
```
