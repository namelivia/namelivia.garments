# Garments client Ansible role [![Ansible Lint](https://github.com/namelivia/ansible-garments-client/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/namelivia/ansible-garments-client/actions/workflows/ansible-lint.yml)

## This is a WIP

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/ansible-ansible-garments-client
```

## Required variables
 - `cloudwatch_region` Cloudwatch region to send the logs to.
 - `cloudwatch_log_group` Cloudwatch log group to send the logs to.
 - `garments_api_endpoint` API endpoint for connecting the client to the server API.
 - `domain_name` Domain name for the app.
