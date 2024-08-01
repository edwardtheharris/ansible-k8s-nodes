---
abstract: This role resets existing K8S nodes to prepare for the join role.
authors:
    - name: Xander Harris
      email: xandertheharris@gmail.com
date: 2024-07-24
title: Reset K8S Node
---

## Reset K8S Node Usage

```{code-block} shell
ansible-playbook -t reset site.yml
```

```{index} roles; reset
```

## Reset K8S Node Playbook

```{literalinclude} /roles/reset/tasks/main.yml
:language: yaml
```

```{ansibleautotask} Reset existing nodes
:playbook: site.yml
:role: reset
```
