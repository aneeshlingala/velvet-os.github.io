# After first boot

The images are assuming a US keyboard and are setup for English, so one should configure it as needed after the first boot using the ```/scripts/initial-setup.sh``` script - This will setup the keyboard, timezone and locale. Sometimes, the keyboard setup is skipped, then it can be adjusted in the file /etc/default/keyboard.

Some commands to set the initial keyboard mapping in an x terminal to run anything with the proper keyboard layout before everything is setup properly:

```
english: setxkbmap us
french: setxkbmap fr
german: setxkbmap de
italian: setxkbmap it
portuguese: setxkbmap pt
polish: setxkbmap pl
russian: setxkbmap ru
spanish: setxkbmap es
...
```

You might be interested in running ```/scripts/extend-rootfs.sh``` which will extend the rootfs to the end of the disk.

Additional setup instructions can be found [here](./postinst/readme.md)
