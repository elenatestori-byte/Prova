# Using the registry

For even more solid evidence, you can cross-reference [the data from USBDeview](https://www.nirsoft.net/utils/usbdeview.zip) with the data from the Windows Registry. The operating system keeps a detailed track of the connected peripherals, and this data is not easily erased. The most important registry keys for USB parsing are:

* **USBSTOR:** This key stores information about all USB storage devices connected to your computer. You can find the device type, manufacturer, and serial number, providing you with irrefutable proof that a specific dongle has been connected to the system. The complete path is .`HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Enum\USBSTOR`
* **MountedDevices**: This key records the drive letters assigned to each volume (such as C:, D: etc.) and also includes those assigned to USB peripherals. This allows you to see by which drive letter a specific stick has been recognized by the system. The complete path is .`HKEY_LOCAL_MACHINE\SYSTEM\MountedDevices`
