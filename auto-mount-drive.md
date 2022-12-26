
To get file system UUID
```bash
sudo blkid
```

Make mount point
```bash
sudo mkdir /mnt/driveName
```

Register the mounted volume to fstab (file system table)
_example of ext4_
```bash
UUID=uuid  /mnt/driveName  ext4  defaults  0  2
```

_example of ntfs_
```bash
UUID=uuid  /mnt/driveName  ntfs  defaults   0   2
```

_example of btrfs_
```bash
UUID=uuid  /mnt/driveName   btrfs   defaults  0   2
```

_source: https://www.linuxbabe.com/desktop-linux/how-to-automount-file-systems-on-linux_
