FF7 game save structure for Okteta
==================================

This is a plugin for the KDE hex editor [Okteta](https://userbase.kde.org/Okteta),
to explore the structure of save files from the game
[Final Fantasy VII](https://en.wikipedia.org/wiki/Final_Fantasy_VII) by Square Enix.
I've tried it with the PC and Android versions, which use the same file format.
Now you can inspect your game stats in detail, max out your gil, or bring Aeris back.

If you do edit anything, you'll need to recalculate the checksum for that save slot.

Based on information from the Qhimm wiki: <http://wiki.qhimm.com/view/FF7/Savemap>

On the PC (Steam) version, I found my save files at: (within my home directory)
`Documents/Square Enix/FINAL FANTASY VII Steam/user_XXXXXXXX/saveXX.ff7`

On the Android version, I found my save files at:
`/sdcard/Android/data/com.square_enix.android_googleplay.FFVII/files/Documents/saveXX.ff7`

On the iOS version (you'll need to be jailbroken), I found my save files at: (hex part may vary)
`/var/mobile/Containers/Data/Application/4A9D9590-BB03-44F7-A2ED-58B09CC584C1/Documents/saveXX.ff7`

To install, clone/copy the contents (specifically, `metadata.desktop` and `main.osd`)
to their own directory under your user or system Okteta structures directory.
For me this means `~/.kde/share/apps/okteta/structures/ff7` or
`/usr/share/apps/okteta/structures/ff7`.
