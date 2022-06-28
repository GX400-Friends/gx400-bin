# GX400 FPGA Core Change Log

## 2022-06-28 – Beta 2

* Fixed partially off-screen sprites bleeding to the other edge of the screen;
* Fixed sprites flickering when entering the screen;
* Implemented sprite double-buffering, like on the original hardware;
* Fixed black dots and vertical lines on objects mades of adjacent, large, and/or zoomed sprites;
* Fixed video flipping for cocktail mode;
* Fixed audio clock frequency, that was accidentally left a bit too low after tests;
* Adjusted the PLL to achieve an accurate 6.144 MHz pixel clock;
* CPU, audio, and pixel clocks, as well as refresh rate, are therefore now all accurate with respect to the original hardware;
* Game ROMs are now loaded to SDRAM;
* Updated to the latest jtframe framework, which in turn updates to the latest MiSTer framework;
* Fixed sprite drawing order, which was noticeable when there were a lot of sprites on screen;
* Fixed sprites missing after reset;
* Implemented pause function;
* Updated MRAs for `update_all.sh` distribution.

### Known issues:

None.

## 2022-03-14 – Beta 1

* First public version;
* Nemesis and Nemesis (UK) are fully playable.

### Known issues:

* Screen Flip/Cocktail Mode is not properly implemented yet;
* Resetting the game several times will make the sprites disappear;
* Sprite glitches with many objects on screen;
* Audio volumes need to be adjusted;
* PLL frequencies need to be slightly adjusted.
