Getting started
---------------
To initialize your local repository using the ThinkingBridge trees, use a command like this:

    repo init -u git://github.com/ThinkingBridge/platform_manifest.git -b jb-mr1

then

    repo sync -j16


Building the ROM
------------------------

To build ThinkingBridge you must cd to the working directory.

Now you can run the build script:

    ./build-tb.sh -device- -sync- -thread-


* device: Choose between the following supported devices: 
   - Build All Devices (all)
   - Nexus S (crespo)
   - Wifi Nexus 7 (grouper)
   - Galaxy S2 Alt (i9100g)
   - Galaxy S2 (i9100) # Not ready
   - Int. Galaxy S3 (i9300)
   - Galaxy Nexus (maguro)
   - Nexus 4 (mako)
* sync: Will sync latest ThinkingBridge sources before building
* threads: Allows to choose a number of threads for syncing and building operation.



You might want to consider using CCACHE to speed up build time after the first build.

This will make a signed flashable zip file located in out/target/product/-device-/thinkingbridge_DEVICE_VERSION.NO_DATE.zip

Example: /out/target/product/crespo/thinkingbridge_crespo_stable_20130101.zip
