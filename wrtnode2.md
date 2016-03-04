WRTnode2 Getting Started Wiki
=============================
03-03-2016

Initial Connect
---------------

1. Connect WRTnode2 to dev-board and power Micro-B USB port with 5V
2. Connect to WiFI "WRTnode2R_XXX", password=12345678
3. Open browser, type 192.168.8.1
4. Log on as root with above password
5. Go to password configuration and choose root password
6. ssh into WRTnode2
    ```bash
    ssh root@192.168.8.1
    ````

Connect to local WiFi and change broadcast SSID
-----------------------------------------------

1. 
```bash
vi /etc/config/wireless 
```
Change SSIDs and passwords
2. Reset network
```bash
\etc\init.d\network reload
```

Install python-light
--------------------

1. SSH into WRTnode2
2.
```bash
opkg update
opkg install python-light
```
