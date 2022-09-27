# Fabric DPDK Installation Script

This repo contains the DPDK installation script along with an example install on a 2-node Fabric slice.

The host OS in example is Ubuntu 20.04, while the NIC used is ConnectX-6.

Hugepage size is set to 4GB, which is configurable in the script and can be increased/decreased depending on application and/or system resources.

DPDK is installation directory is `/usr/src/dpdk` on the nodes. DPDK version used is 20.11 which uses meson and ninja build tools.

To confirm the working of DPDK, `dpdk-helloworld` program is run at the end of installation which should output hello from each CPU core, which is indication of a successful installation.
