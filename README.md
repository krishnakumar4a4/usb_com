## USB COM
Uses libusb to capture usb traffic from userspace, can also be used to write.

```cargo run```
Shows the list of all devices, configurations, interfaces and endpoints etc

```cargo run --example read_wacom_device 1386 890```
Read interrupt endpoint from wacom pen tablet, should be run with sudo otherwise throws permission denied.
Doesn't work on mac even with sudo.

Next steps:
- Integrate with libudev to identify device plugged in
- Able to write to USB device
- Tinker with other modes of USB like bulk, isochronous.


