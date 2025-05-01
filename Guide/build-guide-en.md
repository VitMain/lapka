# Guide

1. Order a PCB production using Gerber files.

> I used [SJ PCB](https://aliexpress.ru/store/129841).
> You can use JLCPCB, PCBWay or similar.

2. Buy needed parts, specifically:
	- 36 Choc v2 switches (I used [Kailh Deep Sea Islet](https://aliexpress.ru/item/1005004684367347.html?spm=a2g2w.orderdetail.0.0.1cb14aa6TeBgaj&sku_id=12000040713238946))
	- 2 [SuperMini nRF52840](https://aliexpress.ru/item/1005008099333183.html) controllers
	- 2 batteries of `041230` format.
	- (optional) 2 [SMD 4x4x1.5mm](https://aliexpress.ru/item/32802382507.html) buttons
	- and soldering iron/fan, solder/paste and other things for soldering

3. Order or print parts of the case. There are STL/3MF files in the repo (with example of print settings).

4. Order or print keycaps. This keyboard use non-standard keycaps that have Choc-spacing (18×17 instead of 19×19 on MX) and MX stem simultaneously (to be compatible with Choc v2 switches). You can use [KLP Lame](https://github.com/braindefender/KLP-Lame-Keycaps) or any other keycaps that has those properties.

5. There are two long PLS pin headers that come with SuperMini. You should remove pins that colored RED (according to [pin layout](./pin_layout_v2.png) image). They are not meant to be soldered!

6. To determine the right height for pin headers, detach black plastic pieces from short pin headers and attach them onto the long ones.

7. Solder pin headers to PCB and controllers. At this step, you can flash the debug firmware to check that it prints the right symbols and everything is working properly. You can use [key-test.ru](https://key-test.ru), shortening switch pins with tweezers.

8. After you check that everything is OK, you should place case parts (Frame and Thumb), insert and solder switches. Also, you can solder Reset buttons, if you have them.

9. Solder the battery to `B+` (red) and `B-` (black) pins.

10. Clip spacer part onto PCB between Frame and controller case. After that, place controller case and you are good to go! Now, repeat that with the other part of the split.

> Warning! PCB's are symmetrical. Therefore, pin headers must NOT be flipped! They must be soldered with the same orientation that it is on the other part of the split.
