# NOTE
## This repository is a work in progress, you may experience bugs, glitches and general oddities. Should these occur please report them as issues. It is not actively being worked on and will require community assistance to finish.

# Information
A French translation of https://github.com/gb-mobile/pokecrystal-mobile-eng
This translation was performed via text dumps and a (somewhat) sophisticated find/replace script.
It is possible that some menus were missed by the find/replace script, and need translating manually.


## TO-DO

Due to this translation being performed using a find/replace script, several lines which are duplicated in English but have differences between them in other languages get skipped over.
To complete the translation of non-mobile features into French, the following lines need to be identified and placed accordingly:
https://github.com/gb-mobile/pokecrystal-mobile-fra/wiki/Potentially-misplaced-or-Missing-lines


- Adjust any menus to match those of the original French games (currently set to English sizing and formatting)
- Check for any untranslated menus missed by the find/replace script.
- Translate any of mobile features. (Anything English under /mobile/, /maps/GoldenrodPokecenter1F.asm, maps/PokecomCenterAdminOfficeMobile.asm, data/text/common_1.asmm data/text/common_3.asm and data/text/battle.asm).
- Also refer to the English build for 'Text_BattleReceptionistIntro:', 'Text_TradeReceptionistIntro:' and 'Text_TimeCapsuleReceptionistIntro:' for proper mobile translations of the PokeCOM Club reception dialogue.
- Determine the value of 'REGION CODE' in engine/link/mystery_gift.asm
- Fix the known issues.


## Setup [![Build Status][ci-badge]][ci]

For more information, please see [INSTALL.md](INSTALL.md)

After setup has been completed, you can choose which version you wish to build.
To build a specific version, run this command inside the repository directory in cygwin64:

`make`


Other languages are being worked on, but are not complete and still require a lot of polish.

## Using Mobile Adapter Features

To take advantage of the Mobile Adapter features, we currently recommend the GameBoy Emulator BGB:
https://bgb.bircd.org/

and libmobile-bgb:
https://github.com/REONTeam/libmobile-bgb/releases

Simply open BGB, right click the ‘screen’ and select `Link > Listen`, then accept the port it provides by clicking `OK`.
Once done, run the latest version of libmobile for your operating system (`mobile-windows.exe` or windows and `mobile-linux` for linux).
Now right click the ‘screen’ on BGB again and select `Load ROM…`, then choose the pokecrystal-mobile `.gbc` file you have built.

## Mobile Adapter Features

A full list of Mobile Adapter features for Pokémon Crystal can be found here:
https://github.com/gb-mobile/pokecrystal-mobile-en/wiki/Pok%C3%A9mon-Crystal-Mobile-Features

## Contributors

- Pret           : Initial disassembly
- Matze          : Mobile Restoration & Japanese Code Disassembly
- Damien         : Code
- DS             : GFX & Code
- Ryuzac         : Code & Japanese Translation
- Zumilsawhat?   : Code (Large amounts of work on the EZ Chat system)
- REON Community : Support and Assistance

[ci]: https://github.com/pret/pokecrystal/actions
[ci-badge]: https://github.com/pret/pokecrystal/actions/workflows/main.yml/badge.svg
