# yocto-BBB-simple
Ongoing collection of simple Yocto build files for BBB

<h3>sato-sdk-chromuium-A</h3>

<strong>sato-sdk-chromium-A</strong> is a sato build with a chromium WEB Browser, gcc, nano and others that work on a BeagleBone Black.

<h3>sato-sdk-chromium-LAMP</h3>

<strong>sato-sdk-chromium-LAMP</strong> is a sato build with a chromium Web Browser and Apache, PHP, MariaDB and PhpMyAdmin. It also has gcc, nano and the other things from the previous, -A build, listed above.

NOTE: Sound does not seem to be working.

This build works on the BeagleBone Black and the x86-64 platform. The x86-64 took many hours to build; much, much longer than the BBB. Neither system has sound with the current configuration files. The only change between these two machine was to build them with their specific MACHINE name:
- beaglebone-yocto
- genericx86-64

The x86-64 build, while running from a USB stick, on my fastest machine, was very snappy and the browser looked nice. A dual monitor setup created one big display window that had each half on a seperate display in a side by side layout. Unplugging one monitor fixed that but it was very interesting to see it layed out that way.


