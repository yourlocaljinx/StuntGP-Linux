# StuntGP-Linux
## running stuntgp on linux and limitations.

# Special Thanks to:
## The community on the [Trickstart](https://discord.gg/ykzAWnA) Discord Server

# DISCLAIMER!
## This was tested on linux **Manjaro** with Sway DE. i *don't know* if it works on other distros

# Prerequisites
> [Wine](https://www.winehq.org/)

> [PlayOnLinux](https://www.playonlinux.com/en/)

> [A StuntGP Iso](https://www.myabandonware.com/game/stunt-gp-ddu)

> [StuntKit](https://github.com/stuntkit/StuntKit) and [SkScreen Module](https://github.com/stuntkit/StuntKit_modules/releases/tag/v0.3.0) (Optional): [SkFreeze Module](https://github.com/stuntkit/StuntKit_modules/releases/tag/v0.3.0).

> And most importantly patience (A LOT OF PATIENCE)

# INSTALLATION
1) Extract the StuntGP iso to a directory accessible to playonlinux
2) Click Install Program on PlayOnLinux
3) Click Install a program thats not present in the list, it should open a window titled "Manual Installation"
4) Click Next
5) Click "Install program in a new virtual drive", and type a name like "stuntgp", this will be the name of the wine directory and prefix
6) Click Next, in this window we want to check the configure wine option, a new winecfg window will open, we are going to switch the windows version from **Windows 10** to **Windows XP**. after changing close this window and click next.
7) Click 64 bits windows installation
8) Then click explore and select the "Setup.exe" file inside the iso you extracted earlier, do not select the autorun.exe file, it wont install SGP
9) Install Stunt GP normally, relax while the installation finishes =)
10) After the installation finishes add a shortcut to the "StuntGP - Configuration" program
11) Close the playonlinux installation window and open the Configuration program, this is going to generate the GAME.CGF file that we need to set our monitor resolution, apply the configuration and click ok.
12) In playonlinux click the "open directory" button and copy the SKScreen module (and the SKFreeze one if you downloaded it) and the StuntKit loader in the game's root folder.
13) edit GAME.CFG with your preferred text editor: set "DISPLAYRESWIDTH" to the **width** of your resolution (For example: 1920) and set "DISPLAYRESHEIGHT" to the **height** of your resolution (For Example: 1080) and save the file.
14) On PlayOnLinux now click Configure click on the name of the wineprefix you set before (Step 5), and click Create a new shortcut, then select the **StuntKit_D3D.exe** and close the window.
15) And Done!

# FAQ:
## Why not use steam and proton?
> it seems that proton **doesn't** support directx7 which is needed for StuntGP to run
## Is there a simpler way?
> Surely there is, i just dont know how to do it and i got the best results with this method
## Why Not running it with just WINE?
> i don't know why but wine just refuses to start the StuntGP.exe file
## Will this repo be updated if you find a simpler method
> Yes it will.
## Isn't there a compiled StuntGP linux version?
> No, linux wasn't very popular (and was very limited) at the time StuntGP released, so Team17 never did a linux version for the game
