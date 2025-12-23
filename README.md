# PowerRiser – Lenovo Tiny 5 PCIe & NVMe Riser Board

![Front view of V2 of the board](https://github.com/nandfarm/PowerRiser/blob/main/Photos/2025-05-22T19_36_39.707Z-Media%20(24).jpg)

PowerRiser is a custom-designed passive riser board that allows you to break out the proprietary Lenovo Tiny 5 series PCIe connector into a standard open-ended x8 PCIe slot, while also providing an additional M.2 NVMe slot (2230/2242 sizes only) for further storage expansion. This board was specifically designed for select Lenovo Tiny 5 series systems (8th/9th gen), such as:

- ThinkCentre M720q

- ThinkCentre M920q

- ThinkCentre M920x

- ThinkStation P330 Tiny

⚠ Please note: The additional M.2 slot supports only PCIe NVMe drives, not SATA drives.

<a href="https://www.tindie.com/stores/nandfarm/?ref=offsite_badges&utm_source=sellers_NandFarm&utm_medium=badges&utm_campaign=badge_small"><img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-smalls.png" alt="I sell on Tindie" width="200" height="55"></a>

## Background
This project is inspired by the [TinyRiser](https://github.com/a-little-wifi/Tinyriser)  board originally designed by [WifiCable](https://x.com/wificable_). After building a batch of [TinyRisers](https://github.com/a-little-wifi/Tinyriser) for personal use and realizing some of my Lenovo Tiny systems had clearance issues (due to the WiFi/BT expansion boards), I decided to create my own variant — which I now call PowerRiser. If you are considering using 2260 or 2280 (with caution) NVMEs, please connect with [WifiCable](https://x.com/wificable_) for details on how to acquire the [TinyRiser](https://github.com/a-little-wifi/Tinyriser).

PowerRiser was developed to:

- Avoid clearance conflicts with other expansion boards.

- Allow installation of short NVMe drives (2230/2242) without obstruction.

- Provide an open-ended x8 PCIe connector that can accept longer x16 PCIe cards (electrically still x8).

Physically, the only modification required is removing the front metal bracket that holds the Bluetooth antenna. (Please refer to the photos in the repo for installation examples, including with an x16 graphics card installed.)

## Usage & Limitations
You can safely install longer PCIe cards (x16), but electrically the slot remains x8.

NVMe drives supported: 2230 and 2242 sizes only.

This riser is only compatible with the Lenovo Tiny 5 series models listed above.

SATA M.2 drives are not supported on the added M.2 slot.

## Project Origin & Intent
This project was built from personal need, trial, and experimentation and so far I have built about 20 boards for my own setups and for others. I hope it helps others facing the same limitations with their Lenovo Tiny builds.

## License
This project is licensed under the CERN Open Hardware License v2 - Strongly Reciprocal (CERN-OHL-S).

You are free to:

 - Manufacture and assemble this board.

- Use it in your own projects.

- Modify and improve it.

However, any modifications and derived works must also be distributed under the same license.

For full license terms, please refer to [CERN-OHL-S](https://ohwr.org/project/cernohl/wikis/home).

## Reports from buyers

As some amy know I have sent a mass email to everyone who bought this board to ask what drive they are using and if they had issues with them. So many replies! Thank you all for the support. Below is the list with everything I received. I will update it as things come in. Keep in mind that this is not an exhaustive list. There are many moderls of drives out there and all should be compatible. If you do find anything let me know!

SSDs reported OK:


- Crucial P310 2230 1TB

- Sabrent Rocket 2230 1TB (SB-2130-1TB)

- Kingston NV3 2230-SNV3SM3/1T0

- WD Black SN770M 2000 GB M.2 2230

- Corsair MP600 Micro 2TB

- Intel DC P3605 1.6TB

- Micron 2400 Series MTFDKBK256TGE 256GB

- ADATA Legend 710 256GB

- Intel Optane M10 MEMPEK1J016GAH 16GB




Issues reported:


- SK Hynix 2230 PVC10 1TB -> reported as not detected at all

- SK Hynix 2230 BC711 512GB -> works but ASPM needs to be turned off in bios, or disable the L1.1 and L1.2 substates in the OS.

- Micron 2400 Series MTFDKCD1T0QFM 1TB -> gets detected at Windows startup but then dissapears. Probably also a ASPM related issue but no further tests were made.


## Disclaimer
⚠ Use at your own risk.
By using, manufacturing, or assembling this board, you accept that:

I am not responsible for any damages, whether physical, financial, or mental, arising from its use.

The design has been made available for educational, experimental, and hobbyist purposes.

Always double-check compatibility, power requirements, and mechanical fit before installation.

## Project Links

Tindie Listing (if you wish to purchase a pre-assembled unit): [PowerRiser on Tindie](https://www.tindie.com/products/nandfarm/powerriser-by-nandfarm/)
