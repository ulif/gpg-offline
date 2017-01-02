# gpg-offline
Handle gpg keys offline.

The setup described here is currently based on Debian 8 (Jessie).


## Create a bootable USB stick (4 GB or more)

Download a Debian live image and copy it to your stick:

    $ wget http://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-8.6.0-amd64-standard.iso
    $ sudo cp debian-live-8.6.0-amd64-standard.iso /dev/sdX
    $ sudo sync

We use the (commandline-oriented) standard image of Debian.

In case of trouble see
https://www.debian.org/releases/stable/amd64/ch04s03.html.en.

