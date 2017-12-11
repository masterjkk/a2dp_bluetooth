# a2dp_bluetooth

## a2dp_source

To connect a set of Bluetooth Headphones or Bluetooth Speakers to Raspbian Jessie, use the `configure` file, and run it.

```
git clone https://github.com/bareinhard/a2dp_bluetooth
cd a2dp_bluetooth
./configure
```

**Pairing, Trusting, and Connecting**
```
sudo bluetoothctl
[bluetooth]# power on
[bluetooth]# agent on
[bluetooth]# default-agent
[bluetooth]# scan on
[bluetooth]# pair XX:XX:XX:XX:XX
[bluetooth]# trust XX:XX:XX:XX:XX
[bluetooth]# connect XX:XX:XX:XX:XX
[bluetooth]# exit
```

**After the install, you will need to reboot and manually pair, trust, and connect your device only once. Going forward you will only need to turn on the bluetooth device and it will automatically connect**
