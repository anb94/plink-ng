# Modified dose2plink

This repo has been forked from https://github.com/chrchang/plink-ng.

Modifications have been made to plink-ng/1.9/dose2plink.c in order to be able to compile with system zlib.

In order to compile plink-ng/1.9/dose2plink.c make sure gcc and zlib is installed on your machine such as:

```
  sudo apt-get install zlib1g-dev
  sudo apt install build-essential
```


in ubuntu.

To compile you can do the following:

```
  cd plink-ng/1.9/
  gcc dose2plink.c -lz -o /path/to/file/dose2plink
```

You can then add dose2plink to your path by adding it to your environment, such as:

```
  export PATH=$PATH:/path/to/file/dose2plink
```