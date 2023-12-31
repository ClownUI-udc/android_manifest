
![banner](https://raw.githubusercontent.com/kutemeikito/Ryzen-Script/master/clownui.png)
# ClownUI

## Getting Started ## 
---------------
To get started with the ClownUI sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

### Requirements
- Around 500GB disk space.
- Around 16+GB RAM running Linux.

To initialize your local repository, use command:

```bash
repo init -u https://github.com/ClownUI/android_manifest.git -b udc
```

## Then sync up: ##

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###

```bash
. build/envsetup.sh
lunch clown_$devicecodename-userdebug
make clown -j$(nproc --all) | tee log.txt
```

-----------------------------------------------------------------------------
Credits:
=======
 * [**CAF**](https://source.codeaurora.org)
 * [**AOSP**](https://android.googlesource.com)
 * [**ProtonPlus**](https://github.com/protonplus-org)
 * [**SuperiorOS**](https://github.com/SuperiorOS)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**Xdroid OSS**](https://github.com/xdroid-oss)
 * [**AncientOS**](https://github.com/ancient-lab)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**PixelOS**](https://github.com/PixelOS-AOSP)
 * [**ProjectBlaze**](https://github.com/ProjectBlaze)
 * [**Derpfest**](https://github.com/DerpFest-AOSP)
 * [**ColtOS**](https://github.com/Colt-Enigma)
 * [**EvolutionX**](https://github.com/Evolution-X)
-----------------------------------------------------------------------------
