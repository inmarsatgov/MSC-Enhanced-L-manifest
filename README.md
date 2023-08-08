# MSC repo manifest
- Forked from [c444-manifest](https://github.com/WinSystems/c444-manifest)
- MSC branch ```msc-5.15```
- MSC manifest ```itx-p-c444_msc_5.15.32.xml```

# Usage
```console
repo init -u git@github.com:inmarsatgov/MSC-Enhanced-L-manifest.git -b msc-5.15 -m itx-p-c444_msc_5.15.32.xml
repo sync -j4
```

# Yocto Layers

# Summary

| layer                     |     path                                                            | priority |
| ------------------------- | ------------------------------------------------------------------- | -------- |
| meta                      | /home/msc-build/msc/build/sources/poky/meta                         | 5        |
| meta-poky                 | /home/msc-build/msc/build/sources/poky/meta-poky                    | 5        |
| meta-oe                   | /home/msc-build/msc/build/sources/meta-openembedded/meta-oe         | 5        |
| meta-multimedia           | /home/msc-build/msc/build/sources/meta-openembedded/meta-multimedia | 5        |
| meta-python               | /home/msc-build/msc/build/sources/meta-openembedded/meta-python     | 5        |
| meta-freescale            | /home/msc-build/msc/build/sources/meta-freescale                    | 5        |
| meta-freescale-3rdparty   | /home/msc-build/msc/build/sources/meta-freescale-3rdparty           | 4        |
| meta-freescale-distro     | /home/msc-build/msc/build/sources/meta-freescale-distro             | 4        |
| meta-bsp                  | /home/msc-build/msc/build/sources/meta-imx/meta-bsp                 | 8        |
| meta-sdk                  | /home/msc-build/msc/build/sources/meta-imx/meta-sdk                 | 8        |
| meta-ml                   | /home/msc-build/msc/build/sources/meta-imx/meta-ml                  | 8        |
| meta-chromium             | /home/msc-build/msc/build/sources/meta-browser/meta-chromium        | 7        |
| meta-clang                | /home/msc-build/msc/build/sources/meta-clang                        | 7        |
| meta-gnome                | /home/msc-build/msc/build/sources/meta-openembedded/meta-gnome      | 5        |
| meta-perl                 | /home/msc-build/msc/build/sources/meta-openembedded/meta-perl       | 5        |
| meta-networking           | /home/msc-build/msc/build/sources/meta-openembedded/meta-networking | 5        |
| meta-filesystems          | /home/msc-build/msc/build/sources/meta-openembedded/meta-filesystems| 5        |
| meta-nxp-demo-experience  | /home/msc-build/msc/build/sources/meta-nxp-demo-experience          | 7        |
| meta-qt6                  | /home/msc-build/msc/build/sources/meta-qt6                          | 5        |
| meta-python2              | /home/msc-build/msc/build/sources/meta-python2                      | 7        |
| meta-tpm                  | /home/msc-build/msc/build/sources/meta-security/meta-tpm            | 10       |
| meta-winsys               | /home/msc-build/msc/build/sources/meta-winsys                       | 11       |


## poky
 - path: ```sources/poky```
 - repo: ```https://git.yoctoproject.org/poky```
 - revision: ```27de52e402ae000dfa502d52908cd6e6aef923ec```
 - upstream: ```kirkstone```
 - last commit: ```Wed Apr 27 11:09:57 2022 +0200```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 946   |
| ```*.bbclass```  | 213   |
| ```*.bbappend``` | 14    |


Reference distribution of the Yocto project
- contains ```bitbake```, ```OpenEmbedded Core```
- starting point for building your own OS distribution
- no binary files, all builds are from source

Poky [releases](https://wiki.yoctoproject.org/wiki/Releases)
MSC is based on the ```Kirkstone ``` release.


### Directories
```
├── bitbake            : bitbake python package
├── contrib            : plugins etc
├── documentation      : Yocto Project documentation
├── meta               : the core metadata - this is the key port of poky
|                        Definition of machines, the poky distribution, and
|                        the packages that make up a given system
├── meta-poky          : busybox, psplash, tiny-init
├── meta-selftest      : test layer used by scripts/oe-selftest
├── meta-skeleton      : example recipes and configuration files
├── meta-yocto-bsp     : details about using the Yocto Project hardware
|                        reference BSPs
├── oe-init-build-env  : 
└── scripts            : 
```

## meta-openembedded
 - path: ```sources/meta-openembedded```
 - repo: ```https://github.com/openembedded/meta-openembedded```
 - revision: ```5357c7a40eaf8d1bcf7ff58edbba8e9527e40c7d```
 - upstream: ```kirkstone```
 - last commit: ```Wed Apr 27 09:23:51 2022 -0700```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 1941  |
| ```*.bbclass```  | 24    |
| ```*.bbappend``` | 4     |

Collection of layers for the OE-core universe. This repository is a collection
of layers to suppliment OE-Core with additional packages, Each layer have
designated maintainer.

```
├── contrib
├── COPYING.MIT
├── meta-filesystems
├── meta-gnome
├── meta-initramfs
├── meta-multimedia
├── meta-networking
├── meta-oe
├── meta-perl
├── meta-python
├── meta-webserver
├── meta-xfce
└── README
```

## meta-security
 - path: ```sources/meta-security```
 - repo: ```https://git.yoctoproject.org/meta-security```
 - revision: ```c79262a30bd385f5dbb009ef8704a1a01644528e```
 - upstream: ```kirkstone```
 - last commit: ```-```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 100   |
| ```*.bbclass```  | 8     |
| ```*.bbappend``` | 12    |

Provides security tools, hardening tools for Linux kernels and libraries for
implementing security mechanisms.

## meta-python2
 - path: ```sources/meta-python2```
 - repo: ```https://git.openembedded.org/meta-python2```
 - revision: ```f02882e2aa9279ca7becca8d0cedbffe88b5a253```
 - upstream: ```kirkstone```
 - last commit: ```Tue Feb 22 10:12:36 2022 +0100```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 313   |
| ```*.bbclass```  | 6     |
| ```*.bbappend``` | 0     |

## meta-qt6
 - path: ```sources/meta-qt6```
 - repo: ```https://code.qt.io/yocto/meta-qt6.git```
 - revision: ```b2894aad5c1aaa85f2f5c7b94391b7c51c39e555```
 - upstream: ```6.3```
 - last commit: ```Thu Apr 28 06:34:09 2022 +0000```
 - used by MSC: ```no```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 50    |
| ```*.bbclass```  | 6     |
| ```*.bbappend``` | 0     |

## meta-browser
 - path: ```sources/meta-browser```
 - repo: ```https://github.com/OSSystems/meta-browser/```
 - revision: ```d25d8ee98a656b2534d0eec6138ef264529fab4f```
 - upstream: ```N/A```
 - last commit: ```Mon Dec 20 08:07:38 2021 +0100```
 - used by MSC: ```no```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 98    |
| ```*.bbclass```  | 1     |
| ```*.bbappend``` | 0     |

Chromium and Firefox

## meta-clang
 - path: ```sources/meta-clang```
 - repo: ```https://github.com/kraj/meta-clang```
 - revision: ```85d956d95401479ca666139e31f662f60c156d5f```
 - upstream: ```kirkstone```
 - last commit: ```Fri Apr 29 10:40:55 2022 -0700```
 - used by MSC: ```TBD```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 18    |
| ```*.bbclass```  | 3     |
| ```*.bbappend``` | 23    |

clang/llvm as alternative to system C/C++ compiler for OpenEmbedded/Yocto 
Project based distributions. This can cohabit with GNU compiler and can be used
for specific recipes or full system compiler.

## meta-freescale
 - path: ```sources/meta-freescale"```
 - repo: ```https://github.com/Freescale/meta-freescale```
 - revision: ```2fb1ce365338126aad365012ebb913b3e4a9f1be```
 - upstream: ```kirkstone```
 - last commit: ```Sat Apr 30 11:50:37 2022 -0300```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 151   |
| ```*.bbclass```  | 15    |
| ```*.bbappend``` | 39    |

Support for Freescale's platforms for use with OpenEmbedded and/or Yocto.

## meta-freescale-3rdparty
 - path: ```sources/meta-freescale-3rdparty```
 - repo: ```https://github.com/Freescale/meta-freescale-3rdparty```
 - revision: ```de0eb1408150d77f9cce97c559f9a5a3c71e5d6c```
 - upstream: ```kirkstone```
 - last commit: ```Mon Apr 25 08:44:34 2022 -0300```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 31    |
| ```*.bbclass```  | 1     |
| ```*.bbappend``` | 12    |

Support for Freescale's ARM based platforms for use with OpenEmbedded and/or
Yocto Freescale's BSP layer.

## meta-freescale-distro
 - path: ```sources/meta-freescale-distro```
 - repo: ```https://github.com/Freescale/meta-freescale-distro```
 - revision: ```fc15f5003043da23212596be7366ae2547c308ad```
 - upstream: ```kirkstone```
 - last commit: ```Sat Apr 30 11:52:51 2022 -0300```
 - used by MSC: ```TBD```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 25    |
| ```*.bbclass```  | 0     |
| ```*.bbappend``` | 2     |

Support for Freescale's Demonstration images for use with OpenEmbedded and/or
Yocto Freescale's BSP layer.

## fsl-community-bsp-base
 - path: ```sources/base```
 - repo: ```https://github.com/Freescale/fsl-community-bsp-base```
 - revision: ```60f79f7af60537146298560079ae603260f0bd14```
 - upstream: ```kirkstone```
 - last commit: ```Mon Jul 12 11:23:41 2021 -050```
 - used by MSC: ```-```
| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 0     |
| ```*.bbclass```  | 0     |
| ```*.bbappend``` | 0     |

Contains ```setup-environment``` and ```README```
bblayers
```
  sources/poky/meta
  sources/poky/meta-poky
  sources/meta-openembedded/meta-oe
  sources/meta-openembedded/meta-multimedia
  sources/meta-openembedded/meta-python
  sources/meta-freescale
  sources/meta-freescale-3rdparty
  sources/meta-freescale-distro
```

## meta-imx
 - path: ```sources/meta-imx```
 - repo: ```https://github.com/nxp-imx/meta-imx```
 - revision: ```refs/tags/rel_imx_5.15.32_2.0.0```
 - upstream: ```N/A```
 - last commit: ```Thu May 25 12:07:40 2023 +0200 (Active)```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 148   |
| ```*.bbclass```  | 7     |
| ```*.bbappend``` | 88    |

i.MX Linux Yocto Project BSP 5.15.32_2.0.0 Release
Contains ```imx-setup-release.sh```

## meta-timesys
 - path: ```sources/meta-timesys```
 - repo: ```https://github.com/TimesysGit/meta-timesys```
 - revision: ```edce180f0389a13e678cb0edafb7f8980648e1a4```
 - upstream: ```N/A```
 - last commit: ```Tue Feb 1 11:59:22 2022 -0800```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 0     |
| ```*.bbclass```  | 2     |
| ```*.bbappend``` | 0     |

Scripts for image manifest generation used for security monitoring and
notification as part of the Timesys Vigiles product offering. Vigiles is a
vulnerability management tool that provides build-time Yocto CVE Analysis of
target images. It does this by collecting metadata about packages to be
installed and uploading it to be compared against the Timesys CVE database.

## meta-winsys
 - path: ```sources/meta-winsys```
 - repo: ```https://github.com/WinSystems/meta-winsys```
 - revision: ```itx-p-c444_5.15.32```
 - upstream: ```N/A```
 - last commit: ```Thu Jun 1 18:24:08 2023 +0000 (Active)```
 - used by MSC: ```yes```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 19    |
| ```*.bbclass```  | 0     |
| ```*.bbappend``` | 10    |

Contains ```winsys-setup-release.sh```

## meta-nxp-demo-experience
 - path: ```sources/meta-nxp-demo-experience```
 - repo: ```https://github.com/nxp-imx-support/meta-nxp-demo-experience```
 - revision: ```8fade3993b832ecd823771644f2a7b731f8f4527```
 - upstream: ```kirkstone```
 - last commit: ```Thu Apr 28 08:06:25 2022 -0700```
 - used by MSC: ```no```

| Extension        | Count |
| ---------------- | ----- |
| ```*.bb```       | 1     |
| ```*.bbclass```  | 0     |
| ```*.bbappend``` | 1     |

Holds all the needed configuration to build the i.MX demos as well as the i.MX
Demo Launcher interface

# References
 - [c444 Yocto Build Guide 5.15](https://github.com/WinSystems/c444-manifest/wiki/BSP-Documentation-5.15)
