# Introduction #

Rudix 2012 will feature a robust package set for Lion and Snow Leopard.

# Proposing Features #

  * Include Introduction telling about Rudix when installing a package from the web. **DONE**
  * Include logo when installing a package from the web. **DONE**
  * Create a independent repository for Snow Leopard packages to avoid the _compat-_ packages in current repository. **DONE**

## Rudix Command Line ##

  * Rudix search must be case-insentitive.
```
rudix search Mercurial
mercurial-1.3.1-0
mercurial-1.3.1-1
```

  * Package aliases and information, like 'bazaar' to link to 'bzr'. Example:
```
rudix install bazaar
To install Bazaar use 'bzr'
```

## Packages ##

Include new packages.

  * Apache HTTPd 2.4.x
  * Django
  * Go language
  * Monit
  * Squid 2.7.x
  * Supervisor

# Maybe #

  * Build packages with a safe LANG value.
```
LANG=C; export LANG
```
  * Adopt Ruby modules
  * Adopt PHP modules