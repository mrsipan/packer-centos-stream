# Build qemu Centos-stream images

Build minimal CentOS-Stream `qcow2` images that can be used in _kvm_ or _xen_.

```bash
PACKER_LOG=1 packer build main.json
```

In another terminal, watch the output installation:

```bash
mkfifo /tmp/qemu-serial.in /tmp/qemu-serial.out
cat /tmp/qemu-serial.out

```

