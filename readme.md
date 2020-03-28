# ZSTD sample files
This repository contains some Zstandard (or zstd) sample files you can use to test out your code or binaries  
You need git lfs support to clone this repository

## decodecorpus
Folder contains 1000 test files generated with zstd's decodecorpus tool.  

Filenames have following pattern:
* z000000 - z000999 (uncompressed binary data files)
* z000000.zst - z000999.zst (compressed ZSTD files)

Largest file is 1 046 445 bytes (*z000305*)  
There are multiple files with 0 byte size

They were generated with following command
```
./decodecorpus -ptestfiles -otestfiles -n1000 -s1337
```