---
abstract: Ansible Role to join a node to an existing cluster.
date: 2025-08-21
title: Join a node to the cluster
---

A brief description of the role goes here.

## Requirements

`kubectl` and `kubeadm` available in the executable path of the targets.

## Role Variables

n/a

## Dependencies

n/a

## Example Playbook

After you have run the code in the [ansible-kcp](https://github.com/edwardtheharris/ansible-kcp.git)
repository, you should find in this repository the text files required to parse for connection
information to the cluster.

This is generally handled with certificates and matching tokens, which should be generated during
the build process.


```{code-block} yaml

- name: join
  hosts: k8s-nodes
  roles:
      - { role: username.rolename, x: 42 }
```

### License

Copyright (c) 2025, Xander Harris. All rights reserved.
