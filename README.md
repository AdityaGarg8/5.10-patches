mbp-16.1-linux-wifi - 5.10.x
==============

Arch Linux package for Linux kernel with bleeding edge 2018+ MacBook Pro support.

This is a very unsupported quick fix to get Wifi working on some MBP devices using the Corellium patch from here (https://github.com/corellium/linux-m1/commit/02ad06fbf2b35916ee329a9bb80d73840d6e2973.patch?branch=02ad06fbf2b35916ee329a9bb80d73840d6e2973&diff=unified) and Aunali1's fantastic work here (https://github.com/aunali1/linux-mbp-arch). 

In order to get the patch to apply cleanly I've needed to remove some of the patches to support other BRCM devices in the various Macbooks. I've tested this on an MBP16.1, it should work on other models with the BCM4364 and BCM4377.

You should be able to use this directly on Arch or Manjaro as below. 

This repo has been updated so you should no longer have to remove any patches yourself if attempting a build on another distro.

    git clone https://github.com/AdityaGarg8/5.10-patches.git
    cd 5.10-patches
    makepkg -si


