## This is toolchain build script for LFS based on SVN book
### How to use:

1. Run ./fetch-sources to download all needed sources

       ./fetch-sources
       
2. create $LFS directory (`/mnt/lfs` is default, you can change it in `build-properties`)

       sudo mkdir -v /mnt/lfs

3. create `$LFS/tools` and symlink it to root directory (/)

       sudo mkdir -v /mnt/lfs/tools
       sudo ln -sv /mnt/lfs/tools /

4. change perm/owner of `/mnt/lfs/tools` to your user (change `emmett` to your user)

       sudo chown -v emmett:emmett /mnt/lfs/tools

5. run ./strap to build the toolchain

       ./strap
