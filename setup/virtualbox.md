Setup Virtualbox
====

- Create directory

```
sudo mkdir /vm
sudo chown master:staff /vm
```

- Download & install Virtualbox
- Install extention pack
- Download & unzip VM: IE11 on Win7

https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/

```
mv ~/Downloads/IE11_Win7 /vm/
```

- Open Virtualbox
- File -> Import Appliance...
- Setting
  - System
    - CPU: 4
    - Base memory: 2GB
  - Ports -> USB 2.0
- Take a snapshot
- Boot
- Disable scheduled defragmentation

### References

- https://sites.google.com/site/easylinuxtipsproject/oldgrub

