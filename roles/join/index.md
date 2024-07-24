---
abstract: This directory contains the playbook to create an intermediate CA.
authors:
    - name: Xander Harris
      email: xandertheharris@gmail.com
date: 2024-03-08
title: Join K8S nodes
---

## Join K8S usage

```{code-block} shell
ansible-playbook -t join site.yml
```

```{index} ansible; join
```

### Join K8S Playbook

```{literalinclude} roles/join/tasks/main.yml
:language: yaml
```
