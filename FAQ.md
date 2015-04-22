# FAQ #

## What does Rudix mean? ##

Rudix is the mixing of Rudá and Unix and it doesn't mean anything special besides the name of the author.

## What are the advantages of Rudix against the others? ##

In one word: simplicity.
All programs are pre-compiled and self-contained (no external dependencies) and installable as Mac OS X packages.

## Why does Rudix install packages under /usr/local? ##
Why invent another path? /usr/local is the standard place for all **third party software** in every Unix on planet Earth.

## Why do I need to keep entering root password to install in /usr/local? ##
The path /usr/local is owned by the user _root_ and group _wheel_ and even administrators can't write into this kind of permission without entering the password for root -- by the way, Administrators are in the special group _admin_.

## Why do I avoid to type the root password when I use rudix commands? ##

Find information about using sudo (and visudo) without typing password.
```
%admin  ALL=(ALL) NOPASSWD: ALL
```

## How do I Bootstrap Rudix in command line? ##
```
curl -O http://rudix.googlecode.com/hg/Ports/rudix/rudix.py
sudo python rudix.py install rudix
```

You will be probably asked for administrator password.

## How do I install/uninstall a package? ##

See [Usage](http://rudix.org/#usage).

## How do I remove Rudix? I mean, all packages at once ##
```
sudo rudix -R
```

## I dislike Rudix. Is there any alternative? ##
We recommend [Homebrew](http://mxcl.github.com/homebrew/) if you need more packages than we have or just dislike Rudix.

There are other package systems for Mac OS X if you want also:
  * [MacPorts](http://www.macports.org/)
  * [Fink](http://www.finkproject.org/)

## Why PowerPC is not supported? ##
I (the Author) no longer own an iBook, so it's not possible to compile and test for PowerPC.