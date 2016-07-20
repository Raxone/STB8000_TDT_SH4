# STB8000_TDT_SH4
This is version Duckbox TDT SH4 for Albis STB8000(ufs913).

This build or (https://github.com/Duckbox-Developers) is not builds for final firmware.

This builds if for easy build and modified driver,kernel or python plugin for enigma and put/change in basic HDMU or another firmware for ufs913 etc.

My version of builds is modified kernel and drivers for albis8000 and need HDMU firmware for ufs913.

In ufs913 HDMU firmware change drivers and kernel to work on albis8000.

How To..
1. Clone git repo

    git clone https://github.com/Raxone/STB8000_TDT_SH4.git

2. cd STB8000_TDT_SH4

3. Install dependency
    
    sudo ./prepare4cdk.sh 

4. cd STB8000_TDT_SH4/cdk

5. make dir cdk/root/boot and put in boot dir audio.elf and video.elf from stb and rename it in audio_7105.elf and video_7105.elf

6. Configure and build
    ./make.sh

28

5

y

2

4

1

1

make crosstool driver -j4

(To build kernel,toolchain and driver configured for Albis Stb8000)

or

make yaud-enigma2-pli-nightly -j4

(-j4 = use 4 cpu core if got more set it -j8)
(this build all)


Choose between the following revisions:
========================================================================================================
 0) Newest                 - E2 OpenPli gstreamer / libplayer3    (Can fail due to outdated patch)     
========================================================================================================
 1) Use your own e2 git dir without patchfile
========================================================================================================
 2) Mon, 17 Aug 2015 07:08 - E2 OpenPli gstreamer / libplayer3 cd5505a4b8aba823334032bb6fd7901557575455
========================================================================================================
Media Framework : gstreamer
External LCD    : no
Select          : 2

On error try rerun.
