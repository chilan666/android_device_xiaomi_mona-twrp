## TWRP Device tree for POCO X5 Pro 5G (codename: redwood)

## Device specifications
| Feature                 | Specification                                                              |
| :---------------------- | :--------------------------------                                          |
| CPU                     | Octa-core (1x2.4 GHz Cortex-A78 & 3x2.2 GHz Cortex-A78 & 4x1.9 GHz Cortex-A55) |
| Chipset                 | Qualcomm SM7325 Snapdragon 778G 5G (6 nm)                                  |
| GPU                     | Adreno 642L                                                                |
| Memory                  | 6 GB / 8 GB                                                                |
| Shipped Software        | Android 12, MIUI 14                                                        |
| Storage                 | 128 GB / 256 GB                                                            |

## Device picture

![POCO X5 Pro 5G/Redmi Note 12 Pro Speed Edition](https://fdn2.gsmarena.com/vv/pics/xiaomi/xiaomi-poco-x5-pro-5g-1.jpg "POCO X5 Pro 5G/Redmi Note 12 Pro Speed Edition")

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/brigudav/android_device_xiaomi_redwood_twrp.git -b android-12.1 device/xiaomi/redwood
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_redwood-eng
make adbd bootimage
```
## Image-related Notes
- For some reason, this device (A/B) can't boot a custom recovery image temporarily; `fastboot boot twrp-name.img` doesn't work.
- If you flash TWRP like you are directly flashing boot.img, there's a chance of breaking the booting process and will throw in a bootloop.

## Copyright

```
#
# Copyright (C) 2023 The TWRP Open Source Project
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
