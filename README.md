# TWRP Device Tree for Samsung Galaxy Tab S7 FE (SM-T733)

> ⚠️ **Attention:** This is for the WiFi Variant only! LTE/5G Variants use a differrent Chipset!

The Galaxy Tab S7 FE (codenamed _"gts7fewifi"_) is an upper-mid-range tablet from Samsung.

It was announced in May 2021 and released in June 2021.

## Device specifications

| Feature                        | Specification                                                                             |
| -----------------------------: | :---------------------------------------------------------------------------------------- |
| Chipset                        | Qualcomm SM7325 Snapdragon 778G 5G                                                        |
| CPU                            | Octa-core (1x2.4 GHz Kryo 670 Prime, 3x2.2 GHz Kryo 670 Gold & 4x1.9 GHz Kryo 670 Silver) |
| GPU                            | Qualcomm Adreno 642L                                                                      |
| Memory                         | 4GB / 6GB / 8GB RAM (LPDDR4X)                                                             |
| Shipped OS                     | Android 11 (One UI 3.1) - Android 14 (One UI 6.1)                                         |
| Storage                        | 64GB / 128GB / 256GB (UFS 2.1)                                                            |
| MicroSD                        | Up to 1TB                                                                                 |
| Battery                        | 10090mAh Li-Ion (non-removable), 45W fast charge                                          |
| Dimensions                     | 284.8 x 185 x 6.3 mm (11.21 x 7.28 x 0.25 in)                                             |
| Display                        | 12,4", 1600 x 2560 pixels, 16:10 ratio, TFT LCD, 60Hz (~243 ppi density)                  |
| Rear Camera 1 (IMX355)         | 8 MP, f/1.9, 27.6mm (wide), 1/3.5", 1.12µm                                                |
| Front Camera (GC5035)          | 5 MP, f/2.2, 25.4mm (wide), 1/4.44", 1.12µm                                               |
| Sensors                        | Accelerometer, Gyro, Proximity (virtual), Compass, Hall IC, Grip                          |
| Extras                         | Dual speakers                                                                             |

## Device picture

<img src="https://image-us.samsung.com/SamsungUS/home/mobile/tablets/galaxy-tab-s7-fe/GalaxyTabS7plusLite_Combo_001_MysticBlack_1600x1200.png" width="60%"/>

## Kernel source

Extracted from T733XXS8DXJ1 Stock Firmware

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/Bush-cat/android_device_samsung_gts7fewifi-twrp.git -b android-12.1 device/samsung/gts7fewifi
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_gts7fewifi-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2022 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```
