# TWRP Device Tree for Samsung Galaxy M52 5G

The Galaxy M52 5G (codenamed _"m52xq"_) is an upper-mid-range smartphone from Samsung.

It was announced in September 2021 and released in October 2021.

## Device specifications

| Feature                        | Specification                                                                             |
| -----------------------------: | :---------------------------------------------------------------------------------------- |
| Chipset                        | Qualcomm SM7325 Snapdragon 778G 5G                                                        |
| CPU                            | Octa-core (1x2.4 GHz Kryo 670 Prime, 3x2.2 GHz Kryo 670 Gold & 4x1.9 GHz Kryo 670 Silver) |
| GPU                            | Qualcomm Adreno 642L                                                                      |
| Memory                         | 6GB / 8GB RAM (LPDDR4X)                                                                   |
| Shipped OS                     | Android 11 (One UI 3.1)                                                                   |
| Storage                        | 128GB / 256GB (UFS 2.1)                                                                   |
| SIM                            | Hybrid Dual SIM (Nano-SIM, dual stand-by)                                                 |
| MicroSD                        | Up to 1TB                                                                                 |
| Battery                        | 4860mAh Li-Ion (non-removable), 25W fast charge                                           |
| Dimensions                     | 164.2 x 76.4 x 7.4 mm (6.46 x 3.01 x 0.29 in)                                             |
| Display                        | 6.7", 1080 x 2400 pixels, 20:9 ratio, Super AMOLED Plus, 120Hz (~393 ppi density)         |
| Rear Camera 1 (S5KGW3)         | 64 MP, f/1.8, 26mm (wide), 1/1.97", 0.7um, PDAF                                           |
| Rear Camera 2 (imx258)         | 12 MP, f/2.2, 123˚, (ultrawide), 1/3.06", 1.12µm                                          |
| Rear Camera 3 (S5KGW2)         | 5 MP, f/2.4, (macro)                                                                      |
| Front Camera  (IMX616)         | 32 MP, f/2.2, 26mm (wide), 1/2.8", 0.8µm                                                  |
| Fingerprint                    | EgisTec ET713                                                    |
| Sensors                        | Accelerometer, Gyro, Proximity (virtual), Compass, Hall IC, Grip                          |

## Device picture

![M52XQ](https://files.tecnoblog.net/wp-content/uploads/2021/09/galaxy-m52-5g-produto.png)

## Kernel source 

Available at [https://github.com/BlackMesa123/android_kernel_samsung_sm7325/tree/twrp-12.1](https://github.com/BlackMesa123/android_kernel_samsung_sm7325/tree/twrp-12.1)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-11/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/paulowesll/android_device_samsung_m52xq-twrp.git -b android-12.1 device/samsung/m52xq
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_m52xq-eng
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
