[![CI](https://github.com/behid/ansible-users/workflows/CI/badge.svg?event=push)](https://github.com/behid/ansible-users/actions?query=workflow%3ACI)


# ansible-users
Ansible role to create, manage users and groups. You need to use become: true globally in your playbook
for this role to work.

For example usage see default/main.yaml

## Important 
Since version 0.0.6 we use a dict instead of lists for users and groups. This is so that we can merge users between
default, group and host variables. Please note that you can't remove a setting after it's defined so
be careful when for example adding users to groups. I suggest adding users to a group at group or host level.

### Made with inspiration from
https://github.com/willshersystems/ansible-users  
https://github.com/singleplatform-eng/ansible-users   
https://github.com/debops/ansible-users  
