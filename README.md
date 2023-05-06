# remastered_tinycore

This is a remastere patch for [TinyCore Linux (CorePlus)](http://tinycorelinux.net/)

In official iso, it contains 2 folders, `boot` and `cde`. `boot` has following directorys and files
```
boot
 |-/isolinux
 | |-f4
 | |-f3
 | |-f2
 | |-menu.c32
 | |-boot.msg
 | |-boot.cat
 | |-isolinux.bin
 | |-f1
 | |-isolinux.cfg
 |-core.gz
 |-vmlinuz
```
`core.gz` cannot be reverse because it is binded by cat:

```bash
cat rootfs.gz modules.gz > core.gz
```

So I don't focus on uploading source code for scrach for now. 

`cde` has following directorys and files. In `optional` directory, there are so many tczs.

```
cde
|-wifi.instlist
|-remaster.instlist
|-xibase.lst
|-xbase.lst
|-xwbase.lst
|-onboot.lst
|-wififirmware.instlist
|-/optional
|-xfbase.lst
|-kmaps.instlist
|-installer.instlist
```

TODO: I don't want to upload binary on this repository but customize so I created script which downloaded all file and replace it or remove it as a patch for original binary.
