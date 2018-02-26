This is toolchain build script for LFS based on SVN book

1. create $LFS directory (/mnt/lfs is default, you can change it in build-properties)
	sudo mkdir -v /mnt/lfs

2. create $LFS/tools and symlink it to root directory (/)
	sudo mkdir -v /mnt/lfs/tools
	sudo ln -sv /mnt/lfs/tools /

3. change perm/owner of /mnt/lfs/tools to your user
	sudo chown -v emmett:emmett /mnt/lfs/tools

4. run ./strap to build the toolchain
	./strap