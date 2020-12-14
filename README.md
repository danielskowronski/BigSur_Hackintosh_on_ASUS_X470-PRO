# BigSur_Hackintosh_on_ASUS_X470-PRO

This is my snapshot of **EFI** volume for OpenCore BigSur based Hackintosh on the following setup:

* motherboard: ASUS X470-PRO
* CPU: AMD Ryzen 2700X (`17h`)
* memory: 32GB
* network adapter: Intel I211AT (embedded)
* USB 3.1
* PCIe mounted NVMe disk - but normal SATA disk should work too

Refer to https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html#prerequisites for rest of knowledge.

## Network

This may not work out-of-the-box, but after ystem nstall you can load kext with driver: use `NetworkAdapter/Kext-Droplet-V2.dmg` to load `NetworkAdapter/SmallTree-Intel-211-AT-PCIe-GBE.kext`

## GPU

### nVidia
On BigSur nVidia GPUs other than Kepler based (GTX 6xx, GTX 7xx and some Quadro models) won't work except VESA mode 1280x720, on BigSur nVida other than Kepler based (6xx and 7xx) won't work in proper mode. 

Right now I'm waiting for legacy GTX 780 Ti to arrive so I can confirm.
