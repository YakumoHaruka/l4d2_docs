## Known Problems of Community Campaigns   

Here lists the known Left4Dead2 community campaigns suffering from various problems.  It's **NOT** a complete list. The problems listed here were found in the specific version of the campaigns, which indicated by a update time after the download links of that campaign. Authors of specific campaign may update and fix the problems they found. There's no guarantee that I would have noticed of the campaign updates and perform a check and update process on this list. So please **DO NOT** apply any fixes listed here unless you have actually encountered the exact problems described here.  

[TOC]

---

### Alien Trilogy: Section 1
`[chi]` 异形三部曲：第一章  
*alientrilogy_section1_V1_1.vpk*  
[[GameMaps](https://www.gamemaps.com/details/3075)] *Updated: 10/21/11*  
 `Malformed Mission File`  

- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/alientri.txt).   
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### A Path To Exit  
`[chi]` 一条退路  
*apathtoexit.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19892)] *Updated: 03/15/18*  
 `Malformed Mission File`  

- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/apathtoexit.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Blackout Extended  
`[chi]` 灯火管制 加长版  /  `[chi]` 灯火管制  
*blackout_extended.vpk*  
[[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0330/571.html)] *Updated: 03/31/14*  
[[3DMGame](https://dl.3dmgame.com/patch/102073.html)] *Updated: 04/06/17*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file contains non-existing versus/survival map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/blackout_extended.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Burning Night  
`[chi]` 燃烧之夜  
*burningnight.vpk*  
[[GameMaps](https://www.gamemaps.com/details/15991)] *Updated: 01/03/16*  
`Stringtable Dictionary Missing`  /  `Low Uniqueness Map Names`  

- Because of the low uniqueness map names of this campaign, this campaign would easily conflicts with some others. As far as I known, map 2 `streets` conflicts with `Dead St 16` map 2, and map 3 `factory` conflicts with `Left 4 Dust 2` map 1. Currently I have no perfect solution to this problem. You may either not to host the conflicting campaigns at the same time, or try to reorder the addons in `left4dead2/addonlist.txt` manually.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required. 

---

### Centro  
`[chi]` 市中心  
*centro.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2368)] *Updated: 09/19/10*  
[[OrangesGame](http://www.orangesgame.com/map/20150826/43.html)] *Updated: 08/26/15*  
`Survivor Spawn Position Issue` 

- On first map, the survivor spawns on top of a very high building, and the ground is not flat. On a dedicated server, I found that sometimes the player would spawn under the ground, falls to the bottom and dies. I made a [Stripper:Source map configuration file](https://github.com/YakumoHaruka/l4d2_docs/blob/master/stripper/maps/gasometer.cfg) to modify the `info_player_start` and `info_survivor_position` entities to higher posions. The result turns out fine.  

---

### China of the Dead  
`[chi]` 中国丧尸  
*chinaofthedead.vpk*  
[[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0323/527.html)] *Updated: 04/03/2013*  
 `Malformed Mission File`  

- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/kaplin.txt).  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### ClockTown Beta  
`[chi]` 钟镇  
*clocktown_beta.vpk*  
[[GameMaps](https://www.gamemaps.com/details/9631)] *Updated: 02/20/14*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Collaboration 2  
`[chi]` 合作 2  
*collaboration 2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19317)] *Updated: 09/21/17*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  /  `Wrong Map Name`  

- Due to a space character in the name of this mission, you can't start the map in the game. The space character in mission file name also cause some trouble to the ACS/LMM plugin.   
- The mission file contains invalid Image/OuttroImage/Poster settings. All the map's images are pointed to a non-existing file. Also, I suppose this campaign is designed to play with L4D1 survivor set because they are in the poster image. But the mission file is not specifying that, so by default there's the L4D2 survivor set in the game. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/collaboration2.txt) is my fixed version of the mission file, which has the space character in the file name removed.  
- The map files in mission file and in the VPK are named in the form of `l4d2_collabo0X_XXXXX.XXX`, yet the names inside the bsp files are named in the form of `l4d_collabo0X_XXXXX.XXX`. Whenever players get to the safe room in any map of this campaign, the next map will failed to load. To solve this, you have to rename the `.bsp` and `.nav` files in the VPK, and modify the mission file accordingly.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Convoy  
`[chi]` 车队  
*convoy.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7574)] *Updated: 10/16/13*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/convoy.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Crescendo Collision  
`[chi]` 激情碰撞  
*crescendocollision.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6704)] *Updated: 05/11/13*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Days Repeat  
`[chi]` 重复的日子  
*daysrepeat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20083)] *Updated: 05/04/18*  
 `Malformed Mission File`  

- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/daysrepeat.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Dead Jail  
`[chi]` 死亡监狱  
*dead_jail_hard.vpk*  
[[GameMaps](https://www.gamemaps.com/details/14005)] *Updated: 01/30/15*  
`Stringtable Dictionary Missing`  /  `Nested VPK File`  

- There's another `dead_jail_hard.vpk` within the `dead_jail_hard.vpk` which seemed to be a packing problem of the author.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Dead Mines II  
`[chi]` 死亡矿井 2  
*deadmines2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/17974)] *Updated: 02/13/17*  
 `Stringtable Dictionary Missing`   

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Dead on Time 2  
`[chi]` 死亡时刻 2  
*deadontime2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2416)] *Updated: 02/26/10*  
 `Stringtable Dictionary Missing`  /   `Malformed Mission File`  

- Mission file contains inactive survival/scavenge map settings. A removed version can be found [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/deadontimeii.txt).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Dead St 16  
`[chi]` 死圣  
*DeadSt16.vpk*  
[[GameMaps](https://www.gamemaps.com/details/5673)] *Updated: 01/01/16*  
`Low Uniqueness Map Names`  

- Because of the low uniqueness map names of this campaign, this campaign would easily conflicts with some others. As far as I known, map 2 `streets` conflicts with `Burning Night` map 2. Currently I have no perfect solution to this problem. You may either not to host the conflicting campaigns at the same time, or try to reorder the addons in `left4dead2/addonlist.txt` manually.  

---

### Death Hour  
`[chi]` 死亡时间  
*death_hour.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2392)] *Updated: 09/27/10*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Escape from Malabar  
`[chi]` 逃离马拉巴尔  
*exmala_v7.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2513)] *Updated: 08/27/11*  
 `Malformed Mission File`  

- The poster section of the mission file causes parse error due to a  line of description which should be commented. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/exmala.txt) is a simple fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Forgotten Mist  
`[chi]` 被遗忘的迷雾  
*forgottenmist.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8240)] *Updated: 06/02/13*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Freddy Fazbear's Pizzeria  
`[chi]` 玩具熊的披萨餐厅  
*fnaf1v3.vpk*  
[[GameMaps](https://www.gamemaps.com/details/14164)] *Updated: 01/01/19*  
 `Malformed Mission File`  

- Unexpected newlines in mission description.  
- The 5th map's image setting in mission file contains an invalid character `?`. As long as there's no such thing as the 5th map's image, I used the 4th map's image to fix this problem. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/fnaf1.txt) is my fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  

---

### Haha  
`[chi]` 哈哈  
*HAHA1.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19241)] *Updated: 08/21/17*  
 `Stringtable Dictionary Missing`  /  `Mission File Name Confliction`  

