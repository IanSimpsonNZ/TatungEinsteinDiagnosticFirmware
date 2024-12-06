DO NOt USE - I think this is broken as always seems to show a PCI error on the third loop ... working on it ...


This is a crude hack of Fabrizio Di Vittorio's firmware to allow continuous testing of a Tatung Einstein without keyboard or floppy drives attached.

My Einstein had an intermittent fault and I used this firmware to stress test the system until the fault occured.  My system (luckily) seems to have good RAM, so I can't say this version of the fiirmware has been thoroughly tested!

All credit should go to Fabrizio (fdivitto2013@gmail.com - https://github.com/fdivitto)

# Tatung Einstein Diagnostic Firmware
Diagnostic ROM for the Tatung Einstein TC-01


Burn this firmware to a 2764 (rom8k.bin) or 27128 (rom16k.bin) EPROM and place it in the free slot next to the original firmware.

Currently it tests for:
  * 64K dynamic RAMs (8x4164)
  * VDP (TMS9129) and VRAM
  * CTC (timer)
  * PCI (8251 USART)
  * PIO (parallel IO)
     


### Example of all tests passed:
![GitHub Logo](/images/img1.png)


### Example of PSG (Sound Generator and Keyboard controller) not passed:
![GitHub Logo](/images/img2.png)
