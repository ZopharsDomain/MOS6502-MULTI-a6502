EMU programmer,
Included is the source code to my 6502 emulator as well as the game driver for
Asteroids which shows how it is actually used.  This 6502 emulates the basic
instruction set and not the 65C02 nor the 65816.  If you feel like adding the
'undocumented' instructions, please send me your results.  You may use this
in your own projects (not for profit) as long as you mention that it came from
me.  Please feel free to pick at it and offer suggestions for improvements.
Some of the code may look like it's doing things backwards; this is for
Pentium and 486 optimization.  The general rule is that sequential instructions
should not reference the same register.  Another useful rules is that when
running in a 32-bit code segment, use of 16-bit registers is a no-no because it
causes a data size override byte and pipe stall to occur.

Enjoy,
Larry Bank 5/4/98
