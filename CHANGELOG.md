# Docker Image Packaging for OpenJDK

## 13.0.2-XalvistackY - TBC

### Major Changes

## 13.0.2-4alvistack1 - 2020-03-04

### Major Changes

  - Revamp with Molecule and `docker commit`
  - Hotfix for systemd

## 13.0.1-3alvistack1 - 2020-01-15

### Major Changes

  - Replace `dumb-init` with `tini`, as like as `docker --init`
  - Include release specific vars and tasks

## 13.0.1-2alvistack1 - 2020-01-07

  - Ubuntu 18.04 based
  - Handle ENTRYPOINT with dumb-init
  - Self initialize with Ansible, by dogfooding with Ansible Playbook
