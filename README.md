# basler_ipcam_hack
Geutebrueck TopBC-2188 aka Basler BIP2-1600c hacking and reverse engineering

What is here
Internal serial port location and details.

Boot console dump.

And most importantly Root login!
(password is "ipcam"... srsly, basler?!?)

Back-story:
This camera suffered a pretty heavy power surge (lightning strike), frying its PoE power converter chip, LAN PHY and some protection diodes.

Replacing the fried components brought it back to half-alive, establishing ethernet link but not communicating.
I suspect the surge might have gone through the LAN PHY and damaged some IO pins of the processor which at 338-pin BGA package and US$30 is IMO too much risk to replace (but is possible).
Out of the 3 cameras that were in the same lot, 2 were 100% fixed after replacing the aforementioned components, so I guess that's a win after all!
