# Compile Times #

## Machines ##
|MacBook Pro 2.26 Ghz|`MacBookPro5,5/8GB+`|8 GB RAM|640 GB Samsung HD|
|:-------------------|:-------------------|:-------|:----------------|
|MacBook Pro 2.26 Ghz|`MacBookPro5,5/8GB`|8 GB RAM|160 GB Seagate HD|
|MacBook Pro 2.26 Ghz|`MacBookPro5,5`|2 GB RAM|160 GB Seagate HD|
|MacBook 1.83 GHz|`MacBook1,1`|2 GB RAM|160 GB Samsung HD|

## Developer Tools ##
|Version|Machine|GCC/LLVM version|
|:------|:------|:---------------|
|Xcode 4.3|`MacBookPro5,5/8GB+`|i686-apple-darwin11-llvm-gcc-4.2 (GCC) 4.2.1 (Based on Apple Inc. build 5658) (LLVM build 2336.9.00)|
|Xcode 4.2|`MacBookPro5,5/8GB+`|i686-apple-darwin11-llvm-gcc-4.2 (GCC) 4.2.1 (Based on Apple Inc. build 5658) (LLVM build 2336.1.00)|
|Xcode 4.1|`MacBookPro5,5/8GB+`|i686-apple-darwin11-llvm-gcc-4.2 (GCC) 4.2.1 (Based on Apple Inc. build 5658) (LLVM build 2335.15.00)|
|Xcode 4.0|`MacBook1,1`|i686-apple-darwin10-gcc-4.2.1 (GCC) 4.2.1 (Apple Inc. build 5666) (dot 3)|

## Rudix 2012 ##

### Lion + Xcode 4.3 ###
Machine `MBP5,5/8GB+`
| | 1st run | 2nd run |
|:|:--------|:--------|
|bash-4.2|1m41.934s|0m53.172s|
|ccache-3.1.7|0m13.600s|0m5.439s|
|iperf-2.0.5|0m17.192s|0m7.074s|

### Lion + Xcode 4.2 ###
Machine `MBP5,5/8GB+`
| | 1st run | 2nd run |
|:|:--------|:--------|
|aria2-1.14.1|6m15.232s|4m50.824s|
|libidn-1.24|0m54.116s|0m24.463s|
|pcre-8.21|0m38.341s|0m29.131s|
|redis-2.4.7|0m13.423s|0m10.813s|
|varnish-3.0.2| 1m4.423s| 0m55.807s|


### Snow Leopard + Xcode 4.2 ###
Machine `MB1,1`
| | 1st run | 2nd run |
|:|:--------|:--------|
|aria2-1.14.1|14m55.078s|  |
|bash-4.2|4m15.604s|1m56.844s|
|ccache-3.1.7|real	0m23.061s|0m10.242s|

## Rudix 2011 ##

