# pillars-memorial-patch
Small Xdelta patch to remove a transmisogynist message in Pillars of Eternity

**Disclaimer**

* I do not and never have worked at Obsidian, or on Pillars of Eternity, nor am I affiliated with the studio in any way. I'm not a game developer and I do not work in the games industry.
* This mod is provided as-is without express or implied warranty.
* I only have my Steam copy of the English version of Pillars of Eternity, and I do not know whether it will work with any other version of the game.
* This mod (consisting of the .xdelta patch file) is in the public domain.

The new game Pillars of Eternity by Obsidian includes "memorial" messages on in-game graves, as a Kickstarter backer reward. Unfortunately, Obsidian didn't vet the user-submitted messages well enough, and a transmisogynist "joke" ended up in the game. This is a small Xdelta patch to remove it.

(See https://twitter.com/icequeenerika/status/582161950202863616/photo/1)

This patch was generated with Xdelta 1.1. Xdelta is in a state of hosting flux at the moment due to the shutdown of Google Code, but versions up through 3.0f can still be found at http://sourceforge.net/projects/xdelta/.

Some GUI frontends are available for Xdelta. From the command line, after installing Xdelta, open a command prompt window and change to your Pillars of Eternity data folder (if you have the Steam version, this will be Steam/steamapps/common/Pillars of Eternity/PillarsOfEternity_Data). Copy the .xdelta patch to this location, and rename resources.assets to resources.assets.bak. Then enter the command
`xdelta patch resources.assets.bak resources.assets.xdelta resources.assets`

If Xdelta succeeds, the transmisogynist joke will be gone from your copy of the game. If you have the Steam version, you can delete resources.assets.bak. If you have the GoG version you may want to keep it; in case of problems, delete the patched resources.assets file and rename resources.assets.bak back to resources.assets and everything will be back to normal.

**NOTES**
* the patched resources.assets file has a different checksum, so it *will* fail Steam verification. This means that if you click "Verify Integrity of Game Cache" under the "Local Files" tab of the game properties window, the patch will be undone. There should be no other effect on the game, however.
* this mod is a rushed, hacky solution; I think it'll work in many cases, but I'd like to be clear that I think Obsidian should not have allowed that joke through in the first place, should officially apologize for having done so, and should issue an official patch obviating mine as soon as possible.
