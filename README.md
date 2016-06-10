# Ansible Role: grafana-repo

Sets up the Grafana package repository on RedHat/CentOS or Debian/Ubuntu Linux OS family 
servers.

## Requirements

None

## Role Variables

Available variables are listed below with default values (see `defaults/main.yml`):

    grafana_repo_channel: stable

This variable defines the repo channel to setup. The Grafana repo channels available 
are "stable" and "testing." 

## Dependencies

None

## Example Playbook

The most basic usage of this role in a play is as follows:

    - hosts: servers
      roles:
         - role: 'tima.grafana-repo'

To setup the testing channel for Grafana's repository pass in `grafana_repo_channel` 
with the value of "testing": 

    - hosts: servers
      roles:
         - role: 'tima.grafana-repo'
           grafana_repo_channel: testing

## Contributions and Feedback

Any contributions are welcome. For any bugs or feature requests,
please open an issue through Github.

## License

BSD

## Author

Created by [Timothy Appnel](https://github.com/tima).