### Lion + Xcode 4.2 ###
Machine `MBP5,5/8GB+`
| | 1st run | 2nd run |
|:|:--------|:--------|
|aria2-0.13.0|5m4.506s|4m28.906s|
|astyle-2.02|0m7.767s|0m7.559s|
|bash-4.2|1m26.527s|0m51.092s|
|boost-1.47.0|13m49.661s|13m56.328s|
|cabextract-1.4|0m11.738s|0m5.327s|
|cadaver-0.23.3|0m40.534s|0m19.842s|
|ccache-3.1.6|0m9.453s|0m4.459s|
| cflow-1.4|0m33.240s|0m11.834s|
| check-0.9.8|0m20.775s|0m13.390s|
|cscope-15.7a|0m19.369s|0m7.830s|
|ctags-5.8|0m15.437s|0m10.935s|
|coreutils-8.13|3m7.692s|1m27.826s|
|dialog-1.1-20110707|0m23.161s|0m8.906s|
|dtach-0.8|0m7.040s|0m1.941s|
|findutils-4.4.2|1m6.782s|0m28.865s|
|gettext-0.18.1.1|4m51.145s|4m12.926s|
|glib-2.28.8|2m47.803s|2m46.540s|
|lua-5.1.4|0m5.980s|0m4.476s|
|llcms2-2.2|0m43.288s|0m42.155s|
|libevent-2.0.15|0m49.849s|0m34.992s|
|libintl-0.18.1.1|1m6.975s|0m32.139s|
|libjpeg-8c|0m30.073s|0m26.770s|
|libmemcached-1.0.2|2m51.025s|2m35.723s|
|libpng-1.5.6|0m19.656s|0m16.171s|
|lzo-2.06|0m20.370s|0m11.863s|
|mc-4.8.0|1m29.705s|1m18.346s|
|memcached-1.4.9|0m13.807s|0m9.090s|
|pcre-8.20|0m46.851s|0m31.101s|
|pkg-config-0.25|0m39.153s|0m30.105s|
|protobuf-2.4.1|2m36.562s|2m27.373s|
|qemu-0.15.1|6m28.782s|  |
|redis-2.4.2|0m12.394s|0m11.634s|
|rsync-3.0.9|0m40.807s|0m16.170s|
|wget-1.13.4|1m34.153s|m30.088s|
|zsync-0.6.2|0m14.854s|0m10.820s|
|xz-5.0.3|0m36.826s|0m28.579s|

### Lion + Xcode 4.1 ###
Machine `MBP5,5/8GB+`
| | 1st run | 2nd run |
|:|:--------|:--------|
|aria2-0.12.0|5m29.799s|4m39.776s|
|aria2-0.12.1|4m52.203s|4m26.998s|
|astyle-2.0.2|0m8.267s|0m7.505s|
|cabextract-1.4|0m17.166s|0m6.993s|
|ccache-3.1.5|0m13.000s|0m5.729s|
|cflow-1.3|0m45.435s|0m15.616s|
|check-0.9.8|0m31.614s|0m19.686s|
|cscope-15.7a|0m27.683s|0m12.814s|
|ctags-5.8|0m21.978s|0m13.357s|
|dialog-1.1-20110707|0m27.974s|0m11.614s|
|dtach-0.8|0m11.281s|0m3.111s|
|findutils-4.4.2|1m8.125s|0m25.697s|
|gawk-4.0.0|0m32.597s|0m21.794s|
|gettext-0.18.1.1|7m20.699s|6m13.793s|
|git-1.7.6.1|1m32.317s|1m30.122s|
|gmp-5.0.2|1m31.400s|1m21.838s|
|libev-4.0.4|0m12.477s|0m6.704s|
|libevent-2.0.13|0m52.147s|0m36.009s|
|lighttpd-1.4.29|0m51.623s|0m30.804s|
|lua-5.1.4|0m4.382s|0m5.207s|
|libmemcached-0.51|1m35.682s|1m14.786s|
|libunistring-0.9.3|3m30.819s|3m7.990s|
|pcre-8.13|0m35.807s|0m31.215s|
|pkg-config-0.25|0m48.802s|0m31.424s|
|redis-2.2.12|0m15.385s|0m12.261s|
|varnish-3.0.1|1m2.375s|0m55.402s|
|wget-1.13.4|1m59.677s|0m31.412s|
|zsync-0.6.2|0m13.238s|0m10.647s|

### Snow Leopard + Xcode 4.0 ###
Machine MB1,1
| | 1st run | 2nd run |
|:|:--------|:--------|
|aria2-0.12.0|7m46.841s|6m57.686s |
|aria2-0.12.1|7m52.278s|6m57.821s|
|aria2-0.13.0|8m13.623s|7m30.829s|
|bash-4.2|2m54.596s|1m23.285s|
|cflow-1.3|0m40.512s | 0m15.279s|
|findutils-4.4.2|1m29.849s|0m36.017s|
|gawk-4.0.0|0m58.984s|0m40.364s|
|gettext-0.18.1.1|7m0.121s|5m52.582s|
|gmp-5.0.2|2m14.745s|2m0.536s|
|libintl-0.18.1.1|2m34.495s|1m53.622s|
|lua-5.1.4|0m10.916s|0m9.004s|

