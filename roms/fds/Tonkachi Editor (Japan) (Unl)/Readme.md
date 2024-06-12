# Rom hack for Super Mario Bros
# Instructions
[https://tasvideos.org/Forum/Topics/24615?CurrentPage=1&Highlight=524257#524257](https://tasvideos.org/Forum/Topics/24615?CurrentPage=1&Highlight=524257#524257)

## Steps

Okay, so this ROM hack originally came bundled with an unlicensed ROM hacking software for the FDS called "Tonkachi Editor". When said editor is loaded, it tells the user to eject the disk right away before presenting 2 menu options, one for editing any FDS game you insert, and another that gives an explanation on what the software does. The latter is more interesting, as it prompts the user to insert a Super Mario Bros. FDS disk, and then overwrite it with Tonkachi Mario's data. Currently, only one emulator supports swapping FDS disks (and I do mean disks, not sides of the same disk), namely a fork of Nintendulator called NintendulatorNRS.

Here's how it's done in the emulator:
Load the Tonkachi Editor FDS image.
Insert the disk, as the emulator does not do so automatically. (Game -> Insert 2.8 inch disk)
When the title screen appears, eject the disk.
Select the second option, which gives an explanation on what the software does (and later prompts the user to insert a FDS SMB1 disk)
Load the SMB1 FDS disk via File -> Load 2.8 inch disk set.
Wait for the screen to turn red, then insert the SMB1 disk (once again, Game -> Insert 2.8 inch disk)
The software will now write the data to the SMB1 disk.
(probably optional, but always good to check) Reset the emulator (CPU -> Hard Reset) with the now modified SMB1 disk still inserted, and play through 1-1 and see if it matches the temp encode.
Close the emulator, and it'll prompt the user to save the edited disk image as a new image file.

Note that this will produce a slightly different FDS image when going through this route; however, this TAS still syncs with it.

Here are the MD5 hashes of the editor, the unmodified game, and the resulting patched game (at least for me):

 `e19fcb32ff02b557b55cc39d6a9377e6                Tonkachi Editor (Japan) (Unl).fds`
 
 `293303fe565de2333bc1e4115d38fa3f                Super Mario Bros. (Japan).fds`
 
 `4725ea0219c48557403019a40d3defb9                Super Mario Bros. Tonkachi.fds`
