# Voltage OS Moto G84 5G
building Voltage for bangkk

# 
# 
First, we create Voltage directory
```
mkdir ~/voltage && cd ~/voltage
```
Repo Init
```
repo init -u https://github.com/VoltageOS/manifest.git -b 16.2 --git-lfs
```
Sync
```
repo sync -c -j6 --force-sync --no-clone-bundle --no-tags
```

# 
# 
# Cloning tree


NFC
```
git clone https://github.com/VoltageBangkk/android_hardware_samsung_slsi_nfc.git -b 16.2 hardware/samsung/slsi/nfc
```
Vendor common
```
git clone https://github.com/VoltageBangkk/proprietary_vendor_motorola_sm6375-common.git -b 16.2 vendor/motorola/sm6375-common
```
Vendor
```
git clone https://github.com/VoltageBangkk/proprietary_vendor_motorola_bangkk.git -b 16.2 vendor/motorola/bangkk
```
Dolby
```
git clone https://github.com/VoltageBangkk/vendor_sony_dolby.git -b 16.2 vendor/sony/dolby
```
Kernel
```
git clone https://github.com/VoltageBangkk/android_kernel_motorola_sm6375.git -b 16.2 kernel/motorola/sm6375
```
Hardware
```
git clone https://github.com/VoltageBangkk/android_hardware_motorola.git -b 16.2 hardware/motorola
```
Device Common
```
git clone https://github.com/VoltageBangkk/android_device_motorola_sm6375-common.git -b 16.2 device/motorola/sm6375-common
```
Device
```
git clone https://github.com/VoltageBangkk/android_device_motorola_bangkk.git -b 16.2 device/motorola/bangkk
```
# 
# 
# Build
```
. build/envsetup.sh
  ```
```
brunch bangkk
```
# 
# 
# Adding maintainer name to build
https://github.com/VoltageOS/packages_apps_Settings/compare/16.2...VoltageBangkk:packages_apps_Settings:16.2
# 
