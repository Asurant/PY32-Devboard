# PY32 Devboard

## 8/12/2026 - Parts and Schematics

I spent some time brainstorming on what to make. Ended up deciding to make a PY32 devboard. Took me a while to decide what exact PY32 MCU to use but ended up using the PUYA PY32F002BD15S6TU. It's basically a PY32 with 14 pins. I started on the schematics and decided to use a 6 pin USB C connector. Couldn't remember why there was an EH pin so it took me a bit to figure it out, it's just for shielding so it goes to ground. Overall nothing big was done, I do however have ideas on what to do next. I probably will add a way to add a microSD since I never actually did that before. Also solves the problem with storage for it. 
<img width="631" height="404" alt="image" src="https://github.com/user-attachments/assets/47261a99-2bb9-4252-8153-25dd673789ba" />  
## Time Spent: 1 Hour

## 8/13/2026 - Added MicroSD And Schematics Progress

I added the MicroSD today. Took me a while to figure out how it worked and get it set up. I also ended up discovering that MicroSDs used way more pins than I expected (they use 6 at minimum) so I ended up having to switch a 20 pin PY32 (PUYA PY32F002BF15P6TR) since I don't see much use in a large 4 pin devboard. I ended up also discovering at PY32s don't accept USB peripherals on default so I had to go add a CH340 interface controller to allow the USB to actually be used. I also ended up spending a good amount of time understanding the datasheet for the pins and which microSD pins to connect back to the MCU. Along with this I forgot the USB C I was using was a power only USB C. So it pretty much served 0 purpose in this scenerio since it couldn't transfer data so I had to switch it out.
<img width="1226" height="738" alt="image" src="https://github.com/user-attachments/assets/506bb164-7dcf-475f-83b3-12570982a93e" />
## Time Spent: 1.2 Hours
