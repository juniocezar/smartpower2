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
