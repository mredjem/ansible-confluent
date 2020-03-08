# ansible-zookeeper

This role starts a Zookeeper server deployed through Docker and configured with a volume mounted to `/etc/zookeeper`.

## Requirements

For now the role is intended to run on a virtual machine or an EC2 instance with a recent enough distribution to run Docker. No other requirements are needed for now.

## Role Variables

The variables and their default values can be found under the `defaults/main.yml` file.

## Dependencies

Check the [requirements.yml](../requirements.yml) file.

## Example Playbook

A basic playbook to run the `zookeeper` role:

```yml
- name: Install Zookeeper
  hosts: zookeeper
  become: yes
  roles:
    - { name: zookeeper, tags: ["zookeeper"] }
```
