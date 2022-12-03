# fxserver-es_billboard
Es_billboard is a little rework of Es_mapper

# Work Standalone ( compatible Esx/Qbcore)

# Summary : 
- 1- Add security so that not everyone can use the script.
- 2- How activate es_billboard in game.
- 3- REGULAR Questions
- 4- CONVERT XML to YMAP
- 5- Replace Texture
- 6- Shortcut of es_billboard



# Add security so that not everyone can use the script



Add this line inside your cfg to add the permission

      add_ace group.admin billboard allow # allow admin to use billboard menu


exemple : 

      add_ace group.admin command allow # allow all commands for admin

      add_ace group.admin billboard allow # allow admin to use billboard menu
      add_principal identifier.steam:ID_HERE group.admin #replace "ID_HERE" by the id of the user you want set as admin
      add_principal identifier.license:ID_HERE group.admin #replace "ID_HERE" by the id of the user you want set as admin

      add_ace group.billboard # Create a new group for using billboard

      add_ace group.billboard billboard allow # allow billboard to use billboard menu
      add_principal identifier.steam:ID_HERE group.billboard #replace "ID_HERE" by the id of the user you want set as billboard
      add_principal identifier.license:ID_HERE group.billboard #replace "ID_HERE" by the id of the user you want set as billboard



# How activate es_billboard in game

On the console (F8) write " billboard ".
On the tchat write " /billboard ".
On your Keyboard press " F6 " .( You can edit the Key on your config key, press Esc , and check on your FIVEM OPTION KEY LIST)



# REGULAR Questions


 When i save my XML work, where it's save ?
- It's save on the folder "maps". ( es_billboard>maps)

 When i have convert my XML to YMAP, where i put it ?
- You put your exemple.YMAP in the folder [YOUR_YMAP_SAVE]. (es_billboard>stream>[YOUR_YMAP_SAVE])

 I have a billboard limit ?
- No , you can place 5 billboards or 200 on the map.

 I can place a billboard on city center and one on paleto on the same XML ?
- Yes , but separate by place to better find you there and that it is more optimized

 Can i create one XML for paleto , one XML for city center , one XML for sandyshore , etc...
- Yes , and it's better to create more YMAP , if one day you want edit the Paleto place , you just open your " paleto_work.xml" on es_billboard on game , edit it , and convert it again.
If you do a misstake it's more easy to edit/rework/restart one.

 I do it everything alone ?
-  No, if you create a new group in your cfg exemple : group.billboard, people who have this perm can use the /billboard and creat XML, that doesn't creat a conflict in game because only the creator can see what he do. When he have finish and save for exemple " my_work" , you can use /billboard and load " my_work " when you click on the Folder icon , you can check if the work is good. After you can convert the YMAP if you think is ok.
And about the Texture, you can send the PNG file to someone, he creat the new texture, send it to you, and you replace the texture yourself.

 That can be a TEAM Work ? 
- Yes , export the texture on PNG , send it to someone , someone admin can use the /billboard and place billboard , and you just convert the work and replace the texture on the library.



# CONVERT XML to YMAP ( handling takes less than 3 minutes )

What you need : 
- OpenIV ( download link : https://openiv.com/ )
- ME2YM ( download link : https://www.gta5-mods.com/tools/mapeditor-2-ymap-converter)

1) Find you XML save on es_billboard>maps
2) Copy past it on your ME2YM folder ( copy/past it because if you want OPEN ingame your XML work again and edit it)
3) Open ME2YM 
4) Click on File>Open ( search and open your XML )
5) click on File>Export (congrate , you have convert your XML on YMAP.XML , but you need one move to finish the convert)
6) put your YMAP.XML file on OPENIV on your MODS folder ( Don't forget to active ,the " Edit mode " , that finish the convert)
7) Put your new YMAP on the folder "YOUR-YMAP_SAVE" 

Congratulation, your convert XML to YMAP is finish, now your mapping is on the server , every player can see your work. ( When you map ingame , no one see the XML work , on you , you can work when the server is online , convert your XML later and put if before a reboot)



# Replace Texture ( handling takes less than 3 minutes )

What you need : 
- OpenIV ( download link : https://openiv.com/ )
- A software for edit the texture or create one. 

Before to start you need to know something : 
- The new texture with which you will replace need have the SAME NAME ! ( if the texture name is 5 , the name of your texture need to be 66 too) 
- The texture need to be the size 512x512 , or 1024x1024 or 2048x2048. You can replace a texture 1024x1024 with a 512x512 .
- The picture need to be a .PNG ( or a DDS if you know how that work )

1) Find the texture you need to edit on the folder texture library on esbilloard>stream>[TEXTURE]. ( exemple you want the texture 5 , find the library texture "billboard1to7" )
2) Put the library ( billboard1to7 for the exemple) on your OPENIV Mods Folder. ( Think to active " the Edit mode " if you want open and replace )
3) Open the library texture and find Your texture ( The 5 for the exemple ). If you want edit, it simple you can click right on the texture and " export it " on PNG.
4) Open the texture and edit it on your software. 
5) Save your edit work on PNG 
6) Return on the library and click right on the texture , and replace with the new.
7) Click on the Save on the bottom.
8) Put your library texture ( billboard1to7 for the exemple ) on esbilloard>stream>[TEXTURE] and replace the old library texture.

Congratulation, your replace texture is finish, you have now the texture on the billoard.



# Shortcut of es_billboard


- Undo
   - [K] 
- Delete Selection
   - [DELETE] 
- Duplicate
   - [C] 
- Move
   - [B] 
- Show a menu
   - [R] 
- Move object on Z axis
   - [N+] 
- Move object on Z axis
   - [N-] 

- Rotate object
   - [LeftCtrl] + [Up/Down/Left/Right] 
- increase speed
   - [LeftShift] 
- decrease speed
   - [LeftAlt] 


- Deplacement:
   - [W] [A] [S] [D] - [Z] [Q] [S] [D]

- Rotate:
   - [Q] [E] - [A] [E]

- Save quick : ( but take care)
   - [LeftCtrl] + [Space]

- Menu:
   - [1] or [&] - Camera Mode
   - [2] or [é] - Edit
   - [3] or ["] - Add Object
   - [4] or ['] - List
- Select all
   - [U] 