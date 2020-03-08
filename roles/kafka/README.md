# ansible-kafka

This role creates a kafka broker deployed through Docker and configured with a volume mounted to `/etc/kafka`.

## Requirements

For now the role is intended to run on a virtual machine or an EC2 instance with a recent enough distribution to run Docker. No other requirements are needed for now.

## Role Variables

The variables and their default values can be found under the `defaults/main.yml` file as expected from an Ansible Galaxy compliant role.

## Dependencies

Check the [requirements.yml](../requirements.yml) file.

## Example Playbook

A basic playbook to run the `kafka` role:

```yml
- name: Install Kafka
  hosts: kafka
  become: yes
  roles:
    - { name: kafka, tags: ["kafka"] }
```
