Linux
1. Install PlatformIO
```
sudo apt-get install python-pip
sudo pip install -U platformio
platformio --version
```
If you have any issue while installing it, refer this guide.
http://docs.platformio.org/en/stable/installation.html

2. Get source code
```
sudo apt-get install git
git clone https://github.com/juniocezar/smartpower2.git
```


3. Build & Upload
Connect microUSB to Host PC.
You can see the list of USB drivers “CP210x UART Bridge” by lsusb in the terminal.

```
cd smartpower2
sudo platformio run
sudo platformio run --target upload
sudo platformio run --target uploadfs
```


Timer:


 timerId = timer.setInterval(1000, handler);



Reference:

https://wiki.odroid.com/accessory/power_supply_battery/smartpower2#receving_power_data_via_microusb_cable

https://forum.odroid.com/viewtopic.php?f=86&t=25428

http://www.ti.com/lit/ds/symlink/ina231.pdf

https://forum.odroid.com/viewtopic.php?f=86&t=31395&sid=f5b1581d302d2d70643e362fb55622bb

https://forum.odroid.com/viewtopic.php?f=86&t=28883&sid=f5b1581d302d2d70643e362fb55622bb (similar usage)
