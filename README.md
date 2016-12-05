iscsi-restore
=============

A minimal script that uses pc-sysinstall to preform a full restore of an iSCSI
backup created using lpreserver.

## Usage

```
iscsi-restore <GELI ISCSI FILE> [--mount-only]
  --mount-only      Mounts the remote iSCSI device and imports the GELI encrypted zpool so individal files can be pulled from a snapshot
```

## Dependencies
 - pc-sysinstall patches located in [yupyupp/pc-sysinstall:iscsirestore](https://github.com/yupyupp/pc-sysinstall/tree/iscsirestore)
 - An iSCSI backup created by [yupyupp/lpreserver:openssl](https://github.com/yupyupp/lpreserver/tree/openssl)

## Default locations
 - A copy of ```pc-sysinstall``` to be located at ```/root/pc-sysinstall```
 - A pc-sysinstall config file located in ```/server-build/conf/ME```
