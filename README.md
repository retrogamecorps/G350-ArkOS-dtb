# G350-ArkOS-dtb
Simple dtb repo to allow running vanilla ArkOS on the BATLEXP G350 handheld

## Installation

- Download the latest Anbernic RG351MP image from the <a href="https://github.com/christianhaitian/arkos/wiki">ArkOS wiki</a>
- Flash the image to a reputable microSD card using a tool like Rufus or Raspberry Pi Imager
- Once flashed, remove the SD card and put it back into your computer.  You will see a partition named `BOOT`
- On that `BOOT` partition, replace the file named `rk3326-rg351mp-linux.dtb` with the file in this repo
- Insert the card into your G350, power it on, and enjoy your success

## Disclaimers

- ArkOS does not officially support this handheld, you are on your own to troubleshoot issues!
- Once loaded, you can use a USB WiFi adapter to connect to a network and update ArkOS, RetroArch cores, and more.
- The right analog stick inputs will be off in RetroArch.  You can remap them by going to RA Quick Menu > Controls > Port 1 Controls, adjusting the values to match the actual input of the stick, and then save it as a remap file.
- This dtb file was sourced by mcasoo on the Retro Handhelds discord server (likely from the G350's stock microSD card image, or one of the R36S clones).
