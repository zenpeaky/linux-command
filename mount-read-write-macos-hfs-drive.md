## Mount and enable write permission on Apple HFS disk

Install hfsprogs
```bash
yay -Sy hfsprogs
```

create folder with write permission for mount point (devcomp is my username)
```bash
sudo mkdir /run/media/devcomp/Media && sudo chmod -R 777 /run/media/devcomp/Media
```

Mount using hfsprogs (sdXY is partition with its number)
```bash
sudo mount -t hfsplus -o force,rw /dev/sdXY /run/media/devcomp/Media
```
_source : https://superuser.com/questions/84446/how-to-mount-a-hfs-partition-in-ubuntu-as-read-write_
