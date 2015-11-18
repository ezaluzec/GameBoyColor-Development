# GameBoyColor-Development

I wrote code for the GameBoyAdvanced years ago. See [Circuit Cellar Magazine, February 2006](http://www.cc-webshop.com/Circuit-Cellar-Issue-187-February-2006-PDF-FI-2006-187.htm). 

Of course I had a nice XPort cartridge to link my computer to the GBA. There was no hardware work
involved -- just C++ and learning the hardware registers on the GBA.

GBC development is nothing new. There are lots of tutorials on GBC hacking (see the links below).
This repo is a journal of my experience and any code I produced along the way. 

I started with a Game Boy Color and several cartridges I bought from ebay. 

![](https://github.com/topherCantrell/GameBoyColor-Development/blob/master/art/IMG_0310.JPG)

The Gameboy Color is backwards compatible with the Gameboy (non color). That means I can start with
simpler programs that don't access the color registers. The cartridge pinouts are the same.

## Links

This is my primary source. Here is how to remove the existing rom and replace with an FRAM. There
is even a circuit here to program it.
[Gameboy Fram Cart](http://www.robotdungeon.com/ElectronicProjectGameboyROM.html)

[Wikipedia](https://en.wikipedia.org/wiki/Game_Boy_Color)

[http://www.loirak.com/gameboy/gbprog.php](http://www.loirak.com/gameboy/gbprog.php)

[http://belial.blarzwurst.de/gbpaper/paper.pdf](http://belial.blarzwurst.de/gbpaper/paper.pdf)

[http://gbdev.gg8.se/wiki/articles/Main_Page](http://gbdev.gg8.se/wiki/articles/Main_Page)

[Tech info](http://fms.komkon.org/GameBoy/Tech/Software.html)

[Javascript Emulator](http://imrannazar.com/GameBoy-Emulation-in-JavaScript:-Interrupts)

## Development Cartridges

Two of the cartridges (Tarzan and Winnie the Pooh) had clear cases. I chose to hack those.
The screws holding the cartridges together have the Nintendo star-pattern heads. I was able
to carefully unscrew them with needle-nose pliars.

![](https://github.com/topherCantrell/GameBoyColor-Development/blob/master/art/IMG_0322.JPG)

The Tarzan cartridge is very simple: just the ROM and the memory mapper chip. The Pooh cartridge
has a battery-backed RAM in it.

The cartridge is one-sided. It slides into the back of the unit so that the connector pads
and parts are facing out (not in towards the unit).

[Image from here](https://www.insidegadgets.com/2011/03/19/gbcartread-arduino-based-gameboy-cart-reader-%E2%80%93-part-1-read-the-rom/)

![](https://github.com/topherCantrell/GameBoyColor-Development/blob/master/art/cartPinout.png)

I decided to start with the simple ROM+MBC. The board is shorter ... more room at the top for an expansion 
board. The pins on the simpler-ROM are farther apart, and it is easier to work with the board. I used
tiny side-cutters to cut the ROM from its surface mount pads. Each pin on the ROM has a corresponding
through-hole pad for me to tag wires into.

![](https://github.com/topherCantrell/GameBoyColor-Development/blob/master/art/cart2.png)

