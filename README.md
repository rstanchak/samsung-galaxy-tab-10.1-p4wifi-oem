Samsung Galaxy Tab 10.1 WiFi (p4wifi) Android 4.0.4 Factory Reset

# Requirements
- heimdall-flash

# Install
1. Obtain OEM firmware archive
   - https://www.sammobile.com/samsung/gt-p7510/firmware
   - https://samfw.com/firmware/GT-P7510
2. Extract filesystem images
```
unzip <filename.zip>
tar xvf <extracted.tar.md5>
```
3. Enter download mode
   - Hold power button until tablet reboots.
   - As soon 'Samsung Galaxy Tab' logo displays, release power button and hold left volume rocker button.
   - When the screen shows two Android Robot icons, release the left volume button
   - Press the right volume button to enter download mode
   - Press the right volume button again to confirm
   - When the screen shows "Waiting for USB cable...", connect USB cable from tablet to PC
   - The tablet is now ready to be flashed

4. Flash firmware images
```
heimdall flash \
        --SOS recovery.img \
        --LNX boot.img \
        --APP system.img \
        --CAC cache.img \
        --HID hidden.img
```



