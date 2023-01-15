emit(1), interact with a process over TCP.

Usage: emit [port] [command]

This command implements a network-accessible interface to 
arbitrary shell commands. NetCat users may be familiar with
the `-e` flag which does the same thing in some versions.

Example:

[alice@192.168.0.1 ~]$ emit 1234 /bin/sh

[bob@192.168.0.2 ~]$ nc 192.168.0.1 1234

$ whoami

alice
