# vayu-kernel-docker

Automated build workflow to compile a Docker-ready Linux kernel for the **Xiaomi POCO X3 Pro (`vayu` / `bhima`)** running **LineageOS 22.2 (Android 15)**.

## Enabled Kernel Features
- Full Namespaces (`CONFIG_NAMESPACES`, `CONFIG_PID_NS`, `CONFIG_NET_NS`, `CONFIG_IPC_NS`, `CONFIG_UTS_NS`, `CONFIG_USER_NS`)
- Control Groups (`CONFIG_CGROUPS`, `CONFIG_CGROUP_DEVICE`, `CONFIG_CGROUP_PIDS`, `CONFIG_MEMCG`, `CONFIG_CPUSETS`)
- Container Networking & Storage (`CONFIG_BRIDGE`, `CONFIG_VETH`, `CONFIG_OVERLAY_FS`, `CONFIG_IP_NF_NAT`, `CONFIG_NETFILTER_XT_MATCH_ADDRTYPE`)

## Output
Flashable **AnyKernel3** zip package compatible with OrangeFox, TWRP, or Lineage Recovery.
