# [GzOS v0.1.0](https://github.com/OpenTrustGroup/manifest/blob/gzos/release/gzos_v0.1.0) (2018-08-14)

## New Features

* Ported Trusty TEE libsm(secure monitor) to Zircon kernel
* Integrated OPTEE shared memory mechanism to Trusty linux driver and Zircon
* Implemented smc kernel object in Zircon kernel and smc service in Zircon userspace
* Implemented Trusty virtio in Zircon userspace
* Implemented Tipc agent, libtrusty_ipc and libtrusty_app(trusty syscalls) in Zircon userspace to support Trusty IPC mechansim
* Leveraged Garnet appmgr and sysmgr to support on-demand TA loading
* Implemented dynamic TA port publishing mechanism in sysmgr

## Bugs Fix

* N/A

## Known Issues

* Memory leak when testing 'tipc-test -t ta2ta-ipc'
* Deadlock sometimes occurred when testing 'tipc-test -t ta2ta-ipc'
