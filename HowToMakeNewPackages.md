# Introduction #

You are happily using Rudix until one day you discover that a UNIX package you need is not available, what should you do now? First thing, DON’T PANIC. This article will show how to make a new package for Rudix, from Makefiles to PackageMaker projects. Although it might seem complex it is actually mostly filling boilerplate code with the new package data.

For this process we will start by showing how Rudix internals works and then go on to explain how to package an example library (libJPEG) and point how to fix common problems along the way.

# How it Rudix Works? #

Rudix was modeled to be somewhat similar to the RPM build system, only a lot simpler and for Mac OS X. The process of building a package is controlled by a set of Makefiles that automate most of the work, going from download and configuration all the way to running PackageMaker to generate a package (.pkg) and to put it for download.

## Rudix Build System Steps ##

The rudix build system goes through a series of steps to build a ready to download package. They are in order:

| retrieve | prep | build | test | install | check | pkg | final |
|:---------|:-----|:------|:-----|:--------|:------|:----|:------|

The process of uploading the resulting pkg file is automated right now, but only developers have access to put it on the site anyway, so don’t worry about that.

  * retrieve - get the source (the tarball) from the home site (variable URL in Makefile).
  * prep - prepare to build (uncompress the tarball).
  * build - process the build (run configure if necessary).
  * test - test the build using the source's built-in tests.
  * install - proceed with local installation.
  * check - run tests in the local installation.
  * pkg - create the package from files in local installation.
  * final - test the final package

# Starting Up #

In this tutorial we will be creating a new port for Rudix for the [libjpeg](http://www.ijg.org/) library

you need to learn how to download, configure and compile the package you want before trying to make a rudix port.

# Your first Rudix Port #

first clone the Rudix source:

```
$ hg clone https://rudix.googlecode.com/hg/ rudix 
```

ps, if you don’t have mercurial installed just install the package on rudix

Then go to the ports directory and create a new port, the newport rule on the Ports Makefile creates a directory and sets it up for a new port with that name:

```
$ cd rudix/Ports/
$ make newport libjpeg
```

newport takes the name of the new directory for the port and assumes it for the package name.

# Editing the Makefile #

You will have to edit at least this fields:
  * homepage
  * download url
  * package version

```
$ cd libjpeg
```

```
$ open Makefile # or use editor you want, eg. (m)vim, (aqua)emacs, textmate, bbedit
```

# Building the package #

After editing the Makefile we can try to build the package and then go and fix any problems that will happen

```
$ make build
```

## Common errors during the build ##

# Creating a PackageMaker project #

```
$ make pmdoc
```

## The file listing ##
File listing is the one thing that you have to do manually or no files will be in your .pkg file.

# Testing the new package #

```
$ make dmg
```

# Sending it to be included in Rudix #
Create a new ticket on the issue tracker with your patch attached. To get a patch for your work:

```
$ hg diff
```