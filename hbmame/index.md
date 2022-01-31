## HBMAME Sets & Datfiles

<b><span style="color: red;">Kindly share with others what others so kindly shared with you!</span></b><br>
All zipfiles in the sets are TorrentZipped.<br>
If you already have a previous set, simply join the new set by pointing at the content of your previous set.<br>
In order to reproduce the full sets with any Rom Manager, it's highly recommended to use the published datfiles.<br>
HBMAME CHDs and rollback CHDs can be rebuilt or cherry-picked from the current MAME CHDs set.<br>

<b>HBMAME Update sets:</b>

HBMAME - Update ROMs<br>
Set: [HBMAME - Update ROMs (v0.239 to v0.240)](http://mgnet.me/eqwB3ob)<br>
Datfile: [HBMAME - Update ROMs (v0.239 to v0.240)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME - Update ROMs (v0.239 to v0.240).zip)<br>

<b>HBMAME Machines, BIOS and Devices sets:</b>

HBMAME ROMs (bios-devices)<br>
Set: [HBMAME 0.240 ROMs (bios-devices)](http://mgnet.me/eqwB3o6)<br>
Datfile: [HBMAME 0.240 ROMs (bios-devices)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 ROMs (bios-devices).zip)<br>

First, the BIOS set: Some arcade machines shared a common hardware platform, such as the Neo-Geo arcade hardware. As the main board had data necessary to start up and self-test the hardware before passing it off to the game cartridge, it’s not really appropriate to store that data as part of the game ROM sets.<br>
Instead, it is stored as a BIOS image for the system itself (e.g. NEOGEO.ZIP for Neo-Geo games)<br>
<br>
Secondly, the device set. Frequently the arcade manufacturers would reuse pieces of their designs multiple times in order to save on costs and time.<br>
Some of these smaller circuits would reappear in later boards that had minimal common ground with the previous boards that used the circuit, so you couldn’t just have them share the circuit/ROM data through a normal parent/clone relationship. Instead, these re-used designs and ROM data are categorized as a Device, with the data stored as a Device set. For instance, Namco used the Namco 51xx custom I/O chip to handle the joystick and DIP switches for Galaga and other games, and as such you’ll also need the NAMCO51.ZIP device set as well as any needed for the game.<br>
<br>
These sets come in handy specifically when you collect PARTIAL sets of the merged or split kind - OR if you collect JUST the SL ROMs set, and NOT the MAME ROMs set at all.<br>
- Another use is for different emulators/systems that often require specific BIOS files.<br>
- Note: If you collect MAME and Software List FULL sets, then these files are included in the sets, and there is no specific need for you to download these as well.<br>

<b>HBMAME full sets:</b>

HBMAME ROMs<br>
Set: [HBMAME 0.240 ROMs (merged)](http://mgnet.me/eqwB3o7)<br>
Datfile: [HBMAME 0.240 ROMs (merged)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 ROMs (merged).zip)<br>
HBMAME CHDs<br>
Datfile: [HBMAME 0.240 CHDs (merged)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 CHDs (merged).zip)<br>
Datfile (dir2dat): [HBMAME 0.240 CHDs (merged) (dir2dat)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 CHDs (merged) (dir2dat).zip)<br>

<b>HBMAME Rollback full sets:</b>

HBMAME Rollback ROMs<br>
Set: [HBMAME 0.240 Rollback ROMs](http://mgnet.me/eqwB3o0)<br>
Datfile: [HBMAME 0.240 Rollback ROMs](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 Rollback ROMs.zip)<br>
HBMAME Rollback CHDs<br>
Datfile: [HBMAME 0.240 Rollback CHDs](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 Rollback CHDs.zip)<br>
Datfile (dir2dat): [HBMAME 0.240 Rollback CHDs (dir2dat)](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/HBMAME 0.240 Rollback CHDs (dir2dat).zip)<br>
[HBMAME datfile archive](https://github.com/pleasuredome/pleasuredome/raw/gh-pages/hbmame/MisfitMAME_HBMAME_ROMs.7z)

<b>Guide:</b>

[MAME ROMs Set Creation using a dir2dat](https://pleasuredome.miraheze.org/wiki/MAME_ROMs_Set_Creation_using_a_dir2dat)<br>

<b>Merging explained:</b>

split:<br>
A <b>split set</b> is one where the parent set contains all of the normal data it should, and the clone sets contain only what has changed as compared to the parent set.<br>
This saves some space, but isn’t quite as efficient as a merged set.<br>
The clone sets can't operate without their parent set.<br>
Remark: The parent and clones in split sets DO NOT include BIOS or DEVICE files - they are separate files within the set (An example would be 100lions (No BIOS in the parent) and Galaga (No device file in the parent) - This is per MAME design<br>
<br>
merged:<br>
A <b>merged set</b> takes the parent set and one or more clone sets and puts them all inside the parent set’s storage.<br>
To use the existing Pac-Man example, combining the Puckman, Midway Pac-Man (USA) sets, along with various bootleg versions– and combining it all into PUCKMAN.ZIP, would be making a merged set.<br>
Remark: The parent games in a merged set DO NOT include BIOS or DEVICE files - they are separate files within the set (An example would be 100lions (No BIOS in the parent) and Galaga (No device file in the parent) - This is per MAME design<br>
<br>
non-merged:<br>
A <b>non-merged set</b> is one that contains absolutely everything necessary for a given game to run in one ZIP file.<br>
Remark: Even though Non-Merged games -normally- DO NOT include BIOS or DEVICE files within the game, in the case of the PD non-merged set we DO include these within the game, which ensures that every single game can be copied and ran as individual game without the need of any extra files.<br>
This makes a set like this ideal for splitting up on a per-game-basis.
The non-merged set is ideal for those people that work on Arcade PCBs as ALL roms/devices/bios files are contained within the game. This set is also great for those that for instance create their own arcade cabinets and want to copy only very specific games to their PC/Rapsberry/Other, the game.zip file contain all the files needed, no more searching for the dependent parent files, BIOS files, device files - just copy galaga.zip and you are set.<br>
Pick individual games from this set if you are not intending to download a complete ROM set.
