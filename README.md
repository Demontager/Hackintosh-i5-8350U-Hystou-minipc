# Hackintosh on i5-8350U-Hystou minipc-UHD620

Working Hackintosh configuration running MacOS Ventura

- Motherboard: Hystou unknown model
- CPU: Intel(R) Core(TM) i5-8350U CPU @ 1.70GHz  
- RAM: 32GB 2x9905630-031.A00G/16GX Kingston 2400Mhz DDR4
- Storage: Samsung 970 EVO M.2 512GB  
- iGPU: Intel UHD 620  
- Realtek ALC892 (0x0892)
- WIFI/BT: BCM94360CS2
- SMIBIOS: MacBookPro15,2
- OpenCore 0.9.0 RELEASE


![Screenshot 2023-03-19 at 17 25 05](https://user-images.githubusercontent.com/7040503/226187965-38c13f0b-cc16-4501-8c70-c0f0ca8054c3.png)


![Снимок экрана 2023-03-19 в 15 12 05](https://user-images.githubusercontent.com/7040503/226187762-b3aebebe-e232-4336-888a-23250aa2ff6e.png)

![Снимок экрана 2023-03-19 в 15 12 37](https://user-images.githubusercontent.com/7040503/226187768-bd6f46d5-e6a8-47f1-a3f8-490c29302371.png)

## Tested and found working:
- Boot into MacOS 
- HDMI output
- Internal Audio Realtek ALC892
- Sleep Wake up from bluetooth mouse or keyboard
- iGPU hardware acceleration
- WIFI and Bluetooth 
- Internal Gigabit Network Card RTL8111/8168/8411
- Airdrop

It is important to set DVMT Pre-Allocated RAM to 32MB otherwise setting to any other value brakes GPU acceleration in webrowsers
![IMG_0118](https://user-images.githubusercontent.com/7040503/226189390-fa0d1cf5-791e-4918-ad46-3930f7c6eed9.jpg)


BCM94360CS2 is native Apple wifi-bt adapter installed in mini-pci slot via adapter, no need additional kexts.
![Screenshot 2023-03-19 at 18 13 03](https://user-images.githubusercontent.com/7040503/226189200-d0c91428-e42b-4012-a218-3467c165b85c.png)


## Tools used:
- [Opencore](https://dortania.github.io/OpenCore-Install-Guide/) 
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
- [Hackintool](https://github.com/headkaze/Hackintool)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

## Guides:
- [Custom SSDT's with SSDTTime](https://www.tonymacx86.com/threads/custom-ssdts-using-corpnewts-ssdttime.318976/)
- [Making own USB port map](https://www.tonymacx86.com/threads/the-new-beginners-guide-to-usb-port-configuration.286553/#post-2029768)
- [How to map your USB Ports on macOS](https://elitemacx86.com/threads/how-to-map-your-usb-ports-on-macos.581/)

## Benchmarks:
![Screenshot 2023-03-19 at 17 29 59](https://user-images.githubusercontent.com/7040503/226189279-98def08e-d65b-4cb8-a0a7-33e58690e759.png)
