# Skull Canyon
Notes on setting up Ubuntu 16.10 (Yakkety Yak) on Intel NUC6i7KYK

![skull-canyon](img/skull-canyon.jpg)

## Components

* [Intel NUC6i7KYK](http://www.intel.co.uk/content/www/uk/en/nuc/nuc-kit-nuc6i7kyk-features-configurations.html) -
  6th generation Intel® Core™ i7-6770HQ processor with Intel® Iris™ Pro graphics (2.6 to 3.5 GHz Turbo, Quad Core,
  6 MB Cache, 45W TDP).
* [950 PRO NVMe M.2 SSD](http://www.samsung.com/uk/consumer/memory-storage/ssd/950-pro/MZ-V5P256BW) - 256Gb,
  NVMe SSD powered by Samsung V-NAND technology. Up to 2,200MB/s sequential read and 900MB/s write.
* [Komputerbay 32GB ( 2x 16GB) SODIMM](https://www.amazon.co.uk/gp/product/B01H44ARFM) -  Laptop Memory Upgrade
  DDR4 2400MHz PC4-19200 SODIMM 2Rx8 CL16 1.2v Notebook RAM.
* [Microsoft All-in-One Media Keyboard](https://www.microsoft.com/accessories/en-gb/products/keyboards/all-in-one-media-keyboard/n9z-00006).

## Download Ubuntu 16.10

Dowfnload 64-bit desktop ISO image (1.5Gb) from http://releases.ubuntu.com/16.10/ and use
_Startup Disk Creator_ to burn to a USB drive.

## BIOS Settings

BIOS & firmware updates available from: https://downloadcenter.intel.com/product/89187/Intel-NUC-Kit-NUC6i7KYK

### Blink Codes and Beep Codes

The power LED on the Intel® NUC blinks in a pattern if an error occurs during POST.
Intel NUC products that include a front panel audio jack produce an audible beep pattern
that you can hear through headphones or speakers plugged into that jack.

| Code | Diagnosis | Pattern |
|------|-----------|---------|
| 3 blinks (3 beeps) | Memory error | On-off (1.0 second each) three times, then 2.5-second pause (off). The pattern repeats until the computer is powered off. |
| Continual blinks | BIOS Update in progress | Off when the update starts, then on for 0.5 seconds, then off for 0.5 seconds. The pattern repeats until the BIOS update is complete. |
| 2 blinks (2 beeps) | Video error (when no VGA option ROM is found) | On-off (1.0 second each) two times, then 2.5-second pause (off). The pattern repeats until the computer is powered off. |
| 16 on/off blinks (8 beeps) | CPU thermal trip warning | 0.25 seconds on, 0.25 seconds off, 0.25 seconds on, 0.25 seconds off, for a total of 16 blinks. Then the computer shuts down. |

## Keyboard Mappings

`showkey` displays the key mappings and `keytouch-editor` allows custom key mappings to be created.

### References
* http://unix.stackexchange.com/questions/198715/media-key-problems-with-microsoft-keyboard
* http://unix.stackexchange.com/questions/227264/is-it-possible-to-tweak-input-from-touchpad
