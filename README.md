### OrionOS OTA repo
In order for a device to be officially supported by OrionOS, OTA information needs to be added.
Please refer to the following "Readme" to get started

### Introduction
In order for a device to be OTA compliant, there are a few things to know.

### JSON structure
```
{
  "response": [
    {
      "maintainer": "Name (nickname)",
      "oem": "OEM",
      "device": "Device Name",
      "filename": "OrionOS-15.1-<modversion>-<device codename>-<buildtype>-<variant>-<date>.zip",
      "download": "https://sourceforge.net/projects/orionos/files/A15/<device codename>/OrionOS-15.1-<modversion>-<device codename>-<buildtype>-<variant>-<date>.zip/download",
      "timestamp": 0000000000,
      "md5": "abcdefg123456",
      "sha256": "abcdefg123456",
      "size": 123456789,
      "version": "15.1",
      "buildtype": "Official",
      "forum": "https://forum link", #(mandatory)
      "firmware": "https://firmware link",
      "paypal": "https://donation link",
      "telegram": "https://telegram link",
      "github": "GitHub Username",
      "initial_installation_images": [
        "img files to be flashed before sideloading OrionOS's zip"
      ]
    }
  ]
}
```
