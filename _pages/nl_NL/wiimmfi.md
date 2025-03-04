---
title: "Wiimmfi"
---

{% include toc title="Inhoudsopgave" %}

If you need help for anything regarding this tutorial, please join [the RiiConnect24 Discord server](https://discord.gg/rc24) (recommended) or [e-mail us at support@riiconnect24.net](mailto:support@riiconnect24.net).
{: .notice--info}

![Wiimmfi Logo](/images/WiiWiimmfiLogo.jpg)

[Wiimmfi](https://wiimmfi.de) is a replacement service for the now-defunct Nintendo Wi-Fi Connection. It has been developed by Wiimm and Leseratte.

If you get the error 23904 while connecting to Wiimmfi, then you are using an outdated patch.<br> Follow the steps below for the method you're using to connect to Wiimmfi again.<br> See [this page](https://wiimmfi.de/update) for more details.<br>
{: .notice--waarschuwing}

## Different patchers

There are lots of different methods to connect to Wiimmfi. Choose the one that fits your needs best.

### Automatic patching from the Disc Channel using Priiloader

#### Benodigdheden
- A Wii with Priiloader 0.9 or later installed

If you have an older version of Priiloader or don't have it installed, follow [this guide](priiloader) to update/install it.
{: .notice--info}

#### Instructies
1. Hold reset while powering on your Wii (if using a Wii mini, plug in a USB keyboard and press escape).
2. Go to `System Menu Hacks`.
3. Make sure the `Wiimmfi patch v4` hack is enabled.
4. Instellingen opslaan en afsluiten.

If you see the hack `Wiimmfi patch v2` or `Wiimmfi patch v3` instead, then you do not have the latest version of the hacks_hash.ini file.<br> Download it from [here](https://github.com/DacoTaco/priiloader/raw/master/priiloader/hacks_hash.ini) and place it in `/apps/priiloader/hacks_hash.ini` on your SD card or USB drive.<br> Then, repeat the previous steps.
{: .notice--waarschuwing}

### Homebrew (Disc) Application
MrBean35000vr (creator of CTGP-R, a Mario Kart Wii content pack) created a Wiimmfi Disc Patcher that allows you to insert a disc and patch the game on-the-fly for Wiimmfi use, though this must be run every time you start the disc.

#### Benodigdheden
* Een SD-kaart of USB-stick/ harde schijf
* [Auto Wiimmfi Patcher](https://download.wiimmfi.de/patcher/autowiimmfipatcher-latest.zip)

#### Instructies

1. Extract Auto Wiimmfi Patcher to the root of your SD card or USB drive.
2. Insert your SD Card into your Wii, and launch Auto Wiimmfi Patcher from the Homebrew Channel.
3. Insert your game disc (you can insert it before or after launch, it doesn't matter).
4. Wait for patch to complete, and it'll begin!

### No-Homebrew (Disc)
Thanks to Fullmetal5's str2hax exploit, which Leseratte was able to adapt for the Wiimmfi patcher, you can run the Wiimmfi patch without having any homebrew on your Wii.

#### Benodigdheden
* Een Wii met een internet connectie

#### Instructies

1. Voer uw gameschijf in.
2. Go into your internet connection settings and set the DNS server of your console to 95.217.77.151.
3. Go to the WC24 contract information (third button after clicking on "Internet" in the settings).
4. Confirm that you do want to use WC24 and the shop channel
5. The Wiimmfi patcher page should show up. If it doesn't, and you still see the default license agreement, your router might not be compatible with this method.
6. Wait for about 1 minute and 30 seconds for the patcher to load
7. The game should now start with the Wiimmfi patch included

### Automatic patching using a USB Loader
If you are already using USB Loader GX, try updating it to the most recent version. Then, there should be a "private server" setting (both in the global loader options and in the game options) which you can set to "Wiimmfi" to make the USB Loader automatically patch every game you start to work with Wiimmfi.

### ISO Patching
You may not want to run a patcher each time you want to play on Wiimmfi, and maybe you already use a USB Loader. As such, ISO Patchers were created, some for specific games.

#### Benodigdheden
- Your copy of your game (WBFS, ISO, cISO, and other forms that a Wii can use are supported).
- [RiiConnect24 Patcher](https://github.com/RiiConnect24/RiiConnect24-Patcher/releases/) (Windows and Unix)  
  **or**
- [Wiimmfi Patcher (cross-platform)](https://download.wiimmfi.de/patcher/wiimmfi-patcher-latest.zip)
- A USB Loader, [cIOS](cios), and a USB to store the game on (you should already have these if you're using a USB Loader)

#### Instructies
1. Extract the patcher of your choice to a folder, and place your copy of the game in it.
2. Run the patch script for your OS: usually it will end in `.bat` for Windows and `.sh` for Mac/Linux. If you're using the RiiConnect24 Patcher, select your device (Wii, vWii, or Dolphin) and choose the patcher for your game.
3. Once it's finished, get the version out of the `wiimmfi-images` folder (it may be in the folder outside of the patcher - ../wiimmfi-images) and copy it back to your USB.

### WiiWare Patching
You can patch WiiWare games in order to play them on Wiimmfi.

#### Benodigdheden

- Een SD-kaart
- Your copy of your game (in WAD format)
- [RiiConnect24 Patcher](https://github.com/RiiConnect24/RiiConnect24-Patcher/releases/) (Windows and Unix)  
  **or**
- [WiiWare Patcher](https://github.com/RiiConnect24/WiiWare-Patcher/releases) (cross platform)
- [Wii Mod Lite](https://oscwii.org/library/app/WiiModLite)

[If you want to see how to use the WiiWare Patcher, click here!](wiiwarepatcher)
{: .notice--info}

Stappen:
1. Extract the .zip of the latest version of WiiWare Patcher, and put your WAD in it.
2. Run the patch script for your OS: usually it will end in `.bat` for Windows and `.sh` for Mac/Linux. If you're using the RiiConnect24 Patcher, select your device (Wii, vWii, or Dolphin) and choose the WiiWare patcher.
3. If it completed successfully, install the WAD that was made in `wiiware-wads` with Wii Mod Lite.

## Andere dingen

### Mario Kart Wii competities
Wiimmfi allows you to participate in Mario Kart Wii competitions again.

#### Benodigdheden

- Een SD-kaart of USB-stick/ harde schijf
- Mario Kart Wii Competition Patcher
   - [Wii](https://competitions.wiimmfi.de/competition-tool-wii.zip)
   - [Wii U (vWii)](https://competitions.wiimmfi.de/competition-tool-wiiu.zip)

#### Instructies (voor Wii)

1. Extract Mario Kart Wii Competition Patcher and put it in the `apps` folder on your SD Card.
2. Insert your SD card or USB drive into the Wii.
3. Launch the original Mario Kart Wii game (not Wiimmfi patched).
4. Navigate to Settings -> Network Settings (or Nintendo WFC Connection) -> Message Service. If you turned the message service feature on, turn it off and turn it on again.
5. Launch Mario Kart Wii Competition Patcher.
6. The patcher will look for save files for Mario Kart Wii on your storage device in various places, and upload them. This is done in case a missing competition is found in your save file. It will also, of course, patch your Wii for competitions.

If you're using the Wii U, you will have to run the competitions patcher whenever you want to check for a competition, because WiiConnect24 is not enabled on the Wii U.
{: .notice--info}

### DS Spellen
Wiimmfi doesn't only support Wii games, it supports lots of DS games too. Thanks to an exploit called nds-constraint, you can play DS games online without patching your games.

#### Benodigdheden

- A Wi-Fi network with WEP or no security

Getting a Wi-Fi network with WEP or no security is the hardest part, because DS games don't support newer Wi-Fi security types (unless it's one of the few games that are "DSi Enhanced" and can use your Wi-Fi configuration on your DSi or 3DS, like Pokémon Black/White). However, many routers support creating a guest Wi-Fi connection, or you can make a hotspot on your phone or your computer. There are plenty of resources on the Internet that have information on this, so use your favorite search engine to find them.
{: .notice--info}

#### Instructies

1. Go in the Nintendo DS Wi-Fi settings. This can be accessed inside the game you want to play online with.
2. Maak een verbinding.
3. Type in `167.86.108.126` as the primary DNS.
4. Type in `1.1.1.1` as the secondary DNS.
5. Save your connection settings and perform a connection test. If it's successful, then you're ready to play.

### Mario Kart Wii Mods

#### CTGP-R
MrBean35000vr and Chadderz have a custom track distribution called CTGP-R that allows you to use a set of custom tracks and has automatic Wiimmfi patching. Go to the [ChadSoft website](http://chadsoft.co.uk) for the download and instructions.

#### MKW Hack Pack
PhillyG has put together a collection of custom tracks and hacks called MKW Hack Pack, and allows connections to Wiimmfi. To learn how to set it up, go to the [wiki page](http://wiki.tockdom.com/wiki/MKW_Hack_Pack).

#### Wiimms Mario Kart Fun
Wiimm and Leseratte make a custom track distribution called "Wiimms MKW Fun", which gets updated about three times a year. It is based on the LE-CODE framework by Leseratte, has Wiimmfi support, and lots of other features. You can find out more about it on its [wiki page](http://wiki.tockdom.com/wiki/Wiimms_Mario_Kart_Fun).

[Ga door naar de sitenavigatie](site-navigation)<br> We hebben vele andere tutorials die u wellicht interessant vindt.
{: .notice--info}
