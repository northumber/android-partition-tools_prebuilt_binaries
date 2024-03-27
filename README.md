# Android partition tools prebuilt binaries

### Description
- Android partition tools prebuild binaries for editing the super.img
- Binaries built for Linux operating system, I did not test on Windows yet, but works with Ubuntu WSL integration.
- Binaries structure: ARM - armeabi-v7a, arm64-v8a
- Comprehend lpadd, lpdump, lpflash, lpmake, lpunpack

More info on partition tools here: https://android.googlesource.com/platform/system/extras/+/master/partition_tools/

### Usage

Download the latest release from this repository or clone it, open a linux shell and:

```
chmod +x <binary_name>
./<binary_name
```

**To run on X86_64 computers**, download the package "qemu-user":
```
apt install qemu-user
```
and run:
```
qemu-aarch64 <binary_name>
```
(in this case the arm64-v8a binaries are used)
