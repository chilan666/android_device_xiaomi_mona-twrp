## TWRP Device tree for POCO X5 Pro 5G (codename: redwood)
![POCO X5 Pro 5G/Redmi Note 12 Pro Speed Edition](https://fdn2.gsmarena.com/vv/pics/xiaomi/xiaomi-poco-x5-pro-5g-1.jpg "POCO X5 Pro 5G/Redmi Note 12 Pro Speed Edition")


| Feature                 | Specification                                                              |
| :---------------------- | :--------------------------------                                          |
| CPU                     | Octa-core (1x2.4 GHz Cortex-A78 & 3x2.2 GHz Cortex-A78 & 4x1.9 GHz Cortex-A55) |
| Chipset                 | Qualcomm SM7325 Snapdragon 778G 5G (6 nm)                                  |
| GPU                     | Adreno 642L                                                                |
| Memory                  | 6 GB / 8 GB                                                                |
| Shipped Software        | Android 12, MIUI 14                                                        |
| Storage                 | 128 GB / 256 GB                                                            |

## Image-related Notes
- For some reason, this device (A/B) can't boot a custom recovery image temporarily; `fastboot boot twrp-name.img` doesn't work.
- If you flash TWRP like you are directly flashing boot.img, there's a chance of breaking the booting process and will throw in a bootloop.
- Decryption is working, and flashing some archives works too. MTP and Vibration didn't.
