# jupyter

Jupyter on ubuntu: How to install


1) update your OS packages
```
ubuntu@enagamine:~$ sudo apt update
Hit:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal InRelease
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports InRelease [101 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 Packages [8628 kB]
Get:5 http://security.ubuntu.com/ubuntu focal-security InRelease [109 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe Translation-en [5124 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 c-n-f Metadata [265 kB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse amd64 Packages [144 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse Translation-en [104 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse amd64 c-n-f Metadata [9136 B]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [670 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main Translation-en [167 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 c-n-f Metadata [11.1 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [95.6 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/restricted Translation-en [14.8 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [696 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe Translation-en [136 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 c-n-f Metadata [13.2 kB]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 Packages [19.9 kB]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse Translation-en [4668 B]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 c-n-f Metadata [552 B]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/main amd64 c-n-f Metadata [112 B]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/restricted amd64 c-n-f Metadata [116 B]
Get:24 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe amd64 Packages [5304 B]
Get:25 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe Translation-en [1448 B]
Get:26 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe amd64 c-n-f Metadata [224 B]
Get:27 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/multiverse amd64 c-n-f Metadata [116 B]
Get:28 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [372 kB]
Get:29 http://security.ubuntu.com/ubuntu focal-security/main Translation-en [85.1 kB]
Get:30 http://security.ubuntu.com/ubuntu focal-security/main amd64 c-n-f Metadata [5428 B]
Get:31 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [69.9 kB]
Get:32 http://security.ubuntu.com/ubuntu focal-security/restricted Translation-en [11.4 kB]
Get:33 http://security.ubuntu.com/ubuntu focal-security/universe amd64 Packages [519 kB]
Get:34 http://security.ubuntu.com/ubuntu focal-security/universe Translation-en [68.0 kB]
Get:35 http://security.ubuntu.com/ubuntu focal-security/universe amd64 c-n-f Metadata [9364 B]
Get:36 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 Packages [1256 B]
Get:37 http://security.ubuntu.com/ubuntu focal-security/multiverse Translation-en [540 B]
Get:38 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 c-n-f Metadata [116 B]
Fetched 17.6 MB in 3s (6502 kB/s)
Reading package lists... Done
Building dependency tree
Reading state information... Done
45 packages can be upgraded. Run 'apt list --upgradable' to see them.
```

2) install python, pip and dependent packages.

