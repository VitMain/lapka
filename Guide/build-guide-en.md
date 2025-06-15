# Guide

To assemble the keyboard you will need the following parts:

### 1. The boards themselves, 2 pieces.

They can be ordered from any board manufacturer using Gerber files from the repository. I used the services of [SJ PCB](https://aliexpress.ru/store/129841), but you can use JLCPCB, PCBWay or anything else.

### 2. Controllers.

The board is compatible with nRF52840 or nice!nano. You will need 2 or 3 of them, depending on whether you want to use a Dongle, which will extend the life of a single charge several times. You can buy nRF52840 on [AliExpress](https://aliexpress.ru/item/1005008099333183.html).

> Warning! Sometimes controllers can come defective, so it's worth ordering more of them. They're inexpensive and certainly enough to save your nerves.

### 3. Batteries.

You will need 2 batteries of the `041230` format. I bought them on OZON, but you can also look for them on AliExpress or Amazon.

### 4. Switches.

You will need 36 switches of Choc v1 or Choc v2 format. MX or GLP switches are not suitable! Choose to your taste and color. I used [Kailh Deep Sea Islet](https://aliexpress.ru/item/1005004684367347.html?spm=a2g2w.orderdetail.0.0.1cb14aa6TeBgaj&sku_id=12000040713238946)

### 5. Keycaps.

If Choc v1 switches are used, then almost any keycaps for Choc switches will work.

If Choc v2 switches are used, then only custom keycaps that have Choc-spacing (18×17 vs 19×19 for MX) and at the same time an MX stem (compatible with Choc v2 switches) will work. For example, you can use [KLP Lame](https://github.com/braindefender/KLP-Lame-Keycaps).

### 6. Body parts
Which consist of:
1. `Frame` — the main part for the typing cluster.
2. `Thumb` — part for the thumb cluster.
3. `Cover` — part that covers the controller.
4. (Optional) `Spacer` — a small bracket that is installed between the Frame and Cover. It is needed if the Cover part was printed with a small shrinkage and it dangles on the board.

> The repository contains both STL files and 3MF files with examples of my print settings.

### 7. (Optional) 2 buttons of the [SMD 4x4x1.5mm](https://aliexpress.ru/item/32802382507.html) format.

They are soldered to the bottom of the boards and serve for quick access to the Reset function.

<hr>

Having all the necessary parts, as well as a soldering iron, solder/paste and other little things for soldering, you can start the assembling process:

### 1. First, you need to make sure that the controllers work.

> This must be done **BEFORE** starting everything else!

To do this, you need to flash them with Debug firmware and make sure that all the pins press the corresponding keys. Check the functionality of the matrix using [key-test.ru](https://key-test.ru), clamping the contacts of the switches with tweezers.

### 2. Prepare the pin headers

![](./nRF52840-with-pin-headers.jpg)

There are three pin headers that come with controller: two long and one short. We'll need only two long ones.

Using the [pin layout](./pin_layout_v2.png), you need to remove the metal pins marked in red from the header. Red pins **DO NOT** need to be soldered.

![](./pin_layout_v2.png)

In order to accurately determine the height of the header's pins, you can remove the black plastic spacers from the short pin header and put them on the corners of the long pin headers. Having determined the desired height, you can cut off the excess with nippers.

![](./nRF52840-with-modified-pin-header.jpg)

### 3. Solder the headers.

Apply solder paste to the header pins on the board side, align the controller so that the headers are perpendicular to the board, and solder the headers to the board one by one.

![](./nRF52840-pin-header-position.jpg)

You'll get something like that:

![](./photo_2025-06-16_02-17-15.jpg)

> Attention! Both controllers should be facing up. The boards are symmetrical, so the headers should NOT be flipped or mirrored! They should be soldered in the same orientation as on the other half of the keyboard.

### 4. Install the body part

Put Frame and Thumb case parts and insert switches into them.

> Attention! The case parts should be located **between** the board and the switches.

### 5. Final soldering

Apply soldering paste to the contacts of the switches and solder them. Stick the battery between controller and PCB, then solder the battery wires to the pins `B+` and `B-` respectively. At this point, the controller will blink red or blue diodes. At about the same time, you can solder the Reset buttons, if you have them.

### 6. (Optional) Attach a Spacer piece between the Frame and Cover.

### 7. Flash the firmware

Connect the keyboard to the PC, go to the firmware mode in one of the ways:
- press Reset button twice
- short the button pins that is located on the back of the PCB twice
- short the `GND` and `RST` pins twice with tweezers

After this, the controller should connect to the PC as a USB drive.
Copy the firmware file to it and repeat for the other half.

### 8. Finale

Put the controller cover on. Stick the silicone bumpers via perimeter and... Done!
Do the same with the other half.
