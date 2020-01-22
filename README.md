Updated Version to run with node 8 using serialport 6.2.2

Install with:
sudo service pimatic stop
# update npm
npm install -g npm
cd /home/pi/pimatic-app/node_modules/ 
git clone https://github.com/akicker/pimatic-rfl868.git
cd /home/pi/pimatic-app/node_modules/pimatic-rfl868
npm install
npm install -g npm-install-peers
npm-install-peers
npm rebuild
# manually add plugin rfl868 to config.json
cd
sudo /home/pi/pimatic-app/node_modules/pimatic/pimatic.js


pimatic-rfl868
==============

This is a modified copy of pimatic-rflink
Usage: to add a second rflink device - so you can use a 433 MHz module AND a 868 MHz module simultanous

Warning: still under development - no warrenty
