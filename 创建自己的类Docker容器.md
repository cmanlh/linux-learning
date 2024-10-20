## 使用namespace机制为容器提供独立且封闭以下资源
> 命令：[unshare](https://man.archlinux.org/man/unshare.1.en)

### namespace类型
- mount namespace
- UTS namespace
- IPC namespace
- network namespace
- PID namespace
- cgroup namespace
- user namespace
- time namespace

## 通过cgroup控制容器可使用的资源配额
> 配置项：/sys/fs/cgroup

## 为容器设置独立的根目录空间
> 命令：[chroot](https://man.archlinux.org/man/chroot.1)

**构建完善用户空间，一般建议使用busybox**

## 挂载必要的文件系统
> 命令：[mount](https://man.archlinux.org/man/mount.8)

### 必要文件系统
- /proc
- /sys
- /dev

### 用C实现容器的开源项目
- [Create Your Own Container in C](https://github.com/bayegaspard/Build-your-own-Container-from-scrath-in-C)
- [c_container](https://github.com/nathanagez/c_container)