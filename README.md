# Voltage OS Moto G84 5G
building Voltage for bangkk

# First, we create Voltage directory
```
mkdir ~/voltage && cd ~/voltage
```
# Repo Init
```
repo init -u https://github.com/VoltageOS/manifest.git -b 16.2 --git-lfs
```

# NFC
```
git clone https://github.com/VoltageBangkk/android_hardware_samsung_slsi_nfc.git -b 16.2 hardware/samsung/slsi/nfc
```
# Vendor common
```
git clone https://github.com/VoltageBangkk/proprietary_vendor_motorola_sm6375-common.git -b 16.2 vendor/motorola/sm6375-common
```
