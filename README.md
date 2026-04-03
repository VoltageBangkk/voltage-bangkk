# Guide Build for Voltage OS Moto G84 (bangkk)
Learn how to build voltage OS for bangkk easily

![descrição](voltage.jpg)
# 
Ceate Voltage directory
```
mkdir ~/voltage
cd ~/voltage
```
# 
Synchronizing source
```
#repo-init
repo init -u https://github.com/VoltageOS/manifest.git -b 16.2 --git-lfs

#sync
repo sync -c -j6 --force-sync --no-clone-bundle --no-tags
```
# 
Cloning tree
```
#nfc
git clone https://github.com/VoltageBangkk/android_hardware_samsung_slsi_nfc.git -b 16.2 hardware/samsung/slsi/nfc

#vendor-common
git clone https://github.com/VoltageBangkk/proprietary_vendor_motorola_sm6375-common.git -b 16.2 vendor/motorola/sm6375-common

#vendor
git clone https://github.com/VoltageBangkk/proprietary_vendor_motorola_bangkk.git -b 16.2 vendor/motorola/bangkk

#kernel
git clone https://github.com/VoltageBangkk/android_kernel_motorola_sm6375.git -b 16.2 kernel/motorola/sm6375

#hardware
git clone https://github.com/VoltageBangkk/android_hardware_motorola.git -b 16.2 hardware/motorola

#device-common
git clone https://github.com/VoltageBangkk/android_device_motorola_sm6375-common.git -b 16.2 device/motorola/sm6375-common

#device
git clone https://github.com/VoltageBangkk/android_device_motorola_bangkk.git -b 16.2 device/motorola/bangkk

#dolby
git clone https://github.com/VoltageBangkk/vendor_sony_dolby.git -b 16.2 vendor/sony/dolby
```
# 
Build
```
. build/envsetup.sh
brunch bangkk
```
# 
Adding maintainer & SmartPixels to build
https://github.com/ZedissPp/android_device_motorola_bangkk/commit/99c61ef91343f0ec0f8e5f09b0edaa7e188dfa00
#
and
#
https://github.com/ZedissPp/android_device_motorola_bangkk/commit/b3a57db11c73ed47e48ccb9f46b1a17e863a6ba9
# 
GApps
https://github.com/MindTheGapps/16.0.0-arm64/releases
# 
build guide by [ZedissPp](https://github.com/ZedissPp)
Come say hi in our Telegram group!
https://t.me/zedisspechat
