# Debian package from CoreDNS Git

Copy the `debian` directory in the git repository of CoreDNS and then call:

~~~
dpkg-buildpackage -us -uc -b --target-arch amd64
~~~

Other archs are available:

* armhf
* arm64

The `Makefile.release` in the CoreDNS repo will build Darwin and Windows builds before it goes onto
the Linux build, so you'll have to wait a bit before your `.dep` show up.
