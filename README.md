# Server PunkBuster Config for Call of Duty, Battlefield etc. #

You can checkout my Serverlist on Discord: https://discord.gg/A7vtjmw


Most Admins dont know how or are to lazy to configure PunkBuster. But without configuring, PB is only a lame dog.

This Config should give you the best protection for your Server.

You can edit settings as you wish, only the sky's the limit. But be aware that this config is universal, some settings might not work with all games, you have to test it.

Here you can find some Guides https://www.pbbans.com/information-center.html

Following games using PB and can be protected with actual Cheat detection signatures by using PBBans, GGCStream, ACI streaming services.
Also Procon https://myrcon.net/ can be used with the BF4DB Plugin https://bf4db.com/plugin to protect your Battlefield 4 Servers.

> [!NOTE]
> Your SERVER & Client need latest pb files inside pb folder - Auto Update should work for actual supported games like BF3 and BF4. If not; download & update them manually:
> - Supported Games: https://evenbalance.com/pbsetup.php
> - Legacy Games https://community.pbbans.com/files/category/7-legacy-punkbuster-files/
> - Mirror: https://github.com/BestNoob/PunkBusterFiles


> [!IMPORTANT]
> Remember that you always have to register on their website to use their service for your servers.


PBB = PBBans https://www.pbbans.com
AAPG - America's Army Proving Grounds, ~~America's Army 4~~, ~~Battlefield 1942~~, BF2 - Battlefield 2, ~~Battlefield 2142~~, BF3 - Battlefield 3, BF4 - Battlefield 4, ~~Battlefield Bad Company 2~~, BFH - Battlefield Hardline, CoD - Call of Duty, CoD2 - Call of Duty 2, CoD4 - Call of Duty 4, CoD:UO - Call of Duty United Offensive, CoDWaW - Call of Duty 5 World at War, ET - Enemy Territory, ~~Medal of Honor~~, ~~Medal of Honor Warfighter~~, ~~Quake Wars~~, HOS - Red Orchestra 2, RtCW - Return to Castle Wolfenstein


ACI = Anti Cheat Inc. http://www.anticheatinc.net
AAPG - America's Army Proving Grounds, ~~America's Army 3~~, BF3 - Battlefield 3, ~~Battlefield Bad Company 2~~, BF4 - Battlefield 4, BFH - Battlefield Hardline, ~~Medal of Honor Warfighter~~


~~GGC = Together Against Cheaters (Gemeinsam Gegen Cheater) https://www.ggc-stream.net/
America's Army 4
Battlefield 2
Battlefield 3
Battlefield 4
Battlefield Bad Company 2
Battlefield Hardline
Call of Duty 2
Call of Duty 4
Call of Duty United Offensive
Call of Duty 5 World at War
Enemy Territory
Medal of Honor
Medal of Honor Warfighter
Red Orchestra 2~~

> [!NOTE]
> ### If PB doesnt take over your config, for some reasons its needed that u write following in gameserver console: ###

- pb_sv_writecfg
- pb_sv_writecfg pbucon.use
- pb_sv_restart (wait 30 seconds until pb has been restarted)

now your server should be correctly listed for the PB streaming, and the settings should apply. After this you can re-add the lines of my server.cfg to the server.cfg and pbucon.use
(strg+a, strg+c, strg+v - copy and paste)

> [!NOTE]
> ### Special info for LINUX Servers: ###
On Linux servers you have to do the same steps but **additionally copy the content of your pb (PunkBuster) folder to "/cod4server/.callofduty4/pb/"**
If you dont set basepath and homepath it is creating a hidden folder (instead of the Windows AppData) but this folder is missing the needed pb files.
LINUX Servers need all the Windows (.dll) + Linux (.so) files inside the pb folder. (gamename_win32.zip & gamename_linux.zip) 
And remember to check .cfg File for Unix & UTF8, if its Windows, ANSI and BOM it can cause issues wiht older servers/games.

- pb_sv_writecfg
- pb_sv_writecfg pbucon.use
- pb_sv_restart (wait 30 seconds until pb has been restarted)

You can also add those lines via gameserverconsole to your existing server.cfg if you dont want to use mine:

- pb_sv_usessionlimit 10
- pb_sv_uconadd 1 66.55.152.232 pbbhub3-1 pbbanshub
- pb_sv_uconadd 1 66.55.152.233 pbbhub3-2 pbbanshub
- pb_sv_uconadd 1 66.55.152.234 pbbhub3-3 pbbanshub
- pb_sv_AutoUpdBan 1
- pb_sv_task 0 7200 pb_sv_ver
- pb_sv_task 0 86400 pb_sv_update

- pb_sv_writecfg
- pb_sv_writecfg pbucon.use
- pb_sv_restart

> [!NOTE]
> ### Update Info: At August 2024 PBBans HUB has changed to: ###
> - pb_sv_uconadd 1 "38.111.114.231" "pbbhub4-1" "pbbanshub"
> - pb_sv_uconadd 1 "38.111.114.249" "pbbhub4-2" "pbbanshub"
