# 役に立たなかった参照

# MSYS2

```plaintext
Another option is to install the Linux compatiblity tools from [MSYS2](https://www.msys2.org/).

After installation start the msys64 bit terminal from the start menu and install the
C/C++ compiler toolchain. E.g.:

  pacman -S --noconfirm pacman-mirrors pkg-config
  pacman -S --noconfirm --needed base-devel autoconf automake make libtool git \
    mingw-w64-x86_64-toolchain mingw-w64-x86_64-openssl mingw-w64-x86_64-libtool

This will give you a compilation suite nearly compatible with Unix' standard tools.
```

* MSYS2 をインストール 📖 [MSYS2](https://www.msys2.org/)

Input:  

```shell
pacman -S --noconfirm pacman-mirrors pkg-config
```

Output:  

```plaintext
warning: pacman-mirrors-20221016-1 is up to date -- reinstalling
resolving dependencies...
looking for conflicting packages...

Packages (2) pacman-mirrors-20221016-1  pkgconf-1.9.4-1

Total Download Size:   0.06 MiB
Total Installed Size:  0.30 MiB
Net Upgrade Size:      0.29 MiB

:: Proceed with installation? [Y/n]
:: Retrieving packages...
 pkgconf-1.9.4-1-x86_64           61.6 KiB  33.7 KiB/s 00:02 [###############################] 100%
 pacman-mirrors-20221016-1-any     4.1 KiB  1487   B/s 00:03 [###############################] 100%
 Total (2/2)                      65.7 KiB  18.7 KiB/s 00:04 [###############################] 100%
(2/2) checking keys in keyring                               [###############################] 100%
(2/2) checking package integrity                             [###############################] 100%
(2/2) loading package files                                  [###############################] 100%
(2/2) checking for file conflicts                            [###############################] 100%
(2/2) checking available disk space                          [###############################] 100%
:: Processing package changes...
(1/2) reinstalling pacman-mirrors                            [###############################] 100%
(2/2) installing pkgconf                                     [###############################] 100%

ThreadRipper@DESKTOP-QE5C5HQ UCRT64 ~
```

Input:  

```shell
  pacman -S --noconfirm --needed base-devel autoconf automake make libtool git \
    mingw-w64-x86_64-toolchain mingw-w64-x86_64-openssl mingw-w64-x86_64-libtool
```

Output:  

```plaintext
:: There are 19 members in group mingw-w64-x86_64-toolchain:
:: Repository mingw64
   1) mingw-w64-x86_64-binutils  2) mingw-w64-x86_64-crt-git  3) mingw-w64-x86_64-gcc
   4) mingw-w64-x86_64-gcc-ada  5) mingw-w64-x86_64-gcc-fortran  6) mingw-w64-x86_64-gcc-libgfortran
   7) mingw-w64-x86_64-gcc-libs  8) mingw-w64-x86_64-gcc-objc  9) mingw-w64-x86_64-gdb
   10) mingw-w64-x86_64-gdb-multiarch  11) mingw-w64-x86_64-headers-git  12) mingw-w64-x86_64-libgccjit
   13) mingw-w64-x86_64-libmangle-git  14) mingw-w64-x86_64-libwinpthread-git  15) mingw-w64-x86_64-make
   16) mingw-w64-x86_64-pkgconf  17) mingw-w64-x86_64-tools-git  18) mingw-w64-x86_64-winpthreads-git
   19) mingw-w64-x86_64-winstorecompat-git

Enter a selection (default=all):
resolving dependencies...
looking for conflicting packages...

Packages (104) autoconf2.13-2.13-5  autoconf2.69-2.69-2  autoconf2.71-2.71-1  automake1.11-1.11.6-6
               automake1.12-1.12.6-6  automake1.13-1.13.4-7  automake1.14-1.14.1-6  automake1.15-1.15.1-4
               automake1.16-1.16.5-1  binutils-2.40-1  bison-3.8.2-4  diffstat-1.65-1  diffutils-3.9-1
               dos2unix-7.4.4-1  flex-2.6.4-3  heimdal-7.8.0-3  libcbor-0.10.2-1  libfido2-1.13.0-1
               libltdl-2.4.7-3  m4-1.4.19-2  mingw-w64-x86_64-bzip2-1.0.8-2  mingw-w64-x86_64-expat-2.5.0-1
               mingw-w64-x86_64-gettext-0.21.1-1  mingw-w64-x86_64-gmp-6.2.1-5  mingw-w64-x86_64-isl-0.25-1
               mingw-w64-x86_64-libffi-3.4.4-1  mingw-w64-x86_64-libiconv-1.17-3
               mingw-w64-x86_64-libsystre-1.0.1-4  mingw-w64-x86_64-libtre-git-r128.6fb7206-2
               mingw-w64-x86_64-mpc-1.3.1-1  mingw-w64-x86_64-mpdecimal-2.5.1-1  mingw-w64-x86_64-mpfr-4.2.0-1
               mingw-w64-x86_64-ncurses-6.4.20230211-1  mingw-w64-x86_64-python-3.10.10-1
               mingw-w64-x86_64-readline-8.2.001-6  mingw-w64-x86_64-sqlite3-3.41.1-1
               mingw-w64-x86_64-tcl-8.6.12-1  mingw-w64-x86_64-termcap-1.3.1-6  mingw-w64-x86_64-tk-8.6.12-1
               mingw-w64-x86_64-tzdata-2022g-1  mingw-w64-x86_64-windows-default-manifest-6.4-4
               mingw-w64-x86_64-xxhash-0.8.1-2  mingw-w64-x86_64-xz-5.4.1-1  mingw-w64-x86_64-zlib-1.2.13-3
               mingw-w64-x86_64-zstd-1.5.4-1  openssh-9.3p1-1  patch-2.7.6-2  perl-Authen-SASL-2.16-3
               perl-Clone-0.46-1  perl-Convert-BinHex-1.125-2  perl-Encode-Locale-1.05-2  perl-Error-0.17029-1
               perl-File-Listing-6.15-1  perl-HTML-Parser-3.81-1  perl-HTML-Tagset-3.20-3
               perl-HTTP-Cookies-6.10-2  perl-HTTP-Daemon-6.16-1  perl-HTTP-Date-6.05-1
               perl-HTTP-Message-6.44-1  perl-HTTP-Negotiate-6.01-3  perl-IO-HTML-1.004-2
               perl-IO-Socket-SSL-2.081-1  perl-IO-Stringy-2.113-1  perl-LWP-MediaTypes-6.04-1
               perl-MIME-tools-5.510-1  perl-MailTools-2.21-1  perl-Net-HTTP-6.22-1  perl-Net-SMTP-SSL-1.04-2
               perl-Net-SSLeay-1.92-4  perl-TermReadKey-2.38-5  perl-TimeDate-2.33-2  perl-Try-Tiny-0.31-1
               perl-URI-5.17-2  perl-WWW-RobotRules-6.02-2  perl-libwww-6.67-1  texinfo-7.0.2-1
               texinfo-tex-7.0.2-1  autoconf-wrapper-20221207-1  automake-wrapper-20221207-1
               base-devel-2022.12-2  git-2.40.0-1  libtool-2.4.7-3  make-4.4.1-1
               mingw-w64-x86_64-binutils-2.40-2  mingw-w64-x86_64-crt-git-10.0.0.r234.g283e5b23a-1
               mingw-w64-x86_64-gcc-12.2.0-10  mingw-w64-x86_64-gcc-ada-12.2.0-10
               mingw-w64-x86_64-gcc-fortran-12.2.0-10  mingw-w64-x86_64-gcc-libgfortran-12.2.0-10
               mingw-w64-x86_64-gcc-libs-12.2.0-10  mingw-w64-x86_64-gcc-objc-12.2.0-10
               mingw-w64-x86_64-gdb-13.1-3  mingw-w64-x86_64-gdb-multiarch-13.1-3
               mingw-w64-x86_64-headers-git-10.0.0.r234.g283e5b23a-1  mingw-w64-x86_64-libgccjit-12.2.0-10
               mingw-w64-x86_64-libltdl-2.4.7-1  mingw-w64-x86_64-libmangle-git-10.0.0.r234.g283e5b23a-1
               mingw-w64-x86_64-libwinpthread-git-10.0.0.r234.g283e5b23a-1  mingw-w64-x86_64-make-4.4-2
               mingw-w64-x86_64-openssl-3.1.0-1  mingw-w64-x86_64-pkgconf-1~1.8.0-2
               mingw-w64-x86_64-tools-git-10.0.0.r234.g283e5b23a-1
               mingw-w64-x86_64-winpthreads-git-10.0.0.r234.g283e5b23a-1
               mingw-w64-x86_64-winstorecompat-git-10.0.0.r234.g283e5b23a-1

Total Download Size:    175.82 MiB
Total Installed Size:  1091.49 MiB

:: Proceed with installation? [Y/n]
:: Retrieving packages...
 mingw-w64-x86_64-gcc-fortran-12.2...    10.7 MiB   778 KiB/s 00:14 [####################################] 100%
 mingw-w64-x86_64-gcc-objc-12.2.0-...    12.4 MiB   685 KiB/s 00:19 [####################################] 100%
 mingw-w64-x86_64-openssl-3.1.0-1-any     7.3 MiB  1308 KiB/s 00:06 [####################################] 100%
 mingw-w64-x86_64-libgccjit-12.2.0...    10.1 MiB  1113 KiB/s 00:09 [####################################] 100%
 git-2.40.0-1-x86_64                      6.2 MiB  1639 KiB/s 00:04 [####################################] 100%
 mingw-w64-x86_64-gdb-multiarch-13...     6.7 MiB  1433 KiB/s 00:05 [####################################] 100%
 mingw-w64-x86_64-binutils-2.40-2-any     6.1 MiB  1953 KiB/s 00:03 [####################################] 100%
 mingw-w64-x86_64-headers-git-10.0...     5.7 MiB  2.58 MiB/s 00:02 [####################################] 100%
 mingw-w64-x86_64-gcc-12.2.0-10-any      27.7 MiB   813 KiB/s 00:35 [####################################] 100%
 mingw-w64-x86_64-gdb-13.1-3-any          4.3 MiB  2.04 MiB/s 00:02 [####################################] 100%
 mingw-w64-x86_64-crt-git-10.0.0.r...     3.3 MiB  2.32 MiB/s 00:01 [####################################] 100%
 binutils-2.40-1-x86_64                   5.4 MiB  1893 KiB/s 00:03 [####################################] 100%
 mingw-w64-x86_64-tcl-8.6.12-1-any        2.6 MiB  1277 KiB/s 00:02 [####################################] 100%
 mingw-w64-x86_64-tk-8.6.12-1-any      1987.0 KiB  1055 KiB/s 00:02 [####################################] 100%
 mingw-w64-x86_64-gettext-0.21.1-1-any    3.3 MiB  1247 KiB/s 00:03 [####################################] 100%
 mingw-w64-x86_64-gcc-ada-12.2.0-1...    19.9 MiB   493 KiB/s 00:41 [####################################] 100%
 mingw-w64-x86_64-python-3.10.10-1-any   18.4 MiB   396 KiB/s 00:48 [####################################] 100%
 mingw-w64-x86_64-ncurses-6.4.2023...  1796.6 KiB  1537 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-isl-0.25-1-any       1396.6 KiB   926 KiB/s 00:02 [####################################] 100%
 mingw-w64-x86_64-sqlite3-3.41.1-1-any 1459.7 KiB   802 KiB/s 00:02 [####################################] 100%
 texinfo-7.0.2-1-x86_64                1340.1 KiB   699 KiB/s 00:02 [####################################] 100%
 openssh-9.3p1-1-x86_64                 963.1 KiB  1027 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-gcc-libs-12.2.0-...   876.1 KiB  1082 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-gcc-libgfortran-...   852.6 KiB  1533 KiB/s 00:01 [####################################] 100%
 bison-3.8.2-4-x86_64                   778.1 KiB  1129 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-libiconv-1.17-3-any   719.8 KiB  1000 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-zstd-1.5.4-1-any      611.8 KiB   766 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-gmp-6.2.1-5-any       571.7 KiB   726 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-xz-5.4.1-1-any        570.9 KiB   913 KiB/s 00:01 [####################################] 100%
 automake1.16-1.16.5-1-any              526.3 KiB   882 KiB/s 00:01 [####################################] 100%
 heimdal-7.8.0-3-x86_64                 544.5 KiB   754 KiB/s 00:01 [####################################] 100%
 automake1.15-1.15.1-4-any              513.4 KiB   933 KiB/s 00:01 [####################################] 100%
 make-4.4.1-1-x86_64                    505.9 KiB   725 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-readline-8.2.001...   504.9 KiB   679 KiB/s 00:01 [####################################] 100%
 automake1.12-1.12.6-6-any              503.1 KiB   784 KiB/s 00:01 [####################################] 100%
 automake1.14-1.14.1-6-any              503.1 KiB   699 KiB/s 00:01 [####################################] 100%
 automake1.13-1.13.4-7-any              501.5 KiB   536 KiB/s 00:01 [####################################] 100%
 automake1.11-1.11.6-6-any              490.2 KiB   612 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-mpfr-4.2.0-1-any      430.2 KiB   902 KiB/s 00:00 [####################################] 100%
 dos2unix-7.4.4-1-x86_64                429.4 KiB  1101 KiB/s 00:00 [####################################] 100%
 libtool-2.4.7-3-x86_64                 397.2 KiB   651 KiB/s 00:01 [####################################] 100%
 diffutils-3.9-1-x86_64                 380.0 KiB   506 KiB/s 00:01 [####################################] 100%
 autoconf2.71-2.71-1-any                326.6 KiB   508 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-tools-git-10.0.0...   315.3 KiB   499 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-mpdecimal-2.5.1-...   321.9 KiB   443 KiB/s 00:01 [####################################] 100%
 flex-2.6.4-3-x86_64                    303.8 KiB   506 KiB/s 00:01 [####################################] 100%
 autoconf2.69-2.69-2-any                284.0 KiB   828 KiB/s 00:00 [####################################] 100%
 m4-1.4.19-2-x86_64                     238.1 KiB   491 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-tzdata-2022g-1-any    227.8 KiB   583 KiB/s 00:00 [####################################] 100%
 perl-Net-SSLeay-1.92-4-x86_64          209.4 KiB   583 KiB/s 00:00 [####################################] 100%
 perl-MIME-tools-5.510-1-any            183.6 KiB   469 KiB/s 00:00 [####################################] 100%
 perl-IO-Socket-SSL-2.081-1-any         157.2 KiB   419 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-expat-2.5.0-1-any     155.8 KiB   383 KiB/s 00:00 [####################################] 100%
 autoconf2.13-2.13-5-any                136.3 KiB   323 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-make-4.4-2-any        135.1 KiB   412 KiB/s 00:00 [####################################] 100%
 perl-libwww-6.67-1-any                 129.8 KiB   319 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-mpc-1.3.1-1-any       104.4 KiB   141 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-xxhash-0.8.1-2-any    106.1 KiB   108 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-zlib-1.2.13-3-any     103.8 KiB   139 KiB/s 00:01 [####################################] 100%
 patch-2.7.6-2-x86_64                    96.8 KiB   130 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-bzip2-1.0.8-2-any      89.1 KiB   169 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-libtre-git-r128....    84.2 KiB   153 KiB/s 00:01 [####################################] 100%
 perl-HTML-Parser-3.81-1-x86_64          80.2 KiB   290 KiB/s 00:00 [####################################] 100%
 perl-URI-5.17-2-any                     80.1 KiB   274 KiB/s 00:00 [####################################] 100%
 perl-MailTools-2.21-1-any               81.0 KiB   156 KiB/s 00:01 [####################################] 100%
 perl-HTTP-Message-6.44-1-any            77.1 KiB   301 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-pkgconf-1~1.8.0-...    79.1 KiB   158 KiB/s 00:01 [####################################] 100%
 perl-IO-Stringy-2.113-1-any             66.4 KiB   254 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-libltdl-2.4.7-1-any    50.2 KiB   193 KiB/s 00:00 [####################################] 100%
 libfido2-1.13.0-1-x86_64                76.4 KiB   150 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-libffi-3.4.4-1-any     42.5 KiB  81.0 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-winpthreads-git-...    40.0 KiB  77.5 KiB/s 00:01 [####################################] 100%
 perl-LWP-MediaTypes-6.04-1-any          40.7 KiB  52.8 KiB/s 00:01 [####################################] 100%
 perl-Error-0.17029-1-any                39.4 KiB  77.8 KiB/s 00:01 [####################################] 100%
 libltdl-2.4.7-3-x86_64                  39.1 KiB  75.1 KiB/s 00:01 [####################################] 100%
 perl-Authen-SASL-2.16-3-any             37.9 KiB  74.4 KiB/s 00:01 [####################################] 100%
 perl-TimeDate-2.33-2-any                35.6 KiB  70.0 KiB/s 00:01 [####################################] 100%
 diffstat-1.65-1-x86_64                  29.2 KiB  57.7 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-libwinpthread-gi...    29.0 KiB  57.4 KiB/s 00:01 [####################################] 100%
 perl-Convert-BinHex-1.125-2-any         29.8 KiB  38.9 KiB/s 00:01 [####################################] 100%
 perl-HTTP-Date-6.05-1-any               28.9 KiB  55.3 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-termcap-1.3.1-6-any    28.0 KiB  52.0 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-libsystre-1.0.1-...    24.0 KiB  44.4 KiB/s 00:01 [####################################] 100%
 texinfo-tex-7.0.2-1-x86_64              26.1 KiB  48.4 KiB/s 00:01 [####################################] 100%
 perl-Net-HTTP-6.22-1-any                23.1 KiB  86.7 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-libmangle-git-10...    22.2 KiB  46.3 KiB/s 00:00 [####################################] 100%
 mingw-w64-x86_64-winstorecompat-g...    22.1 KiB  41.3 KiB/s 00:01 [####################################] 100%
 perl-HTTP-Cookies-6.10-2-any            21.9 KiB  43.3 KiB/s 00:01 [####################################] 100%
 perl-TermReadKey-2.38-5-x86_64          20.5 KiB  38.2 KiB/s 00:01 [####################################] 100%
 perl-Try-Tiny-0.31-1-any                19.8 KiB  37.1 KiB/s 00:01 [####################################] 100%
 perl-HTTP-Daemon-6.16-1-any             18.7 KiB  35.7 KiB/s 00:01 [####################################] 100%
 libcbor-0.10.2-1-x86_64                 18.1 KiB  35.5 KiB/s 00:01 [####################################] 100%
 perl-IO-HTML-1.004-2-any                14.4 KiB  28.3 KiB/s 00:01 [####################################] 100%
 perl-WWW-RobotRules-6.02-2-any          12.2 KiB  23.5 KiB/s 00:01 [####################################] 100%
 perl-HTTP-Negotiate-6.01-3-any          12.1 KiB  23.6 KiB/s 00:01 [####################################] 100%
 perl-File-Listing-6.15-1-any            10.9 KiB  20.9 KiB/s 00:01 [####################################] 100%
 perl-HTML-Tagset-3.20-3-any             10.9 KiB  21.2 KiB/s 00:01 [####################################] 100%
 perl-Encode-Locale-1.05-2-any           10.7 KiB  20.2 KiB/s 00:01 [####################################] 100%
 perl-Clone-0.46-1-x86_64                10.4 KiB  19.8 KiB/s 00:01 [####################################] 100%
 autoconf-wrapper-20221207-1-any          5.0 KiB  9.81 KiB/s 00:01 [####################################] 100%
 perl-Net-SMTP-SSL-1.04-2-any             4.9 KiB  9.57 KiB/s 00:01 [####################################] 100%
 automake-wrapper-20221207-1-any          4.4 KiB  8.52 KiB/s 00:01 [####################################] 100%
 mingw-w64-x86_64-windows-default-...     3.1 KiB  5.83 KiB/s 00:01 [####################################] 100%
 base-devel-2022.12-2-any                 2.4 KiB  4.63 KiB/s 00:01 [####################################] 100%
 Total (104/104)                        175.8 MiB  2.23 MiB/s 01:19 [####################################] 100%
error: failed retrieving file 'mingw-w64-x86_64-python-3.10.10-1-any.pkg.tar.zst' from mirror.msys2.org : SSL connection timeout
error: failed retrieving file 'mingw-w64-x86_64-gcc-ada-12.2.0-10-any.pkg.tar.zst' from mirror.msys2.org : Operation too slow. Less than 1 bytes/sec transferred the last 10 seconds
error: failed retrieving file 'mingw-w64-x86_64-gcc-12.2.0-10-any.pkg.tar.zst' from mirror.msys2.org : Operation too slow. Less than 1 bytes/sec transferred the last 10 seconds
warning: too many errors from mirror.msys2.org, skipping for the remainder of this transaction
error: failed retrieving file 'mingw-w64-x86_64-gcc-objc-12.2.0-10-any.pkg.tar.zst' from mirror.msys2.org : Operation too slow. Less than 1 bytes/sec transferred the last 10 seconds
error: failed retrieving file 'mingw-w64-x86_64-gcc-fortran-12.2.0-10-any.pkg.tar.zst' from mirror.msys2.org : Operation too slow. Less than 1 bytes/sec transferred the last 10 seconds
(104/104) checking keys in keyring                                  [####################################] 100%
(104/104) checking package integrity                                [####################################] 100%
(104/104) loading package files                                     [####################################] 100%
(104/104) checking for file conflicts                               [####################################] 100%
(104/104) checking available disk space                             [####################################] 100%
:: Processing package changes...
(  1/104) installing binutils                                       [####################################] 100%
(  2/104) installing m4                                             [####################################] 100%
(  3/104) installing bison                                          [####################################] 100%
(  4/104) installing diffstat                                       [####################################] 100%
(  5/104) installing diffutils                                      [####################################] 100%
(  6/104) installing dos2unix                                       [####################################] 100%
(  7/104) installing flex                                           [####################################] 100%
(  8/104) installing texinfo                                        [####################################] 100%
(  9/104) installing texinfo-tex                                    [####################################] 100%
( 10/104) installing make                                           [####################################] 100%
( 11/104) installing patch                                          [####################################] 100%
Optional dependencies for patch
    ed: for patch -e functionality
( 12/104) installing base-devel                                     [####################################] 100%
( 13/104) installing autoconf2.71                                   [####################################] 100%
( 14/104) installing autoconf2.69                                   [####################################] 100%
( 15/104) installing autoconf2.13                                   [####################################] 100%
( 16/104) installing autoconf-wrapper                               [####################################] 100%
( 17/104) installing automake1.11                                   [####################################] 100%
( 18/104) installing automake1.12                                   [####################################] 100%
( 19/104) installing automake1.13                                   [####################################] 100%
( 20/104) installing automake1.14                                   [####################################] 100%
( 21/104) installing automake1.15                                   [####################################] 100%
( 22/104) installing automake1.16                                   [####################################] 100%
( 23/104) installing automake-wrapper                               [####################################] 100%
( 24/104) installing libltdl                                        [####################################] 100%
( 25/104) installing libtool                                        [####################################] 100%
( 26/104) installing heimdal                                        [####################################] 100%
( 27/104) installing libcbor                                        [####################################] 100%
( 28/104) installing libfido2                                       [####################################] 100%
( 29/104) installing openssh                                        [####################################] 100%
( 30/104) installing perl-Error                                     [####################################] 100%
( 31/104) installing perl-Authen-SASL                               [####################################] 100%
( 32/104) installing perl-Encode-Locale                             [####################################] 100%
( 33/104) installing perl-HTTP-Date                                 [####################################] 100%
( 34/104) installing perl-File-Listing                              [####################################] 100%
( 35/104) installing perl-HTML-Tagset                               [####################################] 100%
( 36/104) installing perl-Clone                                     [####################################] 100%
( 37/104) installing perl-IO-HTML                                   [####################################] 100%
( 38/104) installing perl-LWP-MediaTypes                            [####################################] 100%
( 39/104) installing perl-URI                                       [####################################] 100%
( 40/104) installing perl-HTTP-Message                              [####################################] 100%
( 41/104) installing perl-HTML-Parser                               [####################################] 100%
( 42/104) installing perl-HTTP-Cookies                              [####################################] 100%
( 43/104) installing perl-HTTP-Daemon                               [####################################] 100%
( 44/104) installing perl-HTTP-Negotiate                            [####################################] 100%
( 45/104) installing perl-Net-HTTP                                  [####################################] 100%
( 46/104) installing perl-WWW-RobotRules                            [####################################] 100%
( 47/104) installing perl-Try-Tiny                                  [####################################] 100%
( 48/104) installing perl-libwww                                    [####################################] 100%
Optional dependencies for perl-libwww
    perl-LWP-Protocol-https: for https:// url schemes
( 49/104) installing perl-TimeDate                                  [####################################] 100%
( 50/104) installing perl-MailTools                                 [####################################] 100%
( 51/104) installing perl-IO-Stringy                                [####################################] 100%
( 52/104) installing perl-Convert-BinHex                            [####################################] 100%
module test... pass.
( 53/104) installing perl-MIME-tools                                [####################################] 100%
( 54/104) installing perl-Net-SSLeay                                [####################################] 100%
( 55/104) installing perl-IO-Socket-SSL                             [####################################] 100%
( 56/104) installing perl-Net-SMTP-SSL                              [####################################] 100%
( 57/104) installing perl-TermReadKey                               [####################################] 100%
( 58/104) installing git                                            [####################################] 100%
Optional dependencies for git
    python: various helper scripts
    subversion: git svn
( 59/104) installing mingw-w64-x86_64-libwinpthread-git             [####################################] 100%
( 60/104) installing mingw-w64-x86_64-gcc-libs                      [####################################] 100%
( 61/104) installing mingw-w64-x86_64-zstd                          [####################################] 100%
( 62/104) installing mingw-w64-x86_64-binutils                      [####################################] 100%
( 63/104) installing mingw-w64-x86_64-headers-git                   [####################################] 100%
( 64/104) installing mingw-w64-x86_64-crt-git                       [####################################] 100%
( 65/104) installing mingw-w64-x86_64-gmp                           [####################################] 100%
( 66/104) installing mingw-w64-x86_64-isl                           [####################################] 100%
( 67/104) installing mingw-w64-x86_64-libiconv                      [####################################] 100%
( 68/104) installing mingw-w64-x86_64-mpfr                          [####################################] 100%
( 69/104) installing mingw-w64-x86_64-mpc                           [####################################] 100%
( 70/104) installing mingw-w64-x86_64-windows-default-manifest      [####################################] 100%
( 71/104) installing mingw-w64-x86_64-winpthreads-git               [####################################] 100%
( 72/104) installing mingw-w64-x86_64-zlib                          [####################################] 100%
( 73/104) installing mingw-w64-x86_64-gcc                           [####################################] 100%
( 74/104) installing mingw-w64-x86_64-gcc-ada                       [####################################] 100%
( 75/104) installing mingw-w64-x86_64-gcc-libgfortran               [####################################] 100%
( 76/104) installing mingw-w64-x86_64-gcc-fortran                   [####################################] 100%
( 77/104) installing mingw-w64-x86_64-gcc-objc                      [####################################] 100%
( 78/104) installing mingw-w64-x86_64-expat                         [####################################] 100%
( 79/104) installing mingw-w64-x86_64-gettext                       [####################################] 100%
( 80/104) installing mingw-w64-x86_64-libtre-git                    [####################################] 100%
( 81/104) installing mingw-w64-x86_64-libsystre                     [####################################] 100%
( 82/104) installing mingw-w64-x86_64-ncurses                       [####################################] 100%
( 83/104) installing mingw-w64-x86_64-bzip2                         [####################################] 100%
( 84/104) installing mingw-w64-x86_64-libffi                        [####################################] 100%
( 85/104) installing mingw-w64-x86_64-mpdecimal                     [####################################] 100%
( 86/104) installing mingw-w64-x86_64-openssl                       [####################################] 100%
Optional dependencies for mingw-w64-x86_64-openssl
    mingw-w64-x86_64-ca-certificates
( 87/104) installing mingw-w64-x86_64-termcap                       [####################################] 100%
( 88/104) installing mingw-w64-x86_64-readline                      [####################################] 100%
( 89/104) installing mingw-w64-x86_64-tcl                           [####################################] 100%
( 90/104) installing mingw-w64-x86_64-sqlite3                       [####################################] 100%
( 91/104) installing mingw-w64-x86_64-tk                            [####################################] 100%
( 92/104) installing mingw-w64-x86_64-xz                            [####################################] 100%
( 93/104) installing mingw-w64-x86_64-tzdata                        [####################################] 100%
( 94/104) installing mingw-w64-x86_64-python                        [####################################] 100%
( 95/104) installing mingw-w64-x86_64-xxhash                        [####################################] 100%
( 96/104) installing mingw-w64-x86_64-gdb                           [####################################] 100%
Optional dependencies for mingw-w64-x86_64-gdb
    mingw-w64-x86_64-python-pygments: for syntax highlighting
( 97/104) installing mingw-w64-x86_64-gdb-multiarch                 [####################################] 100%
Optional dependencies for mingw-w64-x86_64-gdb-multiarch
    mingw-w64-x86_64-python-pygments: for syntax highlighting
( 98/104) installing mingw-w64-x86_64-libgccjit                     [####################################] 100%
( 99/104) installing mingw-w64-x86_64-libmangle-git                 [####################################] 100%
(100/104) installing mingw-w64-x86_64-make                          [####################################] 100%
(101/104) installing mingw-w64-x86_64-pkgconf                       [####################################] 100%
(102/104) installing mingw-w64-x86_64-tools-git                     [####################################] 100%
(103/104) installing mingw-w64-x86_64-winstorecompat-git            [####################################] 100%
(104/104) installing mingw-w64-x86_64-libltdl                       [####################################] 100%
:: Running post-transaction hooks...
(1/1) Updating the info directory file...

ThreadRipper@DESKTOP-QE5C5HQ UCRT64 ~
```
