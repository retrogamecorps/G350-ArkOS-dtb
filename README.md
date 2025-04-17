# G350-ArkOS-dtb
Simple dtb repo to allow running vanilla ArkOS on the BATLEXP G350 handheld

## Installation

- Download the latest Anbernic RG351MP image from the <a href="https://github.com/christianhaitian/arkos/wiki">ArkOS wiki</a>
- Flash the image to a reputable microSD card using tools like Rufus or Raspberry Pi Imager
- Once flashed, remove the SD card and put it back into your computer.  You will see a partition named "BOOT"
- On that BOOT partition, replace the file named rk3326-rg351mp-linux.dtb with the file in this repo
- Insert the card into your G350, power it on, and enjoy your success

dtb file sourced by mcasoo on the Retro Handhelds discord server (likely from the G350's stock microSD card image, or one of the R36S clones).
