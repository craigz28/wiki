Commands, etc.

## Create an OS X USB stick installer
- sudo /Applications/Install\ OS\ X\ Yosemite.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume --applicationpath /Applications/Install\ OS\ X\ Yosemite.app

## Speed Test Command Line

- wget -O speedtest-cli https://raw.github.com/sivel/speedtest-cli/master/speedtest_cli.py

chmod +x speedtest-cli

./speedtest-cli

Also - wget http://cachefly.cachefly.net/400mb.test -O /dev/null

## Secure Erase in El Capitan
Since secure erase features have been removed from the GUI, command line is as follows:

diskutil secureErase 0 /dev/disk5

There are multiple levels to secureErase, level 0 is the basic level for writing all zeros to the disk
