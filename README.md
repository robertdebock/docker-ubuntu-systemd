Docker Ubuntu Systemd
=====================

This Dockerfile can build containers capable to use systemd.

[![ubuntu build status](https://img.shields.io/docker/cloud/build/robertdebock/ubuntu.svg)](https://hub.docker.com/repository/docker/robertdebock/ubuntu)

Branches
--------

This repository one branche that relate to Ubuntu a version.

|Branch |Ubuntu Version       |Docker image tag|
|-------|---------------------|----------------|
|master |focal fossa (2004)   |focal           |
|bionic |bionic beaver (1804) |bionic          |

Here are Ubuntu's [supported versions](https://wiki.ubuntu.com/Releases).

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/ubuntu
```
