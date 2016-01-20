# Debian 8 Jessie Kernels for Versatile Express A15
Linux kernels for Versatile Express A15 virtual hardware running as KVM virtual machine (VM) on Cubietruck (armhf).

The kernels are built from Debian 8 Jessie kernel sources, see https://packages.debian.org/jessie/linux-source-3.16 .

For running als KVM VM on Cubietruck hardware the kernels are compiled with following changes related to default settings:

- General setup -> Configure standard kernel features (expert users)        
- General setup -> open by fhandle syscalls                                 
- Enable the block layer -> Support for large (2TB+) block devices and files

For each kernel verion two files are available:

- Kernel (zImage)
- VE A15 dtb file
