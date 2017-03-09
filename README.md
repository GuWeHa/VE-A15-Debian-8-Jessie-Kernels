# Debian 8 Jessie Kernels for Versatile Express A15
Linux kernels for Versatile Express A15 virtual hardware running as KVM virtual machine (VM) on Cubietruck (Allwinner A20).

The kernels are built from Debian 8 Jessie kernel sources, see https://packages.debian.org/jessie/linux-source-3.16 .

For running as KVM VM on Cubietruck the kernels are compiled with the following changes:

| menu item              | enabled kernel feature                            |
| :--------------------- | :------------------------------------------------ |
| General setup          | Configure standard kernel features (expert users) |
| General setup          | open by fhandle syscalls                          |
| Enable the block layer | Support for large (2TB+) block devices and files  |

There are two files available for each kernel version:

| file                                         | purpose                                                    |
| :------------------------------------------- | :--------------------------------------------------------- |
| vexpress-debian-3.16.39-1+deb8u2-zImage      | zImage (Kernel)                                            |
| vexpress-debian-3.16.39-1+deb8u1-zImage      | zImage (Kernel)                                            |
| vexpress-debian-3.16.7-ckt20-1+deb8u4-zImage | zImage (Kernel)                                            |
| vexpress-debian-3.16.7-ckt20-1+deb8u3-zImage | zImage (Kernel)                                            |
| vexpress-v2p-ca15-tc1.dtb                    | hardware specific (Versatile Express A15) device tree blob |

Have fun!
