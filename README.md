# dpkg-github
Simple script to download and install .deb files from github users

## Install Debs
`$ dpkg-github -i sharkdp/fd`
Downloads latest .deb and runs `sudo dpkg -i <.deb>` to install

## Options:

### Version
```
$ dpkg-github -v sharkdp/fd
7.2.0
```

### List
```
$ dpkg-github -l sharkdp/fd
https://github.com/sharkdp/fd/releases/download/v7.2.0/fd-musl_7.2.0_amd64.deb
https://github.com/sharkdp/fd/releases/download/v7.2.0/fd-musl_7.2.0_i386.deb
https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_amd64.deb
https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_i386.deb
```

### Latest UR
```
$ dpkg-github -u sharkdp/fd
https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_amd64.deb
```

### Change Architecture
```
$ dpkg-github -a i386 -u sharkdp/fd
> https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_i386.deb
```



