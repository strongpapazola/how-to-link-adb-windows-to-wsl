# how-to-link-adb-windows-to-wsl
how to link adb windows to wsl



we can do it more easily on WSL2

if we installed adb in windows and the path is /mnt/c/platform-tools/adb.exe

the WSL2 adb install at /usr/bin/adb

let change adb to adb_bk and set ln -s to link adb.exe

sudo mv /usr/bin/adb /usr/bin/adb_bk

- U need to find your adb path on windows
sudo ln -s /mnt/c/platform-tools/adb.exe /usr/bin/adb

now we can use adb and work at bash script

try it
