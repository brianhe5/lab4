# Hey! I'm Filing Here

In this lab, I successfully implemented the following functions
write_superblock
write_block_group_descriptor_table
write_block_bitmap
write_inode_bitmap
write_inode_table
write_root_dir_block
write_hello_world_file_block

These functions help to create a 1MiB ext2 file system with 2 directories, 1 regular file, and 1 symlink
## Building

To build this program, run "make"

## Running

To create the image of the filesystem (cs111-base.img), run the program "./ext2-create"

Check specifications of the Ext2 file system by running "dumpe2fs cs111-base.img"

Check for errors by running "fsck.ext2 cs111-base.img"

To ls and call the mounted filesystem mnt to show the directories and files in our filesystem, run:
mkdir mnt
sudo mount -o loop cs111-base.img mnt
ls -ain mnt

## Cleaning up

To remove the executables generated from calling make, run "make clean"

To unmount and remove the mounted filesystem, run "sudo umount mnt" and "rmdir mnt"


