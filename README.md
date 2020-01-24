V 0.7.3 to run on node 8 using serialport 6.2.2
=========================================================
Install with:

sudo service pimatic stop

cd /home/pi/pimatic-app/node_modules/ 

git clone https://github.com/akicker/pimatic-rfl868.git

cd /home/pi/pimatic-app/node_modules/pimatic-rfl868

npm install

You can load the plugin by editing your `config.json` to include:

```json
{
  "plugin": "rfl868",
  "driverOptions": {
    "serialDevice": "/dev/tty.ACM0"
  }
}
```
cd

sudo /home/pi/pimatic-app/node_modules/pimatic/pimatic.js

pimatic-rfl868
==============

This is a modified copy of pimatic-rflink
Usage: to add a second rflink device - so you can use a 433 MHz module AND a 868 MHz module simultanous
