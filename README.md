# lab
On demand virtual lab creation, provisioning, and life-cycle management repo

# Development Containers

## Containers to assist quick prototyping

To install/try any package without affecting main OS, to try some test code in isolated environment, containers are the quick & easy option.

The choice of container for trying out certain stuff depends on type of isolation demanded by target software/application/package.

Some applications like LAMP/full-stack can work with minimal isolation. So, docker is enough to try them out.

Whereas, some applications like DPDK require a full VM environment for them to work. In such case, vagrant needs to be used.

## To auto-create throwaway/snowflake test topology

While few test topologies require more careful and nuanced bringup, most topos can be brought up with simple script.

Depending on whether VM based or docker based topo, the networking needs to be adjusted accordingly. A VM based topo may have OVS.

These snowflake topos are use-n-throw. Use it till you are toying with certain idea. They dismantle it at push of a button.

A new testbed of required topology on given server can be brought up instantly within few mins.

## To auto-create development environment

Setting up a development environment is a time-consuming task, which can be automated. Which sets up:
- Custom environment with personal config and scripts.
- Setup nightly/periodic housekeeping job for cleanup & update

A new dev machine on given server can be brought up instantly within few mins.

## Fewer dependency on Host OS

As most of the work happens in virtualized, isolated environment, the host OS will be clean. Only need to install few container tools.
