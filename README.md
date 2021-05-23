# Mastering Embedded Linux Programming – Third Edition

<a href="https://www.packtpub.com/product/mastering-embedded-linux-programming-third-edition/9781789530384?utm_source=github&utm_medium=repository&utm_campaign=9781789530384"><img src="https://static.packt-cdn.com/products/9781789530384/cover/smaller" alt="Mastering Embedded Linux Programming – Third Edition" height="256px" align="right"></a>

This is the code repository for [Mastering Embedded Linux Programming – Third Edition](https://www.packtpub.com/product/mastering-embedded-linux-programming-third-edition/9781789530384?utm_source=github&utm_medium=repository&utm_campaign=9781789530384), published by Packt.

**Create fast and reliable embedded solutions with Linux 5.4 and the Yocto Project 3.1 (Dunfell)**

## What is this book about?
Embedded Linux runs many of the devices we use every day. From smart TVs and Wi-Fi routers to test equipment and industrial controllers, all of them have Linux at their heart. The Linux OS is one of the foundational technologies comprising the core of the Internet of Things (IoT). This book starts by breaking down the fundamental elements that underpin all embedded Linux projects: the toolchain, the bootloader, the kernel, and the root filesystem. After that, you will learn how to create each of these elements from scratch and automate the process using Buildroot and the Yocto Project.

This book covers the following exciting features: 
* Use Buildroot and the Yocto Project to create embedded Linux systems
* Troubleshoot BitBake build failures and streamline your Yocto development workflow
* Update IoT devices securely in the field using Mender or balena
* Prototype peripheral additions by reading schematics, modifying device trees, soldering breakout boards, and probing pins with a logic analyzer
* Interact with hardware without having to write kernel device drivers

If you feel this book is for you, get your [copy](https://www.amazon.com/dp/1789530385) today!

## Instructions and Navigations
All of the code is organized into folders. For example, Chapter02.

The code will look like the following:
```
if (test expression)
{
  Statement upon condition is true
}
```

**Following is what you need for this book:**
If you’re a systems software engineer or system administrator who wants to learn Linux implementation on embedded devices, then this book is for you. Embedded systems engineers accustomed to programming for low-power microcontrollers can use this book to help make the leap to high-speed systems on chips that can run Linux. Anyone responsible for developing new hardware that needs to run Linux will also find this book useful. Basic working knowledge of the POSIX standard, C programming, and shell scripting is assumed.

With the following software and hardware list you can run all code examples present in the book (Chapter 1-21).

### Software and Hardware List

| Chapters                      | Software/Hardware Required  | OS Required                   |
| ----------------------------- | --------------------------- | ----------------------------- |
| 3, 4, 5, 6, 9, 11, 12, 15, 21 | BeagleBone Black            | Not Applicable |
| 4, 6, 7, 10, 14, 19, 20       | Raspberry Pi 4              | Not Applicable |
| 4, 5, 6                       | QEMU (32-bit arm)           | Linux (Any) |
| 7, 8, 10, 13, 19, 21          | Yocto Project 3.1 (Dunfell) | Compatible Linux Distribution |
| 6, 12, 13, 14, 19, 20, 21     | Buildroot 2020.02 LTS       | Linux (Any) |
| 2, 3, 4, 5                    | Crosstool-NG 1.24.0         | Linux (Any) |
| 3, 9                          | U-Boot v2021.01             | Linux (Any) |
| 4                             | Linux Kernel 5.4            | Linux (Any) |

We also provide a PDF file that has color images of the screenshots/diagrams used in this book. [Click here to download it](http://www.packtpub.com/sites/default/files/downloads/9781789530384_ColorImages.pdf).

## Errata

**Page 26**: The `crosstool-ng-1.24.0` tag of crosstool-ng no longer builds because its `expat-2.2.6` dependency has been removed from SourceForge due to a security vulnerability. The fix is to checkout a later commit that upgrades this dependency to `expat-2.3.0`.

```bash
$ git clone https://github.com/crosstool-ng/crosstool-ng.git
$ cd crosstool-ng
$ git checkout 0528a9d744cc95aac3df40d5a1666f0a1051cf5d
$ ./bootstrap
$ ./configure --prefix=${PWD}
$ make
$ make install
```

When crosstool-ng maintainers tag a release after 1.24.0 readers should upgrade to that.

## Related products <Other books you may enjoy>
* Linux Device Drivers Development  [[Packt]](https://www.packtpub.com/product/linux-device-drivers-development/9781785280009?utm_source=github&utm_medium=repository&utm_campaign=9781785280009) [[Amazon]](https://www.amazon.com/dp/1785280007)

* Hands-On RTOS with Microcontrollers [[Packt]](https://www.packtpub.com/product/hands-on-rtos-with-microcontrollers/9781838826734?utm_source=github&utm_medium=repository&utm_campaign=9781838826734) [[Amazon]](https://www.amazon.com/dp/1838826734)

## Get to Know the Authors
**Frank Vasquez** is an embedded Linux engineer at Lunar Energy. He has over a decade of experience designing and building embedded Linux systems. During that time, he has shipped numerous devices including a rackmount DSP audio server, a diver-held sonar camcorder, and a consumer IoT hotspot. Before his career as an embedded Linux engineer, Frank was a database kernel developer at IBM where he worked on Db2. He lives in Silicon Valley.

**Chris Simmonds** is a software consultant and trainer living in southern England. He has almost two decades of experience in designing and building open-source embedded systems. He is the founder and chief consultant at 2net Ltd, which provides professional training and mentoring services in embedded Linux, Linux device drivers, and Android platform development. He has trained engineers at many of the biggest companies in the embedded world, including ARM, Qualcomm, Intel, Ericsson, and General Dynamics. He is a frequent presenter at open source and embedded conferences, including the Embedded Linux Conference and Embedded World.

## Other books by the authors
* [Mastering Embedded Linux Programming - Second Edition](https://www.packtpub.com/product/mastering-embedded-linux-programming-second-edition/9781787283282?utm_source=github&utm_medium=repository&utm_campaign=9781787283282)
* [Mastering Embedded Linux Programming](https://www.packtpub.com/product/mastering-embedded-linux-programming/9781784392536?utm_source=github&utm_medium=repository&utm_campaign=9781784392536)