- Mission file name `hits.txt` conflicts with [[The Lost Tutorial](https://www.gamemaps.com/details/3680)]. Rename it if you have to host them both.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Halls Of Death  
`[chi]` 死亡大厅  
*hallsofdeathv2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/5559)] *Updated: 10/06/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file contains empty survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/hallsofdeath.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Heartbreak Fridge  
`[chi]` 冰冷的心  
*heartbreakfridge.vpk*  
[[GameMaps](https://www.gamemaps.com/details/3278)] *Updated: 09/19/11*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### hehe 2  
`[chi]` 呵呵 2  
*hehe2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18542)] *Updated: 05/13/17*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### hehe 4  
`[chi]` 呵呵 4  
*hehe4.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18224)] *Updated: 03/25/17*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### hehe 8  
`[chi]` 呵呵 8  
*hehe8.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20341)] *Updated: 07/06/18*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Hystyria  
`[chi]` 歇斯底里  /  `[chi]` 海斯特里亚  /  `[chi]` 逃离施蒂里亚  
*hystyria.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8066)] *Updated: 05/02/13*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Kicked Out: Chapter 4  
`[chi]` 踢出  
*kickedout.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8091)] *Updated: 05/14/13*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Labirinferno  
`[chi]` 地狱迷宫  
*labirinferno.vpk*  
[[GameMaps](https://www.gamemaps.com/details/15286)] *Updated: 08/21/15*  
`Malformed Mission File`  

- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/labirinferno.txt).  
- Only the `server` side needs to redeploy the repaired VPK file.  

---

### Last HeartBeat (2.0)  
`[chi]` 最后的心跳  
*lastheartbeat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4142)] *Updated: 02/02/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/lastheartbeat.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Last Ride  
`[chi]` 最后的旅程  
*lastride.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16525)] *Updated: 03/28/16*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Left4Doom (1.0)  
`[chi]` 求生之毁灭战士  
*left4doom.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2410)] *Updated: 12/24/09*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Left 4 Dust 2  
`[chi]` 尘埃 2  
*left4dust2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7073)] *Updated: 06/16/13*  
 `Malformed Mission File`  

- The 3,5,6,8,10 map sections in the mission file are missing the name strings before them. I don't know whether this is on purpose, in order to hide these maps? Also, there are some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/left4dust2.txt) is my fixed version.  
- Players reported that there are some other problems in game, I have not investigated yet.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Left In Prypiat  
`[chi]` 逃离普里皮亚季  
*leftinprypiat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16942)] *Updated: 08/21/16*  
 `Malformed Mission File`  

- The name of `coop_boss_spawning` section in the mission file is commented, leaving the section dangled. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/leftinprypiat.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Let's Build 2 Core  
`[chi]` 一起来建造2：核心  
*lb2core.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4257)] *Updated: 10/14/13*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Mass Maze  
`[chi]` 大迷宫  
*mass_maze.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4371)] *Updated: 12/25/16*  
 `Stringtable Dictionary Missing`  /  `Wrong Map Name`  

- The second map's name should be `mass_maze_2nd_stage.bsp` but the actual file was named `mass_maze_2nd_stage_d.bsp`.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### My Fear  
`[chi]` 我的恐惧  
*myfear.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7656)] *Updated: 07/22/13*  
[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0815/1036.html) Update: 08/15/13  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/myfear.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Napalm Death  
`[chi]` 死亡汽油弹  
*napalmdeath.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2601)] *Updated: 08/18/11*  
`Malformed Mission File`  

- Mission file has invalid survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/thorfinnmap4.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  

---

### No Fate 2  
`[chi]` 绝非宿命 2  
*nofate2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18033)] *Updated: 02/19/17*  
`Classname Missing From Entity`  

- There's no known solution to this problem for me currently.   
  
---

### Power Station  
`[chi]` 地下供电所  
*l4d2_powerstation.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7339)] *Updated: 01/21/13*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Resident Evil: Outbreak  
`[chi]` 生化危机：爆发  
*Outbreak.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2526)] *Updated: 10/12/16*  
`ED_Alloc`  

- The 2nd map `re_outbreak` has a very high `edict` count (about 2000 when there are 1 human and 3 survivor bots) from the beginning, which will easily exceed the entity limit when hosted on a dedicated server for more than 4 survivors, result in an `ED_Alloc` error. I wrote a [Stripper:Source map configuration file](https://github.com/YakumoHaruka/l4d2_docs/blob/master/stripper/maps/re_outbreak.cfg), managed to reduce the entity number in the map to around 1500. Still need some live tests on our 16 survivors server.  
- The 5th map `re_hellfire` also has a fairly high `edict` count (around 1600 when there are 1 human and 3 survivor bots) from the beginning. Here's a [Stripper:Source map configuration file](https://github.com/YakumoHaruka/l4d2_docs/blob/master/stripper/maps/re_hellfire.cfg) managed to reduce the entity number in the map to around 1500. Still need some live tests on our 16 survivors server.  

---

### Road To F18 
`[chi]` 空军之路  /  `[chi]` F18之路  
*road_to_f18_v1.1.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20891)] *Updated: 12/24/18*  
`Melee Weapon Banned`  