```
ubuntu@enagamine:~$ sudo apt install python3-pip python3-dev
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
  binutils binutils-common binutils-x86-64-linux-gnu build-essential cpp cpp-9 dpkg-dev fakeroot g++ g++-9 gcc gcc-9 gcc-9-base libalgorithm-diff-perl
  libalgorithm-diff-xs-perl libalgorithm-merge-perl libasan5 libatomic1 libbinutils libc-dev-bin libc6-dev libcc1-0 libcrypt-dev libctf-nobfd0 libctf0
  libdpkg-perl libexpat1-dev libfakeroot libfile-fcntllock-perl libgcc-9-dev libgomp1 libisl22 libitm1 liblsan0 libmpc3 libpython3-dev libpython3.8-dev
  libquadmath0 libstdc++-9-dev libtsan0 libubsan1 linux-libc-dev make manpages-dev python-pip-whl python3-wheel python3.8-dev zlib1g zlib1g-dev
Suggested packages:
  binutils-doc cpp-doc gcc-9-locales debian-keyring g++-multilib g++-9-multilib gcc-9-doc gcc-multilib autoconf automake libtool flex bison gdb gcc-doc
  gcc-9-multilib glibc-doc bzr libstdc++-9-doc make-doc
The following NEW packages will be installed:
  binutils binutils-common binutils-x86-64-linux-gnu build-essential cpp cpp-9 dpkg-dev fakeroot g++ g++-9 gcc gcc-9 gcc-9-base libalgorithm-diff-perl
  libalgorithm-diff-xs-perl libalgorithm-merge-perl libasan5 libatomic1 libbinutils libc-dev-bin libc6-dev libcc1-0 libcrypt-dev libctf-nobfd0 libctf0
  libdpkg-perl libexpat1-dev libfakeroot libfile-fcntllock-perl libgcc-9-dev libgomp1 libisl22 libitm1 liblsan0 libmpc3 libpython3-dev libpython3.8-dev
  libquadmath0 libstdc++-9-dev libtsan0 libubsan1 linux-libc-dev make manpages-dev python-pip-whl python3-dev python3-pip python3-wheel python3.8-dev zlib1g-dev
The following packages will be upgraded:
  zlib1g
1 upgraded, 50 newly installed, 0 to remove and 44 not upgraded.
Need to get 46.8 MB of archives.
After this operation, 200 MB of additional disk space will be used.
Do you want to continue? [Y/n] yes
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 zlib1g amd64 1:1.2.11.dfsg-2ubuntu1.2 [53.6 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 binutils-common amd64 2.34-6ubuntu1 [207 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libbinutils amd64 2.34-6ubuntu1 [474 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libctf-nobfd0 amd64 2.34-6ubuntu1 [47.0 kB]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libctf0 amd64 2.34-6ubuntu1 [46.6 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 binutils-x86-64-linux-gnu amd64 2.34-6ubuntu1 [1614 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 binutils amd64 2.34-6ubuntu1 [3376 B]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libc-dev-bin amd64 2.31-0ubuntu9.1 [71.7 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 linux-libc-dev amd64 5.4.0-54.60 [1101 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libcrypt-dev amd64 1:4.4.10-10ubuntu4 [104 kB]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libc6-dev amd64 2.31-0ubuntu9.1 [2519 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 gcc-9-base amd64 9.3.0-17ubuntu1~20.04 [19.1 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libisl22 amd64 0.22.1-1 [592 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libmpc3 amd64 1.1.0-1 [40.8 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 cpp-9 amd64 9.3.0-17ubuntu1~20.04 [7494 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 cpp amd64 4:9.3.0-1ubuntu2 [27.6 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libcc1-0 amd64 10.2.0-5ubuntu1~20.04 [41.1 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libgomp1 amd64 10.2.0-5ubuntu1~20.04 [102 kB]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libitm1 amd64 10.2.0-5ubuntu1~20.04 [26.4 kB]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libatomic1 amd64 10.2.0-5ubuntu1~20.04 [9300 B]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libasan5 amd64 9.3.0-17ubuntu1~20.04 [394 kB]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 liblsan0 amd64 10.2.0-5ubuntu1~20.04 [144 kB]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libtsan0 amd64 10.2.0-5ubuntu1~20.04 [320 kB]
Get:24 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libubsan1 amd64 10.2.0-5ubuntu1~20.04 [136 kB]
Get:25 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libquadmath0 amd64 10.2.0-5ubuntu1~20.04 [146 kB]
Get:26 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libgcc-9-dev amd64 9.3.0-17ubuntu1~20.04 [2360 kB]
Get:27 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 gcc-9 amd64 9.3.0-17ubuntu1~20.04 [8241 kB]
Get:28 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 gcc amd64 4:9.3.0-1ubuntu2 [5208 B]
Get:29 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libstdc++-9-dev amd64 9.3.0-17ubuntu1~20.04 [1714 kB]
Get:30 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 g++-9 amd64 9.3.0-17ubuntu1~20.04 [8405 kB]
Get:31 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 g++ amd64 4:9.3.0-1ubuntu2 [1604 B]
Get:32 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 make amd64 4.2.1-1.2 [162 kB]
Get:33 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libdpkg-perl all 1.19.7ubuntu3 [230 kB]
Get:34 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 dpkg-dev all 1.19.7ubuntu3 [679 kB]
Get:35 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 build-essential amd64 12.8ubuntu1.1 [4664 B]
Get:36 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libfakeroot amd64 1.24-1 [25.7 kB]
Get:37 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 fakeroot amd64 1.24-1 [62.6 kB]
Get:38 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libalgorithm-diff-perl all 1.19.03-2 [46.6 kB]
Get:39 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libalgorithm-diff-xs-perl amd64 0.04-6 [11.3 kB]
Get:40 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libalgorithm-merge-perl all 0.08-3 [12.0 kB]
Get:41 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libexpat1-dev amd64 2.2.9-1build1 [116 kB]
Get:42 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libfile-fcntllock-perl amd64 0.22-3build4 [33.1 kB]
Get:43 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libpython3.8-dev amd64 3.8.5-1~20.04 [3941 kB]
Get:44 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libpython3-dev amd64 3.8.2-0ubuntu2 [7236 B]
Get:45 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 manpages-dev all 5.05-1 [2266 kB]
Get:46 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 python-pip-whl all 20.0.2-5ubuntu1.1 [1799 kB]
Get:47 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 zlib1g-dev amd64 1:1.2.11.dfsg-2ubuntu1.2 [155 kB]
Get:48 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 python3.8-dev amd64 3.8.5-1~20.04 [514 kB]
Get:49 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 python3-dev amd64 3.8.2-0ubuntu2 [1212 B]
Get:50 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 python3-wheel all 0.34.2-1 [23.8 kB]
Get:51 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 python3-pip all 20.0.2-5ubuntu1.1 [230 kB]
Fetched 46.8 MB in 1s (54.1 MB/s)
Extracting templates from packages: 100%
(Reading database ... 59940 files and directories currently installed.)
Preparing to unpack .../zlib1g_1%3a1.2.11.dfsg-2ubuntu1.2_amd64.deb ...
Unpacking zlib1g:amd64 (1:1.2.11.dfsg-2ubuntu1.2) over (1:1.2.11.dfsg-2ubuntu1.1) ...
Setting up zlib1g:amd64 (1:1.2.11.dfsg-2ubuntu1.2) ...
Selecting previously unselected package binutils-common:amd64.
(Reading database ... 59940 files and directories currently installed.)
Preparing to unpack .../00-binutils-common_2.34-6ubuntu1_amd64.deb ...
Unpacking binutils-common:amd64 (2.34-6ubuntu1) ...
Selecting previously unselected package libbinutils:amd64.
Preparing to unpack .../01-libbinutils_2.34-6ubuntu1_amd64.deb ...
Unpacking libbinutils:amd64 (2.34-6ubuntu1) ...
Selecting previously unselected package libctf-nobfd0:amd64.
Preparing to unpack .../02-libctf-nobfd0_2.34-6ubuntu1_amd64.deb ...
Unpacking libctf-nobfd0:amd64 (2.34-6ubuntu1) ...
Selecting previously unselected package libctf0:amd64.
Preparing to unpack .../03-libctf0_2.34-6ubuntu1_amd64.deb ...
Unpacking libctf0:amd64 (2.34-6ubuntu1) ...
Selecting previously unselected package binutils-x86-64-linux-gnu.
Preparing to unpack .../04-binutils-x86-64-linux-gnu_2.34-6ubuntu1_amd64.deb ...
Unpacking binutils-x86-64-linux-gnu (2.34-6ubuntu1) ...
Selecting previously unselected package binutils.
Preparing to unpack .../05-binutils_2.34-6ubuntu1_amd64.deb ...
Unpacking binutils (2.34-6ubuntu1) ...
Selecting previously unselected package libc-dev-bin.
Preparing to unpack .../06-libc-dev-bin_2.31-0ubuntu9.1_amd64.deb ...
Unpacking libc-dev-bin (2.31-0ubuntu9.1) ...
Selecting previously unselected package linux-libc-dev:amd64.
Preparing to unpack .../07-linux-libc-dev_5.4.0-54.60_amd64.deb ...
Unpacking linux-libc-dev:amd64 (5.4.0-54.60) ...
Selecting previously unselected package libcrypt-dev:amd64.
Preparing to unpack .../08-libcrypt-dev_1%3a4.4.10-10ubuntu4_amd64.deb ...
Unpacking libcrypt-dev:amd64 (1:4.4.10-10ubuntu4) ...
Selecting previously unselected package libc6-dev:amd64.
Preparing to unpack .../09-libc6-dev_2.31-0ubuntu9.1_amd64.deb ...
Unpacking libc6-dev:amd64 (2.31-0ubuntu9.1) ...
Selecting previously unselected package gcc-9-base:amd64.
Preparing to unpack .../10-gcc-9-base_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking gcc-9-base:amd64 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package libisl22:amd64.
Preparing to unpack .../11-libisl22_0.22.1-1_amd64.deb ...
Unpacking libisl22:amd64 (0.22.1-1) ...
Selecting previously unselected package libmpc3:amd64.
Preparing to unpack .../12-libmpc3_1.1.0-1_amd64.deb ...
Unpacking libmpc3:amd64 (1.1.0-1) ...
Selecting previously unselected package cpp-9.
Preparing to unpack .../13-cpp-9_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking cpp-9 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package cpp.
Preparing to unpack .../14-cpp_4%3a9.3.0-1ubuntu2_amd64.deb ...
Unpacking cpp (4:9.3.0-1ubuntu2) ...
Selecting previously unselected package libcc1-0:amd64.
Preparing to unpack .../15-libcc1-0_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libcc1-0:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libgomp1:amd64.
Preparing to unpack .../16-libgomp1_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libgomp1:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libitm1:amd64.
Preparing to unpack .../17-libitm1_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libitm1:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libatomic1:amd64.
Preparing to unpack .../18-libatomic1_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libatomic1:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libasan5:amd64.
Preparing to unpack .../19-libasan5_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking libasan5:amd64 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package liblsan0:amd64.
Preparing to unpack .../20-liblsan0_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking liblsan0:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libtsan0:amd64.
Preparing to unpack .../21-libtsan0_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libtsan0:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libubsan1:amd64.
Preparing to unpack .../22-libubsan1_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libubsan1:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libquadmath0:amd64.
Preparing to unpack .../23-libquadmath0_10.2.0-5ubuntu1~20.04_amd64.deb ...
Unpacking libquadmath0:amd64 (10.2.0-5ubuntu1~20.04) ...
Selecting previously unselected package libgcc-9-dev:amd64.
Preparing to unpack .../24-libgcc-9-dev_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking libgcc-9-dev:amd64 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package gcc-9.
Preparing to unpack .../25-gcc-9_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking gcc-9 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package gcc.
Preparing to unpack .../26-gcc_4%3a9.3.0-1ubuntu2_amd64.deb ...
Unpacking gcc (4:9.3.0-1ubuntu2) ...
Selecting previously unselected package libstdc++-9-dev:amd64.
Preparing to unpack .../27-libstdc++-9-dev_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking libstdc++-9-dev:amd64 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package g++-9.
Preparing to unpack .../28-g++-9_9.3.0-17ubuntu1~20.04_amd64.deb ...
Unpacking g++-9 (9.3.0-17ubuntu1~20.04) ...
Selecting previously unselected package g++.
Preparing to unpack .../29-g++_4%3a9.3.0-1ubuntu2_amd64.deb ...
Unpacking g++ (4:9.3.0-1ubuntu2) ...
Selecting previously unselected package make.
Preparing to unpack .../30-make_4.2.1-1.2_amd64.deb ...
Unpacking make (4.2.1-1.2) ...
Selecting previously unselected package libdpkg-perl.
Preparing to unpack .../31-libdpkg-perl_1.19.7ubuntu3_all.deb ...
Unpacking libdpkg-perl (1.19.7ubuntu3) ...
Selecting previously unselected package dpkg-dev.
Preparing to unpack .../32-dpkg-dev_1.19.7ubuntu3_all.deb ...
Unpacking dpkg-dev (1.19.7ubuntu3) ...
Selecting previously unselected package build-essential.
Preparing to unpack .../33-build-essential_12.8ubuntu1.1_amd64.deb ...
Unpacking build-essential (12.8ubuntu1.1) ...
Selecting previously unselected package libfakeroot:amd64.
Preparing to unpack .../34-libfakeroot_1.24-1_amd64.deb ...
Unpacking libfakeroot:amd64 (1.24-1) ...
Selecting previously unselected package fakeroot.
Preparing to unpack .../35-fakeroot_1.24-1_amd64.deb ...
Unpacking fakeroot (1.24-1) ...
Selecting previously unselected package libalgorithm-diff-perl.
Preparing to unpack .../36-libalgorithm-diff-perl_1.19.03-2_all.deb ...
Unpacking libalgorithm-diff-perl (1.19.03-2) ...
Selecting previously unselected package libalgorithm-diff-xs-perl.
Preparing to unpack .../37-libalgorithm-diff-xs-perl_0.04-6_amd64.deb ...
Unpacking libalgorithm-diff-xs-perl (0.04-6) ...
Selecting previously unselected package libalgorithm-merge-perl.
Preparing to unpack .../38-libalgorithm-merge-perl_0.08-3_all.deb ...
Unpacking libalgorithm-merge-perl (0.08-3) ...
Selecting previously unselected package libexpat1-dev:amd64.
Preparing to unpack .../39-libexpat1-dev_2.2.9-1build1_amd64.deb ...
Unpacking libexpat1-dev:amd64 (2.2.9-1build1) ...
Selecting previously unselected package libfile-fcntllock-perl.
Preparing to unpack .../40-libfile-fcntllock-perl_0.22-3build4_amd64.deb ...
Unpacking libfile-fcntllock-perl (0.22-3build4) ...
Selecting previously unselected package libpython3.8-dev:amd64.
Preparing to unpack .../41-libpython3.8-dev_3.8.5-1~20.04_amd64.deb ...
Unpacking libpython3.8-dev:amd64 (3.8.5-1~20.04) ...
Selecting previously unselected package libpython3-dev:amd64.
Preparing to unpack .../42-libpython3-dev_3.8.2-0ubuntu2_amd64.deb ...
Unpacking libpython3-dev:amd64 (3.8.2-0ubuntu2) ...
Selecting previously unselected package manpages-dev.
Preparing to unpack .../43-manpages-dev_5.05-1_all.deb ...
Unpacking manpages-dev (5.05-1) ...
Selecting previously unselected package python-pip-whl.
Preparing to unpack .../44-python-pip-whl_20.0.2-5ubuntu1.1_all.deb ...
Unpacking python-pip-whl (20.0.2-5ubuntu1.1) ...
Selecting previously unselected package zlib1g-dev:amd64.
Preparing to unpack .../45-zlib1g-dev_1%3a1.2.11.dfsg-2ubuntu1.2_amd64.deb ...
Unpacking zlib1g-dev:amd64 (1:1.2.11.dfsg-2ubuntu1.2) ...
Selecting previously unselected package python3.8-dev.
Preparing to unpack .../46-python3.8-dev_3.8.5-1~20.04_amd64.deb ...
Unpacking python3.8-dev (3.8.5-1~20.04) ...
Selecting previously unselected package python3-dev.
Preparing to unpack .../47-python3-dev_3.8.2-0ubuntu2_amd64.deb ...
Unpacking python3-dev (3.8.2-0ubuntu2) ...
Selecting previously unselected package python3-wheel.
Preparing to unpack .../48-python3-wheel_0.34.2-1_all.deb ...
Unpacking python3-wheel (0.34.2-1) ...
Selecting previously unselected package python3-pip.
Preparing to unpack .../49-python3-pip_20.0.2-5ubuntu1.1_all.deb ...
Unpacking python3-pip (20.0.2-5ubuntu1.1) ...
Setting up manpages-dev (5.05-1) ...
Setting up libfile-fcntllock-perl (0.22-3build4) ...
Setting up libalgorithm-diff-perl (1.19.03-2) ...
Setting up binutils-common:amd64 (2.34-6ubuntu1) ...
Setting up linux-libc-dev:amd64 (5.4.0-54.60) ...
Setting up libctf-nobfd0:amd64 (2.34-6ubuntu1) ...
Setting up libgomp1:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up python3-wheel (0.34.2-1) ...
Setting up libfakeroot:amd64 (1.24-1) ...
Setting up fakeroot (1.24-1) ...
update-alternatives: using /usr/bin/fakeroot-sysv to provide /usr/bin/fakeroot (fakeroot) in auto mode
Setting up make (4.2.1-1.2) ...
Setting up libquadmath0:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up libmpc3:amd64 (1.1.0-1) ...
Setting up libatomic1:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up libdpkg-perl (1.19.7ubuntu3) ...
Setting up libubsan1:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up libcrypt-dev:amd64 (1:4.4.10-10ubuntu4) ...
Setting up libisl22:amd64 (0.22.1-1) ...
Setting up python-pip-whl (20.0.2-5ubuntu1.1) ...
Setting up libbinutils:amd64 (2.34-6ubuntu1) ...
Setting up libc-dev-bin (2.31-0ubuntu9.1) ...
Setting up libalgorithm-diff-xs-perl (0.04-6) ...
Setting up libcc1-0:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up liblsan0:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up libitm1:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up gcc-9-base:amd64 (9.3.0-17ubuntu1~20.04) ...
Setting up libalgorithm-merge-perl (0.08-3) ...
Setting up libtsan0:amd64 (10.2.0-5ubuntu1~20.04) ...
Setting up libctf0:amd64 (2.34-6ubuntu1) ...
Setting up libasan5:amd64 (9.3.0-17ubuntu1~20.04) ...
Setting up python3-pip (20.0.2-5ubuntu1.1) ...
Setting up cpp-9 (9.3.0-17ubuntu1~20.04) ...
Setting up libc6-dev:amd64 (2.31-0ubuntu9.1) ...
Setting up binutils-x86-64-linux-gnu (2.34-6ubuntu1) ...
Setting up binutils (2.34-6ubuntu1) ...
Setting up dpkg-dev (1.19.7ubuntu3) ...
Setting up libgcc-9-dev:amd64 (9.3.0-17ubuntu1~20.04) ...
Setting up libexpat1-dev:amd64 (2.2.9-1build1) ...
Setting up libpython3.8-dev:amd64 (3.8.5-1~20.04) ...
Setting up zlib1g-dev:amd64 (1:1.2.11.dfsg-2ubuntu1.2) ...
Setting up cpp (4:9.3.0-1ubuntu2) ...
Setting up gcc-9 (9.3.0-17ubuntu1~20.04) ...
Setting up libpython3-dev:amd64 (3.8.2-0ubuntu2) ...
Setting up libstdc++-9-dev:amd64 (9.3.0-17ubuntu1~20.04) ...
Setting up gcc (4:9.3.0-1ubuntu2) ...
Setting up g++-9 (9.3.0-17ubuntu1~20.04) ...
Setting up python3.8-dev (3.8.5-1~20.04) ...
Setting up g++ (4:9.3.0-1ubuntu2) ...
update-alternatives: using /usr/bin/g++ to provide /usr/bin/c++ (c++) in auto mode
Setting up build-essential (12.8ubuntu1.1) ...
Setting up python3-dev (3.8.2-0ubuntu2) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.1) ...
```
3) upgrade pip:

