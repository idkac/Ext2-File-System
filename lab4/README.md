# Hey! I'm Filing Here

In this lab, I successfully implemented a mountable ext2 file that has a working root directory, lost and found directory, regular file, and symbolic link. 

## Building

Run the following commands

make
./ext2-create

## Running
You can get the file system information run the following command. 
dumpe2fs cs111-base.img

You can also check the file system's is correct
fsck.ext2 cs111-base.img

You can also implement the file system by running
mkdir mnt
sudo mount -o loop cs111-base 

## Cleaning up
If you have loaded a file system, then run teh following commands
sudo umount mnt 
rmdir mnt

make clean