- Actually this isn't a real problem. The melee weapons are banned on purpose by the author. If you use a sourcemod plugin like the `l4d2_melee_in_the_saferoom`, a bunch of hunter claws will be spawned instead. If your server really needs melee weapons to work with, you can modify the mission file to enable them, like [this](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/roadtof18.txt). Only the server side needs to redeploy the modified VPK.  

---

### Rural Tour  
`[chi]` 喋血乡间  
*253090805.vpk*  
[[SteamWorkshop](https://steamcommunity.com/sharedfiles/filedetails/?id=253090805)] *Updated: 04/27/14*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Shadow Moses Island  
`[chi]` 摩西岛阴影  
*shadowmosesisland.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2600)] *Updated: 07/22/13*  
 `Malformed Mission File`  

- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/shadowmosesisland.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Silent Hill: Otherside of Life  
`[chi]` 寂静岭：另一边的生活  /  `[chi]` 寂静岭：对方的生活  
*silenthillool_4_7.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7592)] *Updated: 11/03/14*  
`Malformed Mission File`  

- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/shool.txt).  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Skipping Class  
`[chi]` 逃课  
*skipping_class.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6730)] *Updated: 07/04/13*  
[[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0127/188.html)] *Updated: 05/08/14*  
`Malformed Mission File`  

- The coop section of the mission file is not closed, while there are invalid versus/survival/scavenge map configurations derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/skippingclass.txt). 
- The mission file was named `data inside.txt` which contains a space character. This doesn't cause problem, but I renamed it to `skippingclass.txt` in the fix for better reading.  
- Only the `server` side needs to redeploy the repaired VPK file.  

---

### Solemn Blackout  
`[chi]` 圣光熄灭  
*SolemnBlackout.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2389)] *Updated: 10/14/10*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- The mission file contains a scavenge map section with an invalid name `"0"`.  A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/solemnblackout.txt).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### somefun  
`[chi]` 些许有趣的东东  
*somefun.vpk*  
[[GameMaps](https://www.gamemaps.com/details/9391)] *Updated: 01/12/14*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### South Street 3  
`[chi]` 南大街 3  
*southstreet3.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18196)] *Updated: 03/19/17*  
 `Malformed Mission File`  

- `OuttroImage` in the mission file missing the `vgui\` prefix.  
- Survival mode sections in the mission file are missing the names of them, and a pair of outer brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/southstreet-3.txt) is a simple fix for all these problems.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Space Trip REVAMP (port)  
`[chi]` 太空之旅  
*space trip revamp.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8219)] *Updated: 05/21/13*  
`Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/spacetriprevamp.txt) is a fix. 
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Stargate SG-4 v2  
`[chi]` 星际之门2  
*stargate2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6963)] *Updated: 01/31/17*  
[[Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=854169313)] *Updated: 10/13/18*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Storming The Citadel  
`[chi]` 风暴要塞  
*stormingcitadelalpha.vpk*  
[[GameMaps](https://www.gamemaps.com/details/14876)] *Updated: 10/11/15*  
`Stringtable Dictionary Missing`  /  `Malformed Mission File`  

- Mission file has invalid versus/survival/scavenge/holdout map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/stormingcitadelalpha.txt) is a fix.  And, according to the author's comment,  only the first 2 maps are actually released as playable. 
- Redistribution of the repaired VPK file to both the `server` and `client` side is required. 

---

### Tai Chi  
`[chi]` 太极  
*taiji.vpk*  
[[GameMaps](https://www.gamemaps.com/details/9524)] *Updated: 02/27/14*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required. 

---

### The Ancient Maze  
`[chi]` 古代迷宫  
*the_ancient_maze.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2811)] *Updated: 05/04/11*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### The Coaster  
`[chi]` 过山车   /  `[chi]` 港口  
*l4d2_thecoaster.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19484)] *Updated: 11/15/17*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### The Parish Original Beta Map  
`[chi]` 教区原貌  
*parishbeta.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8117)] *Updated: 02/13/14*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### The Police Department  
`[chi]`  警察局  
*thepolicedepartment.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6918)] *Updated: 03/13/13*  
 `Malformed Mission File`  

