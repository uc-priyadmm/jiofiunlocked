# FAQs ❓

1. Q. My device is not visible in fastboot devices A. Confirm driver installation a faulty cable can also be the issue..
2. Q. Everything went well but still no changes in dashboard A. After successful flash if you still don't see the changes your device is probably booting from recovery partition. Try flashing recovery partition by`fastboot erase recoveryfs fastboot flash recoveryfs "D:\system.img"` .
3. Q. After resetting device from pin hole button it shows INVALID SIM. A. This is supposed to happen just reboot the device it'll work again..
4. Q. Can I undo all this and get back to original firmware A. Yes just flash the original firmware provided in post and reset the device.
