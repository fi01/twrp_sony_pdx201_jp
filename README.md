TWRP Device Tree for Xperia 10 II (JP)
====
- Based on [TWRP for Xperia 10 II](https://github.com/sjllls/twrp_sony_pdx201) By Sjll.
- Supports [FBE (File-Based Encryption)](https://source.android.google.cn/security/encryption/file-based) decryption
- System/Vendor prebuilt files extracted from XQ-AU42 (59.0.A.11.52)

## Get source
TWRP repository
```sh
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
repo sync -j2
```
device tree for Xperia 10 II (JP)
```sh
git clone https://github.com/fi01/twrp_sony_pdx201_jp.git -b android-10.0 device/sony/pdx201_jp
```

## Build
```sh
. build/envsetup.sh
lunch omni_pdx201_jp-eng
mka recoveryimage
```
