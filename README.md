FBThrift: Facebook's branch of apache thrift
--------------------------------------------

The main focus of this package is the new C++ server, under thrift/lib/cpp2.  This repo also contains a branch of the rest of apache thrift's repo with any changes Facebook has made, however the build system only supports cpp2.

Apache thrift is at http://thrift.apache.org/

Building
--------

For your convenience, a build script is provided for ubuntu 12.10 64-bit:

```sh
cd fbthrift/thrift
./deps.sh
```

It will automatically pull down folly and build it, and then configure and build thrift.

Dependencies
------------

 - Facebook's folly library: http://www.github.com/facebook/folly

 - Ubuntu 12.10 64-bit requires the following packages:

    - autoconf
    - libtool
    - g++
    - libboost-dev-all
    - libevent-dev
    - flex
    - bison
    - libgoogle-glog-dev
    - scons
    - libkrb5-dev
    - libsnappy-dev
    - libsasl2-dev

Docs
----

Some docs on the new cpp2 server are at:
https://github.com/facebook/fbthrift/blob/master/thrift/doc/Cpp2.md
