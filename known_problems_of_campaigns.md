## Known Problems of Community Campaigns   
  
Here lists the known Left4Dead2 community campaigns suffering from various problems.  It's **NOT** a complete list. The problems listed here were found in the specific version of the campaigns, which indicated by a update time after the download links of that campaign. Authors of specific campaign may update and fix the problems they found. There's no guarantee that I would have noticed of the campaign updates and perform a check and update process on this list. So please **DO NOT** apply any fixes listed here unless you have actually encountered the exact problems described here.  
  
---  
  
**Alien Trilogy: Section 1**  
`[chi]` 异形三部曲：第一章  
*alientrilogy_section1_V1_1.vpk*  
[[GameMaps](https://www.gamemaps.com/details/3075)] *Updated: 10/21/11*  
 `Malformed Mission File`  
  
- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/alientri.txt).   
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**A Path To Exit**  
`[chi]` 一条退路  
*apathtoexit.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19892)] *Updated: 03/15/18*  
 `Malformed Mission File`  
  
- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/apathtoexit.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Blackout Extended**  
`[chi]` 灯火管制 加长版  /  `[chi]` 灯火管制  
*blackout_extended.vpk*  
[[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0330/571.html)] *Updated: 03/31/14*  
[[3DMGame](https://dl.3dmgame.com/patch/102073.html)] *Updated: 04/06/17*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Mission file contains non-existing versus/survival map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/blackout_extended.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**China of the Dead**  
`[chi]` 中国丧尸  
*chinaofthedead.vpk*  
[[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0323/527.html)] *Updated: 04/03/2013*  
 `Malformed Mission File`  
  
- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/kaplin.txt).  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Collaboration 2**  
`[chi]` 合作 2  
*collaboration 2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19317)] *Updated: 09/21/17*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Due to a space character in the name of this mission, you can't start the map in the game. The space character in mission file name also cause some trouble to the ACS/LMM plugin.   
- The mission file contains invalid Image/OuttroImage/Poster settings. All the map's images are pointed to a non-existing file. Also, I suppose this campaign is designed to play with L4D1 survivor set because they are in the poster image. But the mission file is not specifying that, so by default there's the L4D2 survivor set in the game. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/collaboration2.txt) is my fixed version of the mission file, which has the space character in the file name removed.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Convoy**  
`[chi]` 车队  
*convoy.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7574)] *Updated: 10/16/13*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/convoy.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Crescendo Collision**  
`[chi]` 激情碰撞  
*crescendocollision.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6704)] *Updated: 05/11/13*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Days Repeat**  
`[chi]` 重复的日子  
*daysrepeat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20083)] *Updated: 05/04/18*  
 `Malformed Mission File`  
  
- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/daysrepeat.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Dead Mines II**  
`[chi]` 死亡矿井 2  
*deadmines2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/17974)] *Updated: 02/13/17*  
 `Stringtable Dictionary Missing`   
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Dead on Time 2**  
`[chi]` 死亡时刻 2  
*deadontime2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2416)] *Updated: 02/26/10*  
 `Stringtable Dictionary Missing`  /   `Malformed Mission File`  
  
- Mission file contains inactive survival/scavenge map settings. A removed version can be found [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/deadontimeii.txt).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Death Hour**  
`[chi]` 死亡时间  
*death_hour.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2392)] *Updated: 09/27/10*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Escape from Malabar**  
`[chi]` 逃离马拉巴尔  
*exmala_v7.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2513)] *Updated: 08/27/11*  
 `Malformed Mission File`  
  
- The poster section of the mission file causes parse error due to a  line of description which should be commented. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/exmala.txt) is a simple fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Forgotten Mist**  
`[chi]` 被遗忘的迷雾  
*forgottenmist.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8240)] *Updated: 06/02/13*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Haha**  
`[chi]` 哈哈  
*HAHA1.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19241)] *Updated: 08/21/17*  
 `Stringtable Dictionary Missing`  /  `Mission File Name Confliction`  
  