- An needless mission file `mission_manifest_sample.txt` in the missions folder. It is not a valid mission file, `l4d2_mission_manager` plugin will complain for this every time you start the server.  
- The mission file has an invalid outtro image setting, and some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/rpstation.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### The Punisher  
`[chi]` 惩罚者  
*gamemaps-thepunisher.vpk*  
[[GameMaps](https://www.gamemaps.com/details/17170)] *Updated: 08/23/16*  
 `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/thepunisher.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### The Woods   
`[chi]` 森林  
*the woods.vpk*   
[[GameMaps](https://www.gamemaps.com/details/18307)] *Updated: 04/09/17*  
 `Stringtable Dictionary Missing`  /  `Wrong Map Name`  

- The mission file describes the map names as `l4d_thewoods02` `l4d_thewoods03` and so does the actual BSP and NAV files named. But the map names within the BSP files are written `l4d_thewoods_02` `l4d_thewoods_03`. Thus when players make their way to the safe room in first map, the loading screen comes and goes, but there's no actual map change happens. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/thewoods.txt) is a fix to this problem.  And you will need to rename the BSP and NAV files' name as well.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Traps Map 3.0  
`[chi]` 陷阱地图 3.0  
*trapsmap_3_-_08_01_2011.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2652)] *Updated: 01/08/11*  
 `Stringtable Dictionary Missing`  /  `Mission Name Confliction`  

- Mission name conflicts with the example campaign `DeadLine2`. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/trapsmap.txt) is a simple fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Twisted Fates  
`[chi]` 曲折的命运  
*twistedfates.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8065)] *Updated: 05/02/13*  
`Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required. 

---

### Unreal Tournament  
`[chi]` 虚幻锦标赛  
*l4d2unreal.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2484)] *Updated: 03/26/10*  
 `Stringtable Dictionary Missing`  

- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---

### Warp Core  
`[chi]` 曲速核心  
*WARPCORE.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7853)] *Updated: 12/15/13*  
`Malformed Mission File`  

- Mission file has invalid survival map id, and the brackets are unpaired. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/warpcore.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file. 

---

### Whispers In The Dark  
`[chi]` 暗中低语  
*whispersinthedark.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16615)] *Updated: 04/13/16*  
 `Malformed Mission File`  

- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/whispersdark.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---

### Zelda beta (l4d2)  
`[chi]` 塞尔达测试版  /  `[chi]` 塞尔达传说  
*zelda.vpk*  
[[GameMaps](https://www.gamemaps.com/details/5767)] *Updated: 07/16/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  /  `Mission Name Confliction`  /  `info_landmark Error`  

- Mission name conflicts with `Power Station`. The `addontitle` in `addoninfo.txt` and `Name` in  mission file needs to be modified. What's even worse is that the mission file name itself also the same as in `Power Station`. If your server plans on hosting both mission, you need to unpack, rename the mission file to something else like `zelda.txt`, fix the content of it and the `addoninfo.txt`, then pack it up again. A redistribution of the repaired VPK file to your client is inevitable. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/zelda.txt) is a fix of the mission file, which has been renamed to `zelda.txt`.  
- The position at the end of the first map links to the second map with an info_landmark entity. However, the info_landmark entity's position is almost 900 units from the ground. So if players successfully made their way to the safe room of the first map, most (if not all) of them will fall and dead at the beginning of the second map. This can be fix with a [Stripper:Source map configuration file](https://github.com/YakumoHaruka/l4d2_docs/blob/master/stripper/maps/l4d_zelda02.cfg).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  

---

### Zero Warning  
`[chi]` 没有警告  
*1622008461.vpk*  /  *myl4d2addons zero warning campaign.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20963)] *Updated: 01/13/19*  
[[SteamWorkshop](https://steamcommunity.com/sharedfiles/filedetails/?id=1622008461)] *Updated: 01/12/19*  
`Malformed Mission File`  /  `Long Loading Time`  

- When round restarts, there's a significant long pause, which would trigger the dedicated server's watchdog mechanism to raise a SIGALRM signal and restarts the server process. I have to shutdown the watchdog mechanism of the server before I found out what cause the problem and fix it.  