```
ubuntu@enagamine:~$ sudo -H pip3 install --upgrade pip
Collecting pip
  Downloading pip-20.2.4-py2.py3-none-any.whl (1.5 MB)
     |████████████████████████████████| 1.5 MB 17.3 MB/s
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 20.0.2
    Not uninstalling pip at /usr/lib/python3/dist-packages, outside environment /usr
    Can't uninstall 'pip'. No files were found to uninstall.
Successfully installed pip-20.2.4
```

4) Create a virtual environment

```
ubuntu@enagamine:~$ sudo -H pip3 install virtualenv
Collecting virtualenv
  Downloading virtualenv-20.2.1-py2.py3-none-any.whl (4.9 MB)
     |████████████████████████████████| 4.9 MB 16.1 MB/s
Collecting distlib<1,>=0.3.1
  Downloading distlib-0.3.1-py2.py3-none-any.whl (335 kB)
     |████████████████████████████████| 335 kB 59.0 MB/s
Collecting appdirs<2,>=1.4.3
  Downloading appdirs-1.4.4-py2.py3-none-any.whl (9.6 kB)
Requirement already satisfied: six<2,>=1.9.0 in /usr/lib/python3/dist-packages (from virtualenv) (1.14.0)
Collecting filelock<4,>=3.0.0
  Downloading filelock-3.0.12-py3-none-any.whl (7.6 kB)
Installing collected packages: distlib, appdirs, filelock, virtualenv
Successfully installed appdirs-1.4.4 distlib-0.3.1 filelock-3.0.12 virtualenv-20.2.1
```