- Mission file name `hits.txt` conflicts with [[The Lost Tutorial](https://www.gamemaps.com/details/3680)]. Rename it if you have to host them both.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Halls Of Death**  
`[chi]` 死亡大厅  
*hallsofdeathv2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/5559)] *Updated: 10/06/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Mission file contains empty survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/hallsofdeath.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Heartbreak Fridge**  
`[chi]` 冰冷的心  
*heartbreakfridge.vpk*  
[[GameMaps](https://www.gamemaps.com/details/3278)] *Updated: 09/19/11*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**hehe 2**  
`[chi]` 呵呵 2  
*hehe2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18542)] *Updated: 05/13/17*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**hehe 4**  
`[chi]` 呵呵 4  
*hehe4.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18224)] *Updated: 03/25/17*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**hehe 8**  
`[chi]` 呵呵 8  
*hehe8.vpk*  
[[GameMaps](https://www.gamemaps.com/details/20341)] *Updated: 07/06/18*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Kicked Out: Chapter 4**  
`[chi]` 踢出  
*kickedout.vpk*  
[[GameMaps](https://www.gamemaps.com/details/8091)] *Updated: 05/14/13*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Last HeartBeat (2.0)**  
`[chi]` 最后的心跳  
*lastheartbeat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4142)] *Updated: 02/02/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/lastheartbeat.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Last Ride**  
`[chi]` 最后的旅程  
*lastride.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16525)] *Updated: 03/28/16*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Left4Doom (1.0)**  
`[chi]` 求生之毁灭战士  
*left4doom.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2410)] *Updated: 12/24/09*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Left 4 Dust 2**  
`[chi]` 尘埃 2  
*left4dust2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7073)] *Updated: 06/16/13*  
 `Malformed Mission File`  
  
- The 3,5,6,8,10 map sections in the mission file are missing the name strings before them. I don't know whether this is on purpose, in order to hide these maps? Also, there are some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/left4dust2.txt) is my fixed version.  
- Players reported that there are some other problems in game, I have not investigated yet.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Left In Prypiat**  
`[chi]` 逃离普里皮亚季  
*leftinprypiat.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16942)] *Updated: 08/21/16*  
 `Malformed Mission File`  
  
- The name of `coop_boss_spawning` section in the mission file is commented, leaving the section dangled. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/leftinprypiat.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Let's Build 2 Core**  
`[chi]` 一起来建造2：核心  
*lb2core.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4257)] *Updated: 10/14/13*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Mass Maze**  
`[chi]` 大迷宫  
*mass_maze.vpk*  
[[GameMaps](https://www.gamemaps.com/details/4371)] *Updated: 12/25/16*  
 `Stringtable Dictionary Missing`  /  `Wrong Map Name`  
  
- The second map's name should be `mass_maze_2nd_stage.bsp` but the actual file was named `mass_maze_2nd_stage_d.bsp`.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**My Fear**  
`[chi]` 我的恐惧  
*myfear.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7656)] *Updated: 07/22/13*  
[L4D2.cc](http://www.kk175.com/map/hezuo/2013/0815/1036.html) Update: 08/15/13  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/myfear.txt) is a fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**No Fate 2**  
`[chi]` 绝非宿命 2  
*nofate2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18033)] *Updated: 02/19/17*  
`Classname Missing From Entity`  
  
- There's no known solution to this problem for me currently.   
  
---  
  
**Power Station**  
`[chi]` 地下供电所  
*l4d2_powerstation.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7339)] *Updated: 01/21/13*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Shadow Moses Island**  
`[chi]` 摩西岛阴影  
*shadowmosesisland.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2600)] *Updated: 07/22/13*  
 `Malformed Mission File`  
  
- Mission file contains empty versus/survival/scavenge map configurations. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/shadowmosesisland.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Silent Hill: Otherside of Life**  
`[chi]` 寂静岭：另一边的生活  /  `[chi]` 寂静岭：对方的生活  
*silenthillool_4_7.vpk*  
[[GameMaps](https://www.gamemaps.com/details/7592)] *Updated: 11/03/14*  
`Malformed Mission File`  
  
- The mission file contains the non-existing versus/survival/scavenge map configurations likely derived from the `Deadline2` example campaign. A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/shool.txt).  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Solemn Blackout**  
`[chi]` 圣光熄灭  
*SolemnBlackout.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2389)] *Updated: 10/14/10*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  
  
