# BigSur_Hackintosh_on_ASUS_X470-PRO

## This project is obsolete!

While it still works on described hardware platform with Big Sur, it was never tested on Monterey, let alone Ventura. I no longer use this software configuration and can't help with any issues, but I'm keeping this source code as a public archive. 

---

## Disclaimer
Most of the repo consists of files not created by me - this is only compilation. See COPYRIGHTS.md

## Setup description

This is my snapshot of **EFI** volume for OpenCore BigSur based Hackintosh on the following setup:

* motherboard: ASUS X470-PRO
* CPU: AMD Ryzen 2700X (`17h`)
* memory: 32GB
* network adapter: Intel I211AT (embedded)
* GPU: Nvidia GTX 780 Ti (Kepler)
* USB 3.1
* PCIe mounted NVMe disk - but normal SATA disk should work too

Refer to https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html#prerequisites for rest of knowledge.

### WiFi and BT
This is mostly for Apple Watch Unlock support - Fenvi FV-HB1200B works nicely.

## GPU

### nVidia
On BigSur nVidia GPUs other than Kepler based (GTX 6xx, GTX 7xx and some Quadro models) won't work except VESA mode 1280x720, on BigSur nVida other than Kepler based (6xx and 7xx) won't work in proper mode - so called _Web Driver_ is not working on Catalina and BigSur.

