# Linux audio system setup
Status: DRAFT

<!-- MarkdownTOC depth=3-->

- [Base setup](#base-setup)
- [External links](#external-links)

<!-- /MarkdownTOC -->


## Base setup

 * [Compatitble audio interfaces and hardware](http://www.alsa-project.org/main/index.php/Matrix:Main)
 * Install Debian stable
 * Add kxstudio repos (see http://kxstudio.linuxaudio.org/Repositories): ` wget https://launchpad.net/~kxstudio-debian/+archive/kxstudio/+files/kxstudio-repos_9.0.0~kxstudio1_all.deb, sudo dpkg -i kxstudio-repos_9.0.0~kxstudio1_all.deb`
 * switch CPU Frequency scaling to Performance
 * realtimeconfigquickscan



https://bitbucket.org/thismaechler/ubuntustudio-14.04-realtimeaudio/src/74adbac5418c2bad6d52c2cd296f223c82d21649/HOWTO?at=master
https://bitbucket.org/thismaechler/ubuntustudio-14.04-realtimeaudio/src/74adbac5418c2bad6d52c2cd296f223c82d21649/cfg/rtirq?at=master

## External links

### Configuration
 * **[Pro Audio - ArchLinux Wiki](https://wiki.archlinux.org/index.php/Pro_Audio)**
 * [System Preparations](http://www.penguinproducer.com/2011/09/system-preparations/)
 * [System configuration [Linux-Sound]](http://wiki.linuxaudio.org/wiki/system_configuration)
 * [Linux audio user FAQ [Linux-Sound]](http://wiki.linuxaudio.org/faq/start)
 * [Jack Configuration on Focusrite USB Audio](https://bitbucket.org/thismaechler/ubuntustudio-14.04-realtimeaudio/src/74adbac5418c2bad6d52c2cd296f223c82d21649/HOWTO?at=master#HOWTO-88)
 * [List of JACK Frame [or Buffer] & Period settings ideal for USB interface](http://wiki.linuxaudio.org/wiki/list_of_jack_frame_period_settings_ideal_for_usb_interface)
 * [IRQ Prio config](https://bitbucket.org/thismaechler/ubuntustudio-14.04-realtimeaudio/src/74adbac5418c2bad6d52c2cd296f223c82d21649/HOWTO?at=master#HOWTO-179)
 * [PCI Latency Values - MythTV](https://www.mythtv.org/wiki/PCI_Latency)
 * [IRQ Priorities - FFADO](http://subversion.ffado.org/wiki/IrqPriorities)
 * [Setting CPU affinity](http://www.cyberciti.biz/tips/setting-processor-affinity-certain-task-or-process.html)
 * [Rtirq](http://alsa.opensrc.org/Rtirq) - bash script for tweaking IRQ priorities/audio latency
 * [How to optimize jack](http://wiki.linuxaudio.org/wiki/optimize_jack)
 * [Hardware Compatibility List [Linux-Sound]](http://wiki.linuxaudio.org/apps/categories/start?idx=hw)
 * **[Programming and using Linux sound](http://jan.newmarch.name/LinuxSound/)**
 * [The LADI Session Handler](http://www.penguinproducer.com/Blog/2011/12/the-ladi-session-handler/)
 * [Audio Layers Overview [Linux-Sound]](http://wiki.linuxaudio.org/wiki/audio_layers_overview)
 * [Gentoo Pro-Audio Overlay](http://proaudio.tuxfamily.org/wiki/index.php?title=Main_Page) - Pro-audio support for Gentoo users 


##### Misc

 * Firewire config for DV cameras: `modprobe ieee1394 ohci1394 raw1394 video1394 #possibly mknod -m 666 /dev/video1394 c 172 0`
 * Burn MPEG-1/VCD to CD: `cdrdao write --device 0,1,0 -n vcd.toc #vcd.toc from mkvcdfs`



### Development

 * **[Real-Time Linux Wiki](https://rt.wiki.kernel.org/index.php/Main_Page)**
  * [Real-Time Linux kernels](https://www.kernel.org/pub/linux/kernel/projects/rt/)
  * [Brain Fuck Scheduler](https://en.wikipedia.org/wiki/Brain_Fuck_Scheduler) - [Con Kolivas patches](http://ck.kolivas.org/patches/bfs/4.0/4.1/)
 * [Real-time computing - Wikipedia](https://en.wikipedia.org/wiki/Real-time_computing)
 * [Activate and test realtime kernels - Gentoo ProAudioOverlay](http://proaudio.tuxfamily.org/wiki/index.php?title=Realtime_%28RT%29_Kernel#Activate_and_test_RT)
 * [Realtime - Ubuntu Wiki](https://wiki.ubuntu.com/RealTime?highlight=%28realtime%29)
 * [Google search: Real Time Linux on linuxjournal.com](https://www.google.com/?q=Real+Time+Linux+site:http:%2F%2Fwww.linuxjournal.com%2F)
 * [Low Latency Howto - ALSA Project](http://www.alsa-project.org/main/index.php/Low_latency_howto)
 * [Realtime Linux Audio Kernels - linuxaudio.org](http://wiki.linuxaudio.org/wiki/kernel/start) - support for packagers, vendors and users
 * [Ubuntu Realtime kernels](https://wiki.ubuntu.com/RealTime?highlight=%28realtime%29)
 * [rtaudio](https://github.com/thestk/rtaudio) -  A set of C++ classes that provide a common API for realtime audio input/output across Linux (native ALSA, JACK, PulseAudio and OSS), Macintosh OS X (CoreAudio and JACK), and Windows (DirectSound, ASIO, and WASAPI) operating systems. 
 * [openAudioProgrammingTutorials](https://github.com/harryhaaren/openAudioProgrammingTutorials) -  A tutorial style set of programs that will hopefully assist beginner programmers get familiar with the Linux Audio scene