- The mission file contains a scavenge map section with an invalid name `"0"`.  A simple fix [here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/solemnblackout.txt).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**somefun**  
`[chi]` 些许有趣的东东  
*somefun.vpk*  
[[GameMaps](https://www.gamemaps.com/details/9391)] *Updated: 01/12/14*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**South Street 3**  
`[chi]` 南大街 3  
*southstreet3.vpk*  
[[GameMaps](https://www.gamemaps.com/details/18196)] *Updated: 03/19/17*  
 `Malformed Mission File`  
  
- `OuttroImage` in the mission file missing the `vgui\` prefix.  
- Survival mode sections in the mission file are missing the names of them, and a pair of outer brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/southstreet-3.txt) is a simple fix for all these problems.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Stargate SG-4 v2**  
`[chi]` 星际之门2  
*stargate2.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6963)] *Updated: 01/31/17*  
[[Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=854169313)] *Updated: 10/13/18*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**The Ancient Maze**  
`[chi]` 古代迷宫  
*the_ancient_maze.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2811)] *Updated: 05/04/11*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**The Coaster**  
`[chi]` 过山车   /  `[chi]` 港口  
*l4d2_thecoaster.vpk*  
[[GameMaps](https://www.gamemaps.com/details/19484)] *Updated: 11/15/17*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**The Police Department**  
`[chi]`  警察局  
*thepolicedepartment.vpk*  
[[GameMaps](https://www.gamemaps.com/details/6918)] *Updated: 03/13/13*  
 `Malformed Mission File`  
  
- An needless mission file `mission_manifest_sample.txt` in the missions folder. It is not a valid mission file, `l4d2_mission_manager` plugin will complain for this every time you start the server.  
- The mission file has an invalid outtro image setting, and some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/rpstation.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**The Punisher**  
`[chi]` 惩罚者  
*gamemaps-thepunisher.vpk*  
[[GameMaps](https://www.gamemaps.com/details/17170)] *Updated: 08/23/16*  
 `Malformed Mission File`  
  
- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/thepunisher.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**The Woods**   
`[chi]` 森林  
*the woods.vpk*   
[[GameMaps](https://www.gamemaps.com/details/18307)] *Updated: 04/09/17*  
 `Stringtable Dictionary Missing`  /  `Wrong Map Name`  
  
- The mission file describes the map names as `l4d_thewoods02` `l4d_thewoods03` and so does the actual BSP and NAV files named. But the map names within the BSP files are written `l4d_thewoods_02` `l4d_thewoods_03`. Thus when players make their way to the safe room in first map, the loading screen comes and goes, but there's no actual map change happens. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/thewoods.txt) is a fix to this problem.  And you will need to rename the BSP and NAV files' name as well.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Traps Map 3.0**  
`[chi]` 陷阱地图 3.0  
*trapsmap_3_-_08_01_2011.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2652)] *Updated: 01/08/11*  
 `Stringtable Dictionary Missing`  /  `Mission Name Confliction`  
  
- Mission name conflicts with the example campaign `DeadLine2`. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/trapsmap.txt) is a simple fix.  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Unreal Tournament**  
`[chi]` 虚幻锦标赛  
*l4d2unreal.vpk*  
[[GameMaps](https://www.gamemaps.com/details/2484)] *Updated: 03/26/10*  
 `Stringtable Dictionary Missing`  
  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
---  
  
**Whispers In The Dark**  
`[chi]` 暗中低语  
*whispersinthedark.vpk*  
[[GameMaps](https://www.gamemaps.com/details/16615)] *Updated: 04/13/16*  
 `Malformed Mission File`  
  
- Mission file has some unpaired brackets. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/whispersdark.txt) is a fix.  
- Only the `server` side needs to redeploy the repaired VPK file.  
  
---  
  
**Zelda beta (l4d2)**  
`[chi]` 塞尔达测试版  /  `[chi]` 塞尔达传说  
*zelda.vpk*  
[[GameMaps](https://www.gamemaps.com/details/5767)] *Updated: 07/16/12*  
 `Stringtable Dictionary Missing`  /  `Malformed Mission File`  /  `Mission Name Confliction`  /  `info_landmark Error`  
  
- Mission name conflicts with `Power Station`. The `addontitle` in `addoninfo.txt` and `Name` in  mission file needs to be modified. What's even worse is that the mission file name itself also the same as in `Power Station`. If your server plans on hosting both mission, you need to unpack, rename the mission file to something else like `zelda.txt`, fix the content of it and the `addoninfo.txt`, then pack it up again. A redistribution of the repaired VPK file to your client is inevitable. [Here](https://github.com/YakumoHaruka/l4d2_docs/blob/master/fixed_mission_files/zelda.txt) is a fix of the mission file, which has been renamed to `zelda.txt`.  
- The position at the end of the first map links to the second map with an info_landmark entity. However, the info_landmark entity's position is almost 900 units from the ground. So if players successfully made their way to the safe room of the first map, most (if not all) of them will fall and dead at the beginning of the second map. This can be fix with a [Stripper:Source map configuration file](https://github.com/YakumoHaruka/l4d2_docs/blob/master/stripper/maps/l4d_zelda02.cfg).  
- Redistribution of the repaired VPK file to both the `server` and `client` side is required.  
  
