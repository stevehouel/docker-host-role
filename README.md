# Docker Host playbook #


## Requirements

This project must be cloned under specific project's Ansible Roles to Install Docker Package to Host.

## Mandatory Variables

`http_proxy` : Proxy Http

`https_proxy` : Proxy Https

`no_proxy` : No Proxy var

## Optional Variables for every Hosts

`docker_hostname` : Docker images will be stocked under `docker_image_path`/`docker_hostname`. Defaults to *{{ ansible_host.split('.')[0] }}*

## Optional Variables

`ansible_ssh_pub_key` : Set this variable to add a ssh key to the Ansible User

`docker_insecure_registries` : Urls to unsecure registries (Create Ansible variable in table). Default to *["registry.prod.athena.ts-agora.com"]*

`docker_image_path` : Path where Docker images are stocked. Default to */data/docker*

