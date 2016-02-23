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

## Full packet capture

* tcpdump -nnvvXSs 1514

## Helpful openssl commands
#### Get the serial number
* openssl x509 -in /etc/ssl/certs/xyz.crt -serial -noout

#### Get the fingerprint
* openssl x509 -in etc/ssl/certs/cert.pem -fingerprint -sha1
* openssl x509 -in etc/ssl/certs/cert.pem -fingerprint -sha256

#### Generate the public key of both the cert and the key
* openssl x509 -pubkey -noout -in etc/ssl/certs/cert.pem
* openssl rsa -in etc/ssl/certs/key.pem -pubout

#### Generate the modulus and then hash it for both the cert and the key
* openssl x509 -noout -modulus -in etc/ssl/certs/cert.pem | openssl sha256
* openssl rsa -noout -modulus -in etc/ssl/certs/key.pem | openssl sha256

## Get SSH fingerprint
* ssh-keygen -lf root/ssh/id_rsa
