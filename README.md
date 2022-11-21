If you were redirected to this Github page that means that you received a Raspberry Pi Pico from Gabe that he configured into being used as a Bad USB. 

*switching from third person*

I configured these so that you, the lucky recipient, will be able to learn how to make your own payloads and configure them on your own. (And because I don't have jumper wires)

To access the actual storage of Pico, you'll want to hold down on the button marked `BOOTSEL` as you plug the device in. If you do this, we will be able to see a folder when the device is plugged in and we can reset the firmware. 

1. Download the reset firmware from [flash_nuke.uf2](https://datasheets.raspberrypi.com/soft/flash_nuke.uf2)
2. While holding the BOOTSEL button on the Pico, plug in the USB cable to your computer.
3. When the RPI-RP2 drive shows up on your computer, copy the flash_nuke.uf2 file to the Pico
4. After the device reboots, follow the Install instructions [here](https://github.com/dbisu/pico-ducky/blob/main/README.md)


To make it easier, when you set one of these up the first time you can copy the contents of the `lib` directory along with the `code.py`, `boot.py`, and `payload.dd` files. That way, you won't have to do all that much in terms of dragging and dropping. 

When configuring, in order to stop the mass storage device from being displayed, you will want to go into the `boot.py` file and change Line 10 to say: `if(noStorageStatus == False):`. This will be the LAST step you do, as in order to go back into startup mode you'll need to use jumper wires or reformat the device.

As always, please feel free to contact me if you have any questions or need help working it out.

Happy Hacking! (In an educational context only! I am in no way, shape, or form liable for any unauthorized usages of these devices. If you decide to do something edgy and get caught, it is on YOU.)

**Merry Christmas :)**
