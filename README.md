ftbrony
=======

FTP Server for 3DS.


Modifications from original
---------------------------
- Ponys have been removed/replaced
- Building also cia now
- Removed Linux Makefile

Features
--------
- Appears to work well with a variety of clients.
- Supports multiple simultaneous clients. The 3DS itself only appears to support enough sockets to perform 4-5 simultaneous data transfers, so it will help if you limit your FTP client to this many parallel requests.
- Cutting-edge graphics.

Build and install
------------------

You must first install and set up [devkitARM and libctru](http://3dbrew.org/wiki/Setting_up_Development_Environment).
Clone this repository and cd in the resulting directory.

    make

If you don't want to compile yourself, prebuild version can be found [here](https://github.com/Netfreak25/ftbrony/releases).

Copy the `ftbrony.3dsx` file to your SD card and launch it.
Copy the `ftbrony.cia` file to you SD card and install it with e.g. FBI, DevMenu or NASA

Supported Commands
------------------

- ABOR
- ALLO (no-op)
- APPE
- CDUP
- CWD
- DELE
- FEAT
- HELP
- LIST
- MKD
- MODE (no-op)
- NLST
- NOOP
- OPTS
- PASS (no-op)
- PASV
- PORT
- PWD
- QUIT
- REST
- RETR
- RMD
- RNFR
- RNTO
- STAT
- STOR
- STRU (no-op)
- SYST
- TYPE (no-op)
- USER (no-op)
- XCUP
- XCWD
- XMKD
- XPWD
- XRMD

Planned Commands
----------------

- STOU
