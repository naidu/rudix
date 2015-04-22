# Creating a Port #

Pretty formatting XMLs in PMDOC:
```
$ cd name.pmdoc/
$ for x in *.xml ; do xmllint --format $x --output $x ; done
```
# Building #
## Common errors and fixes ##
  * gcc-4.2: -E, -S, -save-temps and -M options are not allowed with multiple -arch flags

Pass to configure the `--disable-dependency-tracking` option.


# Packaging #

## Low-level package management ##

To list all Rudix packages installed:
```
$ pkgutil --pkgs=org.rudix.pkg.*
org.rudix.pkg.apr
org.rudix.pkg.boost
org.rudix.pkg.bvi
org.rudix.pkg.bzr
…
```

To retrieve information about a package:
```
$ pkgutil -v --pkg-info org.rudix.pkg.apr
  package-id: org.rudix.pkg.apr
     version: 1.4.2-1
      volume: /
    location: 
install-time: Sun Nov 14 20:14:49 2010
```

To list file content from a package:
```
$ pkgutil --files org.rudix.pkg.wget
usr
usr/local
usr/local/bin
usr/local/bin/wget
…
```

To remove a package and its files:
```
$ sudo pkgutil --unlink org.rudix.pkg.boost
Do you really want to delete these files? yes
…
$ sudo pkgutil --forget org.rudix.pkg.boost
Forgot package 'org.rudix.pkg.boost' on '/'.
```


Try to find some information about a file in a package:
```
$ pkgutil -v --file-info /usr/local/bin/wget 
     volume: /
       path: /usr/local/bin/wget

       pkgid: org.rudix.pkg.wget
 pkg-version: 1.12
install-time: Wed Sep  1 22:13:00 2010
         uid: 0 (root)
         gid: 0 (wheel)
        mode: 775 (?rwxrwxr-x )
```
## Links ##
  * [PackageMaker How-to](http://s.sudre.free.fr/Stuff/PackageMaker_Howto.html) - documentation about Package Maker,  a bit dated but still useful.

# Misc #

## How do I compile an Universal Binary? ##
In most of the time you pass ```
-arch i386 -arch x86_64``` to CFLAGS, CXXFLAGS and LDFLAGS. This is exactly what Rudix does (see Rules.mk file).

There is another alternative, which is compile in two parts (for two architectures) and then join the binary with lipo:
<pre>
$ gcc -arch i386 hello.c -o hello-i386<br>
$ gcc -arch x86_64 hello.c -o hello-x86_64<br>
$ lipo -create -arch i386 hello-i386 -arch x86_64 hello-x86_64 -o hello<br>
</pre>

## ucontext routines are deprecated ##
If you see
<pre>
#error ucontext routines are deprecated, and require _XOPEN_SOURCE to be defined<br>
</pre>
change in program's source the occurrences of ```
#include <ucontext.h>``` to ```
#include <sys/ucontext.h>```.

Another possible solution is to define XOPEN\_SOURCE ```
#define _XOPEN_SOURCE 1000``` in your sources.

See also:
  * http://duriansoftware.com/joe/PSA:-avoiding-the-%22ucontext-routines-are-deprecated%22-error-on-Mac-OS-X-Snow-Leopard.html
  * http://code.google.com/p/google-perftools/issues/detail?id=169