These are the elements we want built:

	chromium-x11 \
	alsa-lib \
	pulseaudio \
	mpeg2dec \
	gstreamer1.0 \
	nano \
	libexif \
	gcc \
	aspell \
	x11vnc"
  
  The chromuim app is the browser that is working in this build. This build requires the Browser app to be started from a terminal window with the command:
  chromium --no-sandbox
  
  The Layers to do this are:
  
  /home/michael/MoySandbox/yocto/poky/meta \
  /home/michael/MoySandbox/yocto/poky/meta-poky \
  /home/michael/MoySandbox/yocto/poky/meta-yocto-bsp \
  /home/michael/MoySandbox/yocto/poky/meta-python2 \
  /home/michael/MoySandbox/yocto/poky/meta-openembedded/meta-oe \
  /home/michael/MoySandbox/yocto/poky/meta-openembedded/meta-python \
  /home/michael/MoySandbox/yocto/poky/meta-clang \
  /home/michael/MoySandbox/yocto/poky/meta-browser \
  
This is what a previous build looked like. Notice the git branches used:

michael@yocto:~/MoySandbox/yocto/poky/build$ 
michael@yocto:~/MoySandbox/yocto/poky/build$ 
michael@yocto:~/MoySandbox/yocto/poky/build$ bitbake core-image-sato
Loading cache: 100% |                                                                                                            | ETA:  --:--:--
Loaded 0 entries from dependency cache.
Parsing recipes: 100% |###########################################################################################################| Time: 0:00:32
Parsing of 2338 .bb files complete (0 cached, 2338 parsed). 3778 targets, 110 skipped, 0 masked, 0 errors.
NOTE: Resolving any missing task queue dependencies

Build Configuration:
BB_VERSION           = "1.48.0"
BUILD_SYS            = "x86_64-linux"
NATIVELSBSTRING      = "universal"
TARGET_SYS           = "arm-poky-linux-gnueabi"
MACHINE              = "beaglebone-yocto"
DISTRO               = "poky"
DISTRO_VERSION       = "3.2"
TUNE_FEATURES        = "arm vfp cortexa8 neon callconvention-hard"
TARGET_FPU           = "hard"
meta                 
meta-poky            
meta-yocto-bsp       = "gatesgarth:9b58e1d1a87c1b33b180f71799cb32b3ce31211e"
meta-python2         = "gatesgarth:27d2aebdb4d78a608798a4f617d9bcfcbe4a635b"
meta-oe              
meta-python          = "gatesgarth:b9dcf17700014dec679307dc1247882dccd439ca"
meta-clang           = "master:1dfc3a905ad0fed7a3b300aa51153365f9950fe7"
meta-browser         = "master:1aef1b7857bc065c0e350c5732c3f0d69572e9ec"


