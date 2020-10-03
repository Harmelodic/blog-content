I just bought a pair of OnePlus Bullets Wireless, which is an AptX Bluetooth Audio device.

It paired beautifully with my OnePlus 6, but when it came to pairing it with my Macbook Pro, it didn't show up in the Bluetooth menu!

That's because the AptX codec was not enabled in my defaults. To enable it, open a terminal and perform:

```bash
sudo defaults write bluetoothaudiod "Enable AptX codec" -bool true
```

And boom! OnePlus Bullets Wireless now appear in my MacOS Bluetooth menu!
