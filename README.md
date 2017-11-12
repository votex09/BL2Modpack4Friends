Install instructions

- First off, you'll need FilterTool.  
	https://www.dropbox.com/sh/bva2028ban8u1hs/AAAwiSZmV3a7dn6yFdzuZkwoa?dl=0&preview=FilterTool.jar

	>It is java based, so you'll need java installed.  
	If you don't have java, https://java.com/en/download/


- Place the Jar in %Borderlands%/Binaries

	>%Borderlands% is where the game is installed.  
	eg. (C:/Program Files (x86)/Steam/steamapps/common/Borderlands 2)


- Open the Jar with Java.

	>On the first launch of the program a welcome message displays, outlining various features.  
	Click OK  
	A window then will appear where you can select actions to be performed, check all of them.
	Select the dropdown box and select "Tilde" for your console key, this is important.  
	You may optionally select F6 if you desire.


-	For the games you have selected to hex edit, if you did not install the tool to either of your Binaries folders.
	A window will open for you to select Borderlands2.exe and/or BorderlandsPreSequel.exe on your computer.

	>The actions you have selected will be completed through a series of windows.
	(Hexedit BL2 -> Hexedit TPS -> ConsoleKey BL2 -> ConsoleKey TPS)  
	Setting a key for the console allows it to be opened.
	Tilde on the QWERTY (Standard) Keyboard is left of 1 and above TAB.  
	Hex editing the games allows the console to be used for mods since it
	Removes the limitation that most commands will be said into chat.  
	Enables the set command to be used outside of offline mode.

- After the patch completes you can then close the program.
	>You should not ever need this program ever again unless your install gets messed up or you want to edit things.

- Installing the ModPack
	>Download all files from git.
	Place all files in

	%Borderlands2%/Binaries

	>Open the Win32 folder in Binaries, right click Borderlands2.exe and make a shortcut.  Right click this shortcut and click properties.
	In the shortcut tab, there is a field called "target"

	>In this field AT THE END of what is already there, add the following:

	-log -debug -codermode -nosplash -exec=phase.shft

	>Note that there is a space before each "-" including the first one.
	For example:

	"X:/SteamLibrary/steamapps/common/Borderlands 2/Binaries/Win32/Borderlands2.exe" -log -debug -codermode -nosplash -exec=phase.shft

	>This will launch the game with all needed arguments and auto-apply the regular patch (phase.shft)
	Optionally you may change phase.shft to insanity.shft for randomized grenades and relics. (insanity.shft)

	>Place this shortcut on your desktop, running the game through steam might have some bad side effects.
	This way is the most sure fire way of having your cake and eating it too.

- The Console

	>When the game is at the main menu, press ~ (grave/tilde) to open the console.  This is where you will be executing the patch data.
	Do not exec phase.shft/insanity.shft at the title screen (red borderlands logo) You will get a slew of errors and the patch will not work.

- IMPORTANT REMINDER
	>ALWAYS ALWAYS ALWAYS remember to exec phase.shft/insanity.shft when you return to the main menu.
	This rule should apply when changing characters, relogging, reloading areas for boss farming etc.

	>If you do NOT do this, you run the risk of having your character reset, skills and/or items will be removed.
	Please make backups often, the two .reg files that are supplied may aid you in doing that.

	%Documents%/My Games/Borderlands 2/WillowGame/SaveData

	>The above is where your character save data is stored. Sort by date to find your last played character.
	I also recommend turning off steam cloud save.  You do not want steam overriding your saves at the wrong moment, trust me.
