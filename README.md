linux-3.10.33-chromeos
======================

kernel_next chromeos kernel using upstream sources and 3.4 wifi stack

Background: I installed the latest 3.13 upstream kernel on my Acer c720
Chromebook running ubuntu, but wifi would not work using the ath9k driver
I learned that the latest supported kernel for native ChromwOS is
3.10, using the 3.4 wifi stack.

I tried compiling kernel_next sources gitted from the ChromeOS repo
but they severly failed to even compile when trying to make a debian
kernel package.

I downloaded upstream kernel sources, latest 3.10 and 3.4 and tried
compiling those, but there were some inconsistencies with 3.4 files
not building under 3.10. I copied some 3.4 files from kernel_next which
then allowed compilation to procede. 

The kernel now compiles and debs are built, but further testing remains.