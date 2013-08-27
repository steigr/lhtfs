lousy hyper-text filesystem (lhtfs)
===================================

Quickstart
----------
	git clone git://github.com/steigr/lhtfs.git /tmp/lhtfs
	cp /tmp/lhtfs /usr/local/bin/lhtfs
	chmod 0700 /usr/local/bin/lhtfs

Usage
-----

Use with caution, many bugs included!

Every user which should use lhtfs must be in fuse-group (`adduser $USERNAME fuse`).

Copy lhtfs-Script to /usr/local/sbin (or some other location listed in `$PATH`) and make it executable (`chmod 0755 $(which lhtfs)`).

You may add a line to `/etc/fstab` to mount your webserver at boot-time.

fstab-Example
-------------

`lhtfs#http://webserver.example.com /srv/webserver fuse defaults,allow_other 0 0`

