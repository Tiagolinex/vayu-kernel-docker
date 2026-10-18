# CreeviexOs Server Kernel for Poco X3 Pro (vayu)

Automated build workflow to compile the **CreeviexOs Kernel** with enhanced Docker & Home Server features for the **Xiaomi POCO X3 Pro (`vayu` / `bhima`)**.

## Source Base
- Based on [creeviexos/CreeviexOs-Kernel-vayu](https://github.com/creeviexos/CreeviexOs-Kernel-vayu) (KernelSU, Audio Fix, Performance & Display tweaks for vayu).

## Injected Server & Docker Features
- **High Performance Networking:** TCP BBR + Fair Queuing (FQ) as default congestion control.
- **Docker & Container Namespaces:** Namespaces (PID, NET, IPC, UTS, USER), Control Groups (cgroups v1/v2, cpu, memcg, devices), OverlayFS, Bridge, VETH.
- **Memory Optimization:** ZRAM with ZSTD compression + writeback.
- **Flash Storage Multitasking:** BFQ I/O Scheduler tuned for UFS 3.1.
- **Network Filesystems:** CIFS/SMB and NFS client support for mounting NAS and Windows shares.
- **Smart Home & USB Dongles:** USB-Serial drivers (CH341, CP210X, FTDI, ACM) for Zigbee/Z-Wave antennas.
- **Filesystem Compression:** Transparent F2FS compression with ZSTD.
- **Firewall & Routing:** IPSet and IPVS modules.

## Output
Flashable **AnyKernel3** zip package compatible with OrangeFox, TWRP, or Recovery.