### Snow Leopard + Xcode 4 (Old) ###
| | `MB1,1` | `MB1,1` | `MBP5,5` | `MBP5,5` |  `MBP5,5/8GB` | `MBP5,5/8GB` |
|:|:--------|:--------|:---------|:---------|:--------------|:-------------|
|  | No config.cache | With config.cache | No config.cache | With config.cache |
|apr-1.4.5|2m47.597s|1m32.044s|1m10.766s|0m35.931s|
|apr-util-1.3.12|1m4.555s |0m52.938s |0m26.878s|0m19.829s|
|bash-4.1|  |  |1m42.523s|0m59.126s|
|cabextract-1.4|0m31.319s|0m13.282s|x |x |0m14.003s|0m5.610s|
|coreutils-8.9|4m6.545s|3m37.857s|
|gawk-4.0.0|1m54.271s|1m16.170s|
|iperf-2.0.5|0m36.922s|0m17.177s |  |  | 0m18.393s| 0m7.734s |
|lua-5.1.4|0m9.759s|  |0m7.228s|  |
|node-0.3.4|7m6.926s|N.A.|
|readline-6.1|0m47.754s|0m27.059s|
|tmux-1.5|1m38.772s|0m57.377s|- |- |0m29.727s|0m24.596s|
|yasm-1.1.0|  |  |0m37.157s|0m29.652s |
|zsync-0.6.2|0m17.971s|0m11.834s|

## Rudix 2010 ##
Snow Leopard + Xcode 3.
| | `MB1,1` | `MB1,1` | `MBP5,5` | `MBP5,5` |
|:|:--------|:--------|:---------|:---------|
|  | No config.cache | With config.cache | No config.cache | With config.cache |
|apr-1.3.6|1m24.028s|0m52.249s|
|apr-1.3.8|1m32.193s|0m56.453s|
|apr-1.4.2|1m44.969s|
|apr-util-1.3.8|0m37.331s|0m35.426s|
|apr-util-1.3.9|0m37.638s|0m29.520s|
|db-4.7.25|5m16.473s|4m53.583s|
|bash-4.0intel|1m16.101s|0m41.754s|
|bash-4.0|1m52.623s|  |
|bash-4.1|2m32.982s|1m16.749s|
|boost-1.43|
|ccache-2.4|0m7.540s|0m4.111s|0m7.354s|0m3.181s|
|ccache-3.0.1|0m13.666s|0m7.496s|
|coreutils-8.5|4m12.262s|2m21.640s|
|expat-2.0.1|0m23.640s|0m19.143s|
|gettext-0.17|7m18.061s|6m41.956s|
|gettext-0.18.1.1|7m55.515s|
|glib-2.20.4|4m41.823s|4m20.884s|
|guile-1.8.6|2m57.310s|2m12.790s|
|guile-1.8.7|3m0.401s|2m25.682s|
|git-1.6.3.3|1m46.063s|1m40.559s|
|gmp-4.3.1|6m9.634s|6m11.428s|
|gmp-4.3.2| 4m13.899s |	4m1.128s | 2m37.324s | 2m26.434s |
|lynx-2.8.7|1m48.575s|1m38.673s|1m34.932s|1m28.245s|
|lua-5.1.4|0m8.301s|0m7.686s|0m8.165s|0m6.452s|
|mc-4.6.1|1m12.013s|0m50.881s|
|pkgconfig-0.23|0m58.444s|0m45.413s|
|readline-6.0|0m30.144s|0m19.579s|
|varnish-2.0.4|0m57.984s|0m46.826s|0m53.055s|0m42.920s|
|wget-1.12|1m6.948s|0m33.069s|0m53.439s|0m20.500s|
|zsync-0.6.1|0m18.170s| 0m12.183s | 0m11.634s |0m8.552s |

## How to test ##
**First run
```
$ make clean prep
$ time make build
```** Second run
```
$ make clean prep
$ time make build
```