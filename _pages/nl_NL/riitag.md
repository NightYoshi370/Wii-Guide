---
title: "RiiTag on Wii"
---

{% include toc title="Table of Contents" %}

Als u hulp nodig heeft bij iets wat met deze tutorial te maken heeft, sluit u dan aan bij [de RiiConnect24 Discord server](https://discord.gg/b4Y7jfD) (aanbevolen) of [e-mail ons via support@riiconnect24.net](mailto:support@riiconnect24.net).
{: .notice--info}

RiiTag is a customizable and dynamic gamertag. By sharing your gamertag (a dynamic image), you can show what you've been playing to your friends! You connect it to a USB Loader, and the tag updates on-the-fly. You need a Discord account in order to start using RiiTag.

#### Benodigdheden

* Een Computer
* Een tekst bewerker
* Een USB Loader

#### Instructies

##### Deel I - Beginnen

1. [Ga naar de RiiTag website.](https://tag.rc24.xyz/)
2. Klik op `Log In` en log in met uw Discord account.
3. Een venster zal dan openen met de vraag of u `RiiConnect24 Login` wilt toestaan via Discord. Klik op `Authorize`.
4. Klik op`Edit Your Tag` u kunt de opties die hier te vinden zijn naar keuze invullen. U kunt een achtergrond, overlay, vlag, bijnaam, Wii nummer en zelfs toevoegen om deze te laten zien op uw tag (dit is niet nodig als u een USB loader gebruikt).
5. Klik op `Show Key` en kopieer deze cijfers (een key genoemd) ergens waar u makkelijk bij kunt. Dit is niet nodig als u USB Loader GX gebruikt want dan zal uw key een download baar bestand zijn.
6. Klik op `Submit` om uw veranderingen op te slaan.

Deel uw RiiTag key nooit met andere mensen! Als u dit wel doet kunnen met uw key misbruiken.
{: .notice--warning}

##### Deel II - Aan sluiten op een USB Loader

De stappen om RiiTag met uw USB Loader te connecten verschillen per USB Loader.

###### USB Loader GX

1. Laadt USB Loader GX op uw Wii.
2. Ga naar `Settings` > `Features` en zet `Wiinnertag` aan. Klik op `Yes` of `OK` als er dialogen vensters openen.
3. Check of `Initialize Network` aan staat, zo niet zet dit dan aan.
4. Verlaat USB Loader GX.
5. Stop uw SD-kaart of USB-stick / hardeschijf waar uw USB Loader GX data op staat in uw computer.
6. [Ga naar deze pagina.](https://tag.rc24.xyz/Wiinnertag.xml)
7. Op uw webbrowser, klik op uw rechtermuisknop en dan op `Opslaan als`.
8. Save the XML to `/apps/usbloader_gx`  folder on your SD Card or USB device, replacing the existing `Wiinnertag.xml`.
9. You have now set up RiiTag. You can try loading any game now to see if it works correctly.

###### WiiFlow

1. Take the SD Card or USB device where your WiiFlow data is into your computer.
2. Open `/apps/wiiflow/wiiflow.ini` with a text editor. (If you use WiiFlow Lite, the path might have `wiiflow_lite` instead of `wiiflow`.)
3. Search for `gamercards` and replace that line with `gamercards=wiinnertag`.
4. Search for `wiinnertag_url` and replace that line with `wiinnertag_url=http://tag.rc24.xyz/wii?game={ID6}&key={KEY}`.
5. Search for `wiinnertag_key` and replace that line with `wiinnertag_key=<key>`, replacing `<key>` with the key you wrote down in Section 1.
6. Search for `gamercards_enable` and replace that line with `gamercards_enable=yes`.
7. Save the modified `wiiflow.ini` file.
8. You have now set up RiiTag. You can try loading any game now to see if it works correctly.

###### Configurable USB Loader

We do not offer support for Configurable USB Loader, as we are focused on USB Loader GX and WiiFlow.
{: .notice--info}

You can use the `CfgLoaderConfigurator.exe` program (Windows only) instead of editing the `config.txt` file mentioned below if you want to.
{: .notice--info}

1. Take the SD Card or USB device where your Configurable USB Loader data is into your computer.
2. Open `/usb-loader/config.txt` with a text editor.
3. Replace (or add the line) starting with `gamercard_url` with `gamercard_url = http://tag.rc24.xyz/wii?game={ID6}&key={KEY}`.
4. Replace (or add the line) startin with `gamercard_key` with `gamercard_key = <key>`, replacing `<key>` with the key you wrote down in Section 1.
5. Save the modified `config.txt` file.
6. You have now set up RiiTag. You can try loading any game now to see if it works correctly.

[Continue to site navigation](site-navigation)<br> We have many other tutorials that you might like.
{: .notice--info}
