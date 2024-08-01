---
abstract: The readme for some Ansible playbooks that have the goal of deploying
    a Root Certificate Authority to a Linux host.
authors: Xander Harris
date: 2024-03-08
title: Ansible CA Readme
---

## Assumptions

The default configuration assumes a vault password exists at
{file}`/etc/ansible/vault`. It also assumes the inventory file is in YAML format
and located at {file}`/etc/ansible/hosts.yaml`

### Fact Caching

The default configuration uses fact caching with Redis running on the controller
with the default port.

## Usage

You can find an example inventory file below, this inventory is intended
to house a Kubernetes cluster with a pair of control planes that are members
of a Samba Active Directory Domain that contains a pair of controllers and
is responsible for authentication, file, and routing services.

```{code-block} yaml
:caption: /etc/ansible/hosts.yaml

---
kcp:
  hosts:
    kcp01.example.com:
      ansible_host: 172.16.0.5
k8s:
  hosts:
    k8s01.example.com:
      ansible_host: 172.16.0.11
    k8s02.example.com:
      ansible_host: 172.16.0.12
    k8s03.example.com:
      ansible_host: 172.16.0.13
    k8s04.example.com:
      ansible_host: 172.16.0.14
    k8s05.example.com:
      ansible_host: 172.16.0.15
    k8s06.example.com:
      ansible_host: 172.16.0.16
    k8s07.example.com:
      ansible_host: 172.16.0.17
    k8s08.example.com:
      ansible_host: 172.16.0.18
    k8s09.example.com:
      ansible_host: 172.16.0.19
    k8s10.example.com:
      ansible_host: 172.16.0.20
```
