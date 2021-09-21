# GUIDE 📕

1. Locate your device model and download the respective Firmware and extract it to a known location

1. Install drivers and tools
- Install Fastboot [drivers](https://gsmusbdrivers.com/download/adb-fastboot-drivers/)
- Install [Fastboot](https://androiddatahost.com/uq6us)

3. Prepare device

- Remove battery from JioFi
- Locate reset pin hole button
- Lay down JioFi
- Use Paper Clip / SIM Ejector Tool to reset
- While still holding down on the reset button  insert the USB cable
- Release button as soon as all the LEDs in Display turns RED. This means device is in boot loader mode 🌟

4. Flashing Unlocked Firmware

- Open adb and fastboot tools terminal
- Enter following to check if device is connected
- `fastboot devices`
- It will return something like this
- `baxxxxx fastboot`
- This means device is connected. If your device doesn't show up here please check drivers in Device manager
- Now first erase the system partition
- `fastboot erase system`
- It will return something like this
- `erasing 'system'...
OKAY [ 1.104s]
finished. total time: 1.105s`
- Now flash the firmware
- `fastboot flash system "D:\system.img"` ( replace path )
- It should return something like this
- `sending 'system' (34306 KB)...
OKAY [ 1.276s]
writing 'system'...
OKAY [ 9.462s]
finished. total time: 10.741s`
- Now send reboot command to device
- `fastboot reboot`
- You'll notice device will reboot normally now you can unplug the cable.

## ✌️ Congratulations your device is now unlocked and you can reinsert the battery and another SIM for testing.

### ❌  Firmware will take longer than usual to boot do not panic  ❌
