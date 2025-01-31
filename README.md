This is EFI configuration for my Hackintosh system with [**OpenCore**](https://dortania.github.io/OpenCore-Install-Guide/) bootloader version 1.0.2, running macOS Sequoia.

## System Specification

- Processor: Intel Core i5 9400H
- GPU: Intel UHD 630 (Integrated)
- Laptop: Dell Latitude 5401
- Ethernet: Intel I219
- Wi-Fi: Intel Dual Band Wireless AC 9560
- Audio Codec: Realtek ALC3204

## What Works

- Virtualization (but runs like shit cuz igpu)
- GPU Acceleration
- Wi-Fi with [**Heliport**](https://github.com/OpenIntelWireless/HeliPort)
- Sleep state
- Audio port
- All USB port

## What Don't Work or Untested

- Thunderbolt 3:
  There is a TB3 ACPI, but i have not tested it yet.

## Using My EFI

If you want to use my EFI, make sure:

1. PlatformInfo in config.plist is present and set to your correct target platform generated from [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS).
2. [**BIOS settings**](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#intel-bios-settings) are set correctly.
3. you dont sue me if your system exploded.

Every system is different. Double check (tripple even) your work if you have similar system as mine and still don't work.

## Credit

- [**OpenCore**](https://dortania.github.io/OpenCore-Install-Guide/)
- [**Andrey1970**](https://github.com/Andrey1970AppleLife)
- [**USBToolBox**](https://github.com/USBToolBox/tool)
- [**OpenIntelWireless**](https://github.com/OpenIntelWireless/itlwm)
- [**SSDT-AWAC khronokernel**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-AWAC.aml)
- [**SSDT-EC-USBX-DESKTOP 1alessandro1**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml)
- [**SSDT-PLUG-DRTNIA khronokernel**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml)
- [**SSDT-PMC khronokernel**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PMC.aml)
- [**SSDT-PNLF 1Revenger1**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PNLF.aml)
- [**SSDT-XOSI 1Revenger1**](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-XOSI.aml)
