# BlackSharkLib.swift

BlackSharkLib.swift is a swift-library that enables communication between your app and Phone Coolers sold under the Black Shark Brand.

# Supported devices

- Black Shark MagCooler 4 Pro

Other devces may work, but are not supported. if you want a device supported, please feel free to create a issue and i may look into adding support.
Priority for adding new supported devices are based of amount of requests and donations.

Confirmed not supported devices:
- Black Shark MagCooler 5 Pro - Uses different protocol apparently. Device is bought and implementation is around the corner.

# Installation
In Xcode under Project and Package Dependencies add a new pagage and enter the following inthe Search-field:
```
https://github.com/Spillmaker/BlackSharkLib.swift
```

# Usage
- Implement your own BluetoothManager
- Use the static functions to idenitfy peripheral as a supported device when you are scanning
- Use the static functions to connect to the proper read and write characteristics.
- Create the bluetooth payloads you want based on the static functions in the library, and send those payloads to the write characteristic
- Use the static parse-function to parse messages from the read characteristic.
- Read comments on the functions themselves for more info.

# Support
I dont have the capacity to provide free support.
If you want me to implement this library into your application, i may be open for work. Feel free to contact me.

# Known usages
The following apps are known to implement this library. check them out. (Want your app here? open a issue/pr)
- [Moblin](https://github.com/eerimoq/moblin) - Adjust the light and adjusts the fanspeed and heat-power automaticly depending on metrics given by the phone, to make the use of the cooler as quiet as possible during live broadcasts.
