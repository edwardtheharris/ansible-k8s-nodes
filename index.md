---
abstract: This repo holds roles that join K8S nodes to an existing cluster.
authors:
   - name: Xander Harris
     email: xandertheharris@gmail.com
date: 2024-07-24
title: Ansible K8S Nodes
---

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/edwardtheharris/ansible-k8s-ca/ansible.yml?branch=main&style=flat-square&logo=ansible&label=Ansible%20Lint)
![GitHub CodeQL](https://img.shields.io/github/actions/workflow/status/edwardtheharris/ansible-k8s-ca/codeql.yml?branch=main&style=flat-square&logo=githubactions&label=CodeQL)
[![GitHub Pages Status](https://img.shields.io/github/actions/workflow/status/edwardtheharris/ansible-k8s-ca/pages.yml?branch=main&style=flat-square&logo=githubpages&label=GitHub%20Pages)](https://edwardtheharris.github.io/ansible-k8s-ca/)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/edwardtheharris/ansible-k8s-ca/shell.yml?branch=main&style=flat-square&logo=gnubash&label=ShellCheck)

```{index} ansible; roles
```

## Galaxy

```{toctree}
:caption: Ansible Galaxy

roles/index
```

```{index} ansible; galaxy
```

```{toctree}
:caption: meta
:maxdepth: 1

.github/index
license
readme
security
```

```{index} metadata; repository
```

## References

- [community.crypto.x509_certificate](https://docs.ansible.com/ansible/latest/collections/community/crypto/x509_certificate_module.html)
- [How to create a small CA](https://docs.ansible.com/ansible/latest/collections/community/crypto/docsite/guide_ownca.html)

### Indices and tables

- {ref}`genindex`
- {ref}`modindex`
- {ref}`search`

### Playbook

```{literalinclude} /site.yml
:language: yaml
```

### Pre-requisites

To make use of this repository, you should first set up a cluster using the
code located in
[edwardtheharris/ansible-kcp](https://github.com/edwardtheharris/ansible-kcp).
