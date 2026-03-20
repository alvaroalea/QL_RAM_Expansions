# SINCLAIR QL 896kB External Rom Expansion

(C) 2026 Alvaro Alea Fernandez

License under: CERN Open Hardware Licence Version 2 - Strongly Reciprocal

https://ohwr.org/cern_ohl_s_v2.txt

This is based on the work of McLeod Ideafix, Jose Leandro, Zerover and tcat between others. 

This board will provide up to 768kB aditional of static RAM (fast-ram) to the sinclair QL.

This board can be stacked with my old external ram board, jumpers allow a 512Kb, or +256Kb configs of the old board.

There is also a expecial 832Kb config that free the 64Kb top memory for aditional boards without use the ROM Cartridge area (Jose Leandro's QuBide...)

Provide a expansion conector to allow conect aditional interfaces.

There area available 4 configuration trough a dip switch in the PCB.
* 640kB - This is the standar 512kB expansion for any QL
* 832kB - Similar to 256kB provide aditional space for expansion cards correctly configured.
* 896kB - Maximin RAM do not provide aditional space for expansion cards.
* Expecial - This is for use as a second expansion, use the full QL space for a maximun of 898kB, be aware that this is incompatible with a lot of expansion card, so use with caution (Any expansion card that do not use jumper for configuration will be incompatible).


In the GAL folder there is the source code to be compiled with GALasm that you can found here: https://github.com/daveho/GALasm

## Mini Trump Card Compatibility

I have done a version of the trump card disk interface here: https://github.com/alvaroalea/QL_MiniTrump3 , this interface do not
provide memory like the original one. You can combine both cards to mimic the original trump card.

You shall connect this board after the minitrump, you need to change the solder jumper (JP1) to 1-2 to allow the Minitrump card to coordinate with the second memory card.

This jumper can be alwais 1-2, 2-3 is only used if you have another card that need BERR signal (none as far as I know).


![My image](QL_external_ram_892Kb.png) 


