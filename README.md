# G350-ArkOS-dtb
Simple dtb repo to allow running vanilla ArkOS on the BATLEXP G350 handheld.  Part of my <a href="https://retrogamecorps.com/2023/03/27/arkos-starter-guide/">ArkOS Starter Guide</a>.

## Installation

- Download the latest Anbernic RG351MP image from the <a href="https://github.com/christianhaitian/arkos/wiki">ArkOS wiki</a>
- Flash the image to a reputable microSD card using a tool like Rufus or Raspberry Pi Imager
- Once flashed, remove the SD card and put it back into your computer.  You will see a partition named `BOOT`
- On that `BOOT` partition, replace the file named `Image` with the file in this repo
- Add the `rk3326-batlexp-linux.dtb` to the same `BOOT` partition, and delete the file named `rk3326-rg351mp-linux.dtb`
- Using a text editor, open the boot.ini file and rename any references to `rk3326-rg351mp-linux.dtb` with `rk3326-batlexp-linux.dtb`
- Insert the card into your G350, power it on, and enjoy your success

## Disclaimers

- ArkOS does not officially support this handheld, you are on your own to troubleshoot issues!
- Once loaded, you can use a USB WiFi adapter to connect to a network and update ArkOS, RetroArch cores, and more.
- The right analog stick inputs will be off in RetroArch.  You can remap them by going to RA Quick Menu > Controls > Port 1 Controls, adjusting the values to match the actual input of the stick, and then save it as a remap file.
- The dtb and Image files were provided by ChristianHaitian (ArkOS developer), and shared on the <a href="https://retrohandhelds.link/Discord">Retro Handhelds discord server</a>.  It is a nice place to visit if you want to chat or get advice about handhelds/life.
