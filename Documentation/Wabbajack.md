![image](../Resources/Banner.webp)

# Wabbajack Guide

## About Wabbajack and the fork

Wabbajack allows you to install my modpack to your PC by duplicating my setup directly to your PC, including each mod, setting, output etc. 
If you want to better understand the general idea of Wabbajack, refer to a Reddit article 
[_What Wabbajack is and Why You Should Care_](https://www.reddit.com/r/skyrimmods/comments/mbfk5f/what_wabbajack_is_and_why_you_should_care/).

If you would like to learn more general information about the fork, be sure to visit its home page again [here](https://www.nexusmods.com/skyrimspecialedition/mods/51973). 
I would very strongly recommend to check _Questions & Answers_ section for the most popular questions asked by users of the fork.

> **Warning**: Reading this guide is required for the modlist to work as intended. It will not work correctly if you do not get aqquainted and follow all the instructions.

---

## Requirements

In terms of performance, Dragon's Edition needs a bit more resources than its parent, but at the same time not as much as the most popular modlists for high-end PCs' users. Everything from good mid-end PC to high-end PC should run the modlist without any problems, so for GPU it will be a decent card with at least 6 GB VRAM (for example, according to one of the users, with Nvidia RTX 2060 they were able to get 57-60 stable FPS in Riverwood).

  - Fork's installation size - ~ 165 GB.
    - ~ 13 GB (not including CC content) is copied from your Skyrim's installation.
    - Should be put inside SSD to improve load times and prevent stutter.
  - Fork mods' size - ~ 98 GB.
    - Your downloads folder should be the same for all modlists to make the installation process faster and not to make you download the mods once again 
if you have them already.
    - Should be put inside HDD.
  
  - [The Microsoft Visual C++ Redistributable - Visual Studio 2015, 2017, 2019, and 2022 X64](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-160#visual-studio-2015-2017-2019-and-2022).
  - The latest version of Skyrim - 1.6.353. with the Anniversary Upgrade.
 
 > **Warning**: The Anniversary Upgrade isn't optional. Without it the modlist just won't install for you.

---

## Steam Setup

If you have successfully used any other official Wabbajack modlist for Skyrim Special Edition recently and if it uses [Game Stock folder system](https://github.com/wabbajack-tools/wabbajack/wiki/Keeping-The-Game-Folder-Clean-(via-local-game-installs)), which allows us to leave Skyrim completely untouched and this way more compatible with other modpacks, then you don't need to do the steps in this section.

### Steam Library Should Be Outside Windows Related Folders

The best location would be _C:\Steam_. Such location is also called _the root of the drive_. It can also be located in somewhere like _C:\Games\Steam_.

If you have your Steam library inside Windows related folder such as _Desktop, Program Files, Downloads, Documents, OneDrive_ etc., 
use a guide from [here](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) to put it outside of one of these folders.

### Start with Clean Skyrim

I highly recommend uninstalling the game through Steam, deleting the game folder and reinstalling it. You should also clean up the _Skyrim Special Edition_ folder inside _Documents/My Games/_ by deleting the contents inside.

### Set the Game's Language to English

Right click on your `The Elder Scrolls V: Skyrim Special Edition` game, select `Properties`, navigate to the `LANGUAGE` tab and select `English` from the dropdown menu.

### Change Game's Update Behaviour

Head over to the `Properties` again, navigate to the `UPDATES` tab and change _AUTOMATIC UPDATES_ parameter to `Only update this game when I launch it`. 

### Start Skyrim at Least Once

Start the game from Steam and and let it do the initial graphics check. Do not worry about this part as the installation will replace this graphics settings. Start the game and exit once you're in the main menu.

---

## Anniversary Upgrade

If you have successfully used Anniversary Update's Creation Club's (CC) mods for Skyrim Special Edition recently by yourself or by using any other official Wabbajack modlist, then you don't need to follow the next steps in this section.

1. If you haven't done that already, buy Anniversary Upgrade and make sure that Steam installed it.
2. If you don't have a Bethesda account, make it at [Bethesda.net](https://bethesda.net/en/dashboard).
3. Launch Skyrim through Steam.
4. Click the `Play` button.
5. Choose `Creation Club` option.
6. Login with your Bethesda.net credentials.
7. Click the `Download All` button.
8. Wait for Skyrim to finish.

---

## Installation

If you haven't installed Wabbajack yet, grab its latest release from [here](https://github.com/wabbajack-tools/wabbajack/releases), make a folder inside the root of the drive like _C:\Wabbajack_ and place the `Wabbajack.exe` file inside it. This folder must not be in the Windows related folders 
(_Desktop, Program Files, Downloads, Documents, OneDrive_ etc.).

The downloading and installation process can take a very long time, it depends on your system's specifications, your internet's speed and if you have Nexus premium membership.
> It will be way faster if you have one big mod folder for all modlists to make the installation process faster and not to make you download the mods once again 
if you have them already.

1. Open `Wabbajack.exe`.
2. Click on `Browse Modlists` and download `The Phoenix Flavour - Dragon's Edition` from the gallery.
3. Once the download is done, set the installation location again somewhere outside Windows related folders like _C:\Skyrim SE Modlists\The Phoenix Flavour - Dragon's Edition_ or _C:\The Phoenix Flavour - Dragon's Edition_. 
4. Point Wabbajack towards your download location. If you haven't downloaded any mods before, make a folder like _D:/Skyrim SE Mods_ or _D:\Skyrim\Mods_ and 
then point Wabbajack to it.
5. Click the `Play` button.
6. Wait for Wabbajack to finish.
7. If you run into any issues, simply retry the Wabbajack installation. If the installation still fails, 
ask for help in [TPF Discord server](https://discord.gg/m5kMrnHpwm)'s _#tpf-de-wabbajack-support_ channel. 
> To get to the channel, simply find _#role-settings_ channel in the server and choose my role, new channels then will appear in the server's list.
> You will need to upload your log file to the corresponding channel. 
You can find the relevant file (_Wabbajack.current.log_) inside the _logs_ folder within the latest version folder - this will be in the same location you saved _Wabbajack.exe_ to.

---

## Configurations

Now open the folder, where you have saved the modpack, and double-click on _ModOrganizer.exe_ file. You can see the full setup - the mod order is on the left, sorted below separators that may be collapsed by default, and the load order with all plugins on the right.

By default your game is capped at 60 FPS (to avoid any issues related to Skyrim's physics) and is borderless. Your resolution was automatically detected and changed by Wabbajack.

If you want to uncap your framerate (that is on you), do the following:

1. Press on `ESSENTIAL MODS` separator.
2. Double click on `SSE Display Tweaks` mod.
3. Choose `INI files` tab.
4. Press on `SKSE\Plugins\SSEDisplayTweaks.ini`.
5. In line 204, change _FramerateLimit_ parameter to your desired framerate after _=_ sign.
7. Press on `Save` button.

If you want to downscale your resolution, do the following:

1. Press on `ESSENTIAL MODS` separator.
2. Double click on `SSE Display Tweaks` mod.
3. Choose `INI files` tab.
4. Press on `SKSE\Plugins\SSEDisplayTweaks.ini`.
6. In line 58, change _BorderlessUpscale_ parameter to `True`.
7. In line 66, remove `#` sign before _Resolution_ parameter and then write down your monitor's native resolution after _=_ sign.
8. An optional step for those, who seek even more performance - in line 67, remove `#` sign before _ResolutionScale_ parameter and then write down your desired resolution scale after _=_ sign.
> I would recommend to try 0.9 at first as resolution scale below 0.9 can look a bit too blurry depending on your resolution.
9. Press on `Save` button.

If you want to change your field of view (FOV), do the following:

1. Press on `CONTROLS & CAMERA EXTENDED` separator.
2. Double click on `Improved Camera` mod.
3. Choose `INI files` tab.
4. Press on `SKSE\Plugins\ImprovedCameraSE\ImprovedCameraSE.ini`.
5. From line 182 to 203, change FOV parameters to your desired values.
6. Press on `Save` button.

<p>
    <img width="25%" src="https://user-images.githubusercontent.com/37147270/153157130-5fa2ffc8-8770-4b9a-8565-a0e564af2542.png" /> 
</p>

---

Some of the mods inside Mod Organizer are disabled by default in the modpack. Some of these are:
  - _Blade and Bunt - Vanilla Difficulty Modifiers_ under TPF's _DIFFICULTY MODIFIERS_ separator, because it makes the game easier and less interesting. If you find the combat of the game too difficult even after tweaking the game's difficulty, you are free to enable the mod by clicking on a rectangle right next to its name on the left side of MO2, but then you will also need to put its plugin right next after Blade and Blunt's plugin _BladeandBlunt.esp_ on the right side of MO2 by simply dragging it.
  > Here are also two already enabled modifiers for our dragon overhauling mod Dragon War, which greatly improves dragons by actually making them to be treated with cautiousness. In the original mod dragons have too much health, so it becomes a little bit too annoying to fight them and that's where these patches come handy nerfing their health and just a bit - their damage. If you want much longer fights with dragons, feel free to disable these two. 
  - All the mods under _WIDESCREEN SUPPORT_ separator, because obviosuly only a few have those huge monitors. If you are actually one of them, enable all the mods under this section and you are done.
> Do not touch any other disabled mods for now.

Finally we are ready to open and finish configuring the game. Above the load order (in the right pane), you can see the executables drop-down. Very likely _The Phoenix Flavour - Dragon's Edition_ was already selected here, so you can start the game by clicking _Run_.

---

## In-Game Adjustments

And now we are ready to jump into the game.

There are some charcter presets available for your walkthrough. To use them, choose `Presets` option in the top right side of the character creation menu,
then press `F9` button to load available presets and then choose the desired one according to the race and the gender you have choosen for the character.

If you want to make your character on your own, at first we need to activate our character's high poly head (much more detailed head than the vanilla one, 
which you can also shape in much more ways) in character creation menu and then our hair, brows (and/or scars, beard) will look excellent on us.

<p align="center">
    <img width="50%" src="https://user-images.githubusercontent.com/37147270/151776057-aaa74ddf-396d-4bc4-9c83-18be28950be6.png" /> 
</p>

Then customize your character to your heart's content (while being reasonable). Hair with physics for women are obtainable by choosing hair with _KSHairdosSMP.esp_ near their name.
<p align="center">
    <img width="75%" src="https://user-images.githubusercontent.com/37147270/151706652-f8f91309-203f-4b10-a975-8be565db54fd.png" /> 
</p>
If you want to use hair with physics for men, you will find instructions on how to get them a bit later. For better results with those, equip bald hair style now.

---

After you get control over movements of your character, don’t go anywhere right away. 
It will be awesome if you wait for a pop-up about finishing things setting up to appear before doing anything else.
Don't be scared if you saw parts of your body during the movement (and/or after you finished creating your character), that will go away, when you will regain full control of your character.

After talking with Ralof or Hadvar, you can turn on the following mods to decide if you would want to use them. They affect just the visual side of the game. 
If you aren't a fan, just press the same button once again to turn them off. 

* **Look What You See** - Press your `V` key to toggle headtracking in the third person view.
* **Improved Camera** - Use your `F` key to toggle between the first and the third person view.
* **Toggle Compass Hotkey** - Tap `X` key to toggle visibility of your compass.
* **Equipment Toggle** - Press `Arrow Down` button to toggle your heagear's visibility.

Some quick tips before the end:

* **About the option to remove your tail** - It is weird, but you will actually need to equip another tail to get rid from... "them both". To get the tail, open your inventory and in misc item section find an item called `AddItemMenu` and click on it. Another menu with 4 items will pop up. Grab an item with a search option. Then open your inventory and use the item with the search option. Type `tail` in AddItemMenu's searcher. Choose the mod's plugin and grab your tail. Then equip it like gear and your tail will be gone.
* **About hair with physics for men** - You will need to use AddItemMenu again, but this time type the word `hair`.
* **About ENB** - `F10` button toggles the ENB effect, `F11` opens the ENB GUI, `F7` toggles an FPS counter. Feel free to make screenshots with Steam by using `F12`.
> If the ENB isn't for you and you want to change it, delete modpack's _enbseries_ folder and _enbseries.ini_ file from the fork's _Stock Game_ folder and replace with the ones from your desired ENB.
* **About fast travelling** - By default fast travel is disabled, because it becomes much more interesting that way (you travel and discover much more) and there are plenty of ways to travel around - as in vanilla (horses, carriages, boats), paragliding, spells and another mean, which is tied to a quest (don't want to spoil that). If you still aren't sold, feel free to reenable it by disabling _Disable Fast Travel SKSE - No Janky Map UI_ mod under the _INTERFACE EXTENDED_ separator.

---

> **Warning**: Very important information!

_Note_ in the Bannered Mare can be activated **only** after 5 in-game days after you have finished the main quest _Unbound_.

Also a reminder that the modlist uses a mod called _End Times_, which will **end the game** if don't finish the main quest line in **14 real life days, that means 336 real life hours**. That should be enough to do many other things in between saving the world for the first time. 
And don't worry - **the game won't end if you finish the main quest**. You can always enter into MCM again to see how much time you have left. Be sure to remember.

---

## Thank You

And that's it! You are ready for the action.

If you have any questions following these instructions, something doesn't allow you to finish the setup (but before that you have actually checked you have all the requirements for the fork) or if you find a typo or any other mistake in the documentation, 
feel free to report in [TPF Discord server](https://discord.gg/m5kMrnHpwm)'s _#tpf-de-wabbajack-support_ channel. 
If you have experienced a bug during your walkthrough, jump in [*Reporting Bugs*](https://github.com/DragonBlame/tpf-dragons-edition/blob/main/BUGS.md) section first.
> To get to these support channels, simply find _#role-settings_ channel in the server and tick my role, new channels then will appear in the server's list.

If you want to learn more about what the modpack offers and what actually many of the mods do, check my [gameplay guide](https://github.com/DragonBlame/tpf-dragons-edition/blob/main/GAMEPLAY.md). 

If you would like to make any recommendations after looking into what the modlist has to offer or to give me an advice, 
please use _Posts_ feature on Nexus or use _#tpf-de-feedback_ channel on TPF's Discord server. Again to get to the channel, simply find _#role-settings_ channel and tick my role at the end, new channels then will appear in the server's list. Suggestions on how to improve the documentation are also welcome on GitHub.
Before asking additional questions be sure to check the gameplay guide mentioned before and the _Questions & Answers_ section on Nexus.

If you want to help me, don't forget to endorse the fork’s page on Nexus and write something positive for me to read (I am happy to hear from people in Discord too). 
If you want to help even more, you can donate by pressing the button right below. 

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/H2H6ABHYO)

I will post about updates for the modpack in both TPF's and Wabbajack's Discord servers.

If you just want to chat, share your beautiful screenshots, builds or performance parameters, I am still happy to see you around on Nexus and in Discord. :)
