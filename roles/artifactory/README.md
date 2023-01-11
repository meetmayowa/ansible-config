# Ansible Role: Package manager configuration for build machines at CCDC

Configures package managers to use artifactory on Linux/Windows/MacOS

## Requirements

geerlingguy.homebrew, used on MacOS to initialise the HomeBrew package manager

## Role Variables

-   ansible_deployment_artifactory_user: artifactory user with read only access to mirrors
-   ansible_deployment_artifactory_key: api key for above user

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - ccdc.package_manager_configuration

## License

MIT / BSD

## Author Information

This role was created in 2020 by Claudio Bantaloukas, based on existing roles at CCDC, by Jeff Geerling and google searches
