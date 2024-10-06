---
abstract: This role resets existing K8S nodes to prepare for the join role.
authors:
    - name: Xander Harris
      email: xandertheharris@gmail.com
date: 2024-07-24
title: K8S nodes roles
---

## Roles Usage

To run the full cycle on your target nodes simply run the playbook with no tags.

```{code-block} shell
ansible-playbook site.yml
```

```{index} roles; reset
```

```{toctree}
:caption: Roles Contents

join/index
reset/index
```