5) Install Jupyter

```
ubuntu@enagamine:~$ pip install jupyter
Defaulting to user installation because normal site-packages is not writeable
Collecting jupyter
  Downloading jupyter-1.0.0-py2.py3-none-any.whl (2.7 kB)
Collecting ipywidgets
  Downloading ipywidgets-7.5.1-py2.py3-none-any.whl (121 kB)
     |████████████████████████████████| 121 kB 22.5 MB/s
Collecting nbconvert
  Downloading nbconvert-6.0.7-py3-none-any.whl (552 kB)
     |████████████████████████████████| 552 kB 49.9 MB/s
Collecting jupyter-console
  Downloading jupyter_console-6.2.0-py3-none-any.whl (22 kB)
Collecting qtconsole
  Downloading qtconsole-5.0.0-py3-none-any.whl (118 kB)
     |████████████████████████████████| 118 kB 70.4 MB/s
Collecting notebook
  Downloading notebook-6.1.5-py3-none-any.whl (9.5 MB)
     |████████████████████████████████| 9.5 MB 67.2 MB/s
Collecting ipykernel
  Downloading ipykernel-5.3.4-py3-none-any.whl (120 kB)
     |████████████████████████████████| 120 kB 72.3 MB/s
Collecting widgetsnbextension~=3.5.0
  Downloading widgetsnbextension-3.5.1-py2.py3-none-any.whl (2.2 MB)
     |████████████████████████████████| 2.2 MB 67.0 MB/s
Collecting traitlets>=4.3.1
  Downloading traitlets-5.0.5-py3-none-any.whl (100 kB)
     |████████████████████████████████| 100 kB 16.8 MB/s
Collecting nbformat>=4.2.0
  Downloading nbformat-5.0.8-py3-none-any.whl (172 kB)
     |████████████████████████████████| 172 kB 72.0 MB/s
Collecting ipython>=4.0.0; python_version >= "3.3"
  Downloading ipython-7.19.0-py3-none-any.whl (784 kB)
     |████████████████████████████████| 784 kB 64.9 MB/s
Requirement already satisfied: jinja2>=2.4 in /usr/lib/python3/dist-packages (from nbconvert->jupyter) (2.10.1)
Collecting mistune<2,>=0.8.1
  Downloading mistune-0.8.4-py2.py3-none-any.whl (16 kB)
Collecting jupyter-core
  Downloading jupyter_core-4.7.0-py3-none-any.whl (82 kB)
     |████████████████████████████████| 82 kB 2.1 MB/s
Collecting jupyterlab-pygments
  Downloading jupyterlab_pygments-0.1.2-py2.py3-none-any.whl (4.6 kB)
Collecting pygments>=2.4.1
  Downloading Pygments-2.7.2-py3-none-any.whl (948 kB)
     |████████████████████████████████| 948 kB 61.7 MB/s
Collecting defusedxml
  Downloading defusedxml-0.6.0-py2.py3-none-any.whl (23 kB)
Collecting pandocfilters>=1.4.1
  Downloading pandocfilters-1.4.3.tar.gz (16 kB)
Collecting nbclient<0.6.0,>=0.5.0
  Downloading nbclient-0.5.1-py3-none-any.whl (65 kB)
     |████████████████████████████████| 65 kB 6.8 MB/s
Requirement already satisfied: entrypoints>=0.2.2 in /usr/lib/python3/dist-packages (from nbconvert->jupyter) (0.3)
Collecting testpath
  Downloading testpath-0.4.4-py2.py3-none-any.whl (163 kB)
     |████████████████████████████████| 163 kB 65.8 MB/s
Collecting bleach
  Downloading bleach-3.2.1-py2.py3-none-any.whl (145 kB)
     |████████████████████████████████| 145 kB 60.2 MB/s
Collecting jupyter-client
  Downloading jupyter_client-6.1.7-py3-none-any.whl (108 kB)
     |████████████████████████████████| 108 kB 63.1 MB/s
Collecting prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0
  Downloading prompt_toolkit-3.0.8-py3-none-any.whl (355 kB)
     |████████████████████████████████| 355 kB 61.8 MB/s
Collecting ipython-genutils
  Downloading ipython_genutils-0.2.0-py2.py3-none-any.whl (26 kB)
Collecting pyzmq>=17.1
  Downloading pyzmq-20.0.0-cp38-cp38-manylinux1_x86_64.whl (1.1 MB)
     |████████████████████████████████| 1.1 MB 68.4 MB/s
Collecting qtpy
  Downloading QtPy-1.9.0-py2.py3-none-any.whl (54 kB)
     |████████████████████████████████| 54 kB 4.9 MB/s
Collecting terminado>=0.8.3
  Downloading terminado-0.9.1-py3-none-any.whl (13 kB)
Collecting argon2-cffi
  Downloading argon2_cffi-20.1.0-cp35-abi3-manylinux1_x86_64.whl (97 kB)
     |████████████████████████████████| 97 kB 13.4 MB/s
Collecting Send2Trash
  Downloading Send2Trash-1.5.0-py3-none-any.whl (12 kB)
Collecting tornado>=5.0
  Downloading tornado-6.1-cp38-cp38-manylinux2010_x86_64.whl (427 kB)
     |████████████████████████████████| 427 kB 70.1 MB/s
Collecting prometheus-client
  Downloading prometheus_client-0.9.0-py2.py3-none-any.whl (53 kB)
     |████████████████████████████████| 53 kB 4.8 MB/s
Requirement already satisfied: jsonschema!=2.5.0,>=2.4 in /usr/lib/python3/dist-packages (from nbformat>=4.2.0->ipywidgets->jupyter) (3.2.0)
Requirement already satisfied: pexpect>4.3; sys_platform != "win32" in /usr/lib/python3/dist-packages (from ipython>=4.0.0; python_version >= "3.3"->ipywidgets->jupyter) (4.6.0)
Requirement already satisfied: setuptools>=18.5 in /usr/lib/python3/dist-packages (from ipython>=4.0.0; python_version >= "3.3"->ipywidgets->jupyter) (45.2.0)
Collecting pickleshare
  Downloading pickleshare-0.7.5-py2.py3-none-any.whl (6.9 kB)
Collecting decorator
  Downloading decorator-4.4.2-py2.py3-none-any.whl (9.2 kB)
Collecting backcall
  Downloading backcall-0.2.0-py2.py3-none-any.whl (11 kB)
Collecting jedi>=0.10
  Downloading jedi-0.17.2-py2.py3-none-any.whl (1.4 MB)
     |████████████████████████████████| 1.4 MB 68.8 MB/s
Collecting async-generator
  Downloading async_generator-1.10-py3-none-any.whl (18 kB)
Collecting nest-asyncio
  Downloading nest_asyncio-1.4.3-py3-none-any.whl (5.3 kB)
Requirement already satisfied: six>=1.9.0 in /usr/lib/python3/dist-packages (from bleach->nbconvert->jupyter) (1.14.0)
Collecting packaging
  Downloading packaging-20.4-py2.py3-none-any.whl (37 kB)
Collecting webencodings
  Downloading webencodings-0.5.1-py2.py3-none-any.whl (11 kB)
Collecting python-dateutil>=2.1
  Downloading python_dateutil-2.8.1-py2.py3-none-any.whl (227 kB)
     |████████████████████████████████| 227 kB 67.9 MB/s
Collecting wcwidth
  Downloading wcwidth-0.2.5-py2.py3-none-any.whl (30 kB)
Collecting ptyprocess; os_name != "nt"
  Downloading ptyprocess-0.6.0-py2.py3-none-any.whl (39 kB)
Collecting cffi>=1.0.0
  Downloading cffi-1.14.3-cp38-cp38-manylinux1_x86_64.whl (410 kB)
     |████████████████████████████████| 410 kB 69.1 MB/s
Collecting parso<0.8.0,>=0.7.0
  Downloading parso-0.7.1-py2.py3-none-any.whl (109 kB)
     |████████████████████████████████| 109 kB 79.4 MB/s
Collecting pyparsing>=2.0.2
  Downloading pyparsing-2.4.7-py2.py3-none-any.whl (67 kB)
     |████████████████████████████████| 67 kB 11.6 MB/s
Collecting pycparser
  Downloading pycparser-2.20-py2.py3-none-any.whl (112 kB)
     |████████████████████████████████| 112 kB 77.1 MB/s
Building wheels for collected packages: pandocfilters
  Building wheel for pandocfilters (setup.py) ... done
  Created wheel for pandocfilters: filename=pandocfilters-1.4.3-py3-none-any.whl size=7991 sha256=7f9211a120078a7e3983d7edaca842a923cbacd80480203089ed5872426b710f
  Stored in directory: /home/ubuntu/.cache/pip/wheels/fc/39/52/8d6f3cec1cca4ceb44d658427c35711b19d89dbc4914af657f
Successfully built pandocfilters
Installing collected packages: ipython-genutils, traitlets, jupyter-core, python-dateutil, tornado, pyzmq, jupyter-client, ptyprocess, terminado, pycparser, cffi, argon2-cffi, Send2Trash, mistune, pygments, jupyterlab-pygments, defusedxml, nbformat, pandocfilters, async-generator, nest-asyncio, nbclient, testpath, pyparsing, packaging, webencodings, bleach, nbconvert, prometheus-client, wcwidth, prompt-toolkit, pickleshare, decorator, backcall, parso, jedi, ipython, ipykernel, notebook, widgetsnbextension, ipywidgets, jupyter-console, qtpy, qtconsole, jupyter
  WARNING: The scripts jupyter, jupyter-migrate and jupyter-troubleshoot are installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The scripts jupyter-kernel, jupyter-kernelspec and jupyter-run are installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script pygmentize is installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script jupyter-trust is installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script jupyter-nbconvert is installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The scripts iptest, iptest3, ipython and ipython3 are installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The scripts jupyter-bundlerextension, jupyter-nbextension, jupyter-notebook and jupyter-serverextension are installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script jupyter-console is installed in '/home/ubuntu/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
Successfully installed Send2Trash-1.5.0 argon2-cffi-20.1.0 async-generator-1.10 backcall-0.2.0 bleach-3.2.1 cffi-1.14.3 decorator-4.4.2 defusedxml-0.6.0 ipykernel-5.3.4 ipython-7.19.0 ipython-genutils-0.2.0 ipywidgets-7.5.1 jedi-0.17.2 jupyter-1.0.0 jupyter-client-6.1.7 jupyter-console-6.2.0 jupyter-core-4.7.0 jupyterlab-pygments-0.1.2 mistune-0.8.4 nbclient-0.5.1 nbconvert-6.0.7 nbformat-5.0.8 nest-asyncio-1.4.3 notebook-6.1.5 packaging-20.4 pandocfilters-1.4.3 parso-0.7.1 pickleshare-0.7.5 prometheus-client-0.9.0 prompt-toolkit-3.0.8 ptyprocess-0.6.0 pycparser-2.20 pygments-2.7.2 pyparsing-2.4.7 python-dateutil-2.8.1 pyzmq-20.0.0 qtconsole-5.0.0 qtpy-1.9.0 terminado-0.9.1 testpath-0.4.4 tornado-6.1 traitlets-5.0.5 wcwidth-0.2.5 webencodings-0.5.1 widgetsnbextension-3.5.1
```
