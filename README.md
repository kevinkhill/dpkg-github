# dpkg-github
Simple script to download and install .deb files from github users

```
Examples:
 $ dpkg-github -v sharkdp/fd
 7.2.0

 $ dpkg-github -l sharkdp/fd
 https://github.com/sharkdp/fd/releases/download/v7.2.0/fd-musl_7.2.0_amd64.deb
 https://github.com/sharkdp/fd/releases/download/v7.2.0/fd-musl_7.2.0_i386.deb
 https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_amd64.deb
 https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_i386.deb

 $ dpkg-github -u sharkdp/fd
 https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_amd64.deb

 $ dpkg-github -a i386 -u sharkdp/fd
 > https://github.com/sharkdp/fd/releases/download/v7.2.0/fd_7.2.0_i386.deb

 $ dpkg-github -i sharkdp/fd
 dpkg-github: Fetching .deb for sharkdp/fd
 dpkg-github: Querying Github for latest release.
 dpkg-github: Found fd_7.2.0_amd64.deb
 ...
 # Downloads and then runs \$(sudo dpkg -i <.deb>) to install
 ```

