---
title: "RiiTag auf der Wii"
---

{% include toc title="Inhaltsverzeichnis" %}

Solltest du hinsichtlich dieses Tutorials Hilfe benötigen, trete bitte dem [RiiConnect24 Discord-Server](https://discord.gg/rc24) bei (empfohlen), oder kontaktiere uns [per E-Mail unter support@riiconnect24.net](mailto:support@riiconnect24.net).
{: .notice--info}

RiiTag ist ein anpassbarer und dynamischer Gamertag. Durch Teilen deines Gamertags (ein dynamisches Bild) kannst du deinen Freunden zeigen, was du gespielt hast! Du kannst es mit einem USB-Loader verbinden und es aktualisiert sich selbstständig. Du brauchst ein Discord-Konto, um mit der Benutzung von RiiTag anzufangen.

Du möchtest RiiTag gerne auf deiner Wii U installieren? Schaue dir [diese Anleitung](riitag-wiiu) an um zu erfahren, wie du RiiTag mit deinem Wii U-Menü verbindest.
{: .notice--info}

#### Voraussetzungen

* Ein Computer
* Einen Texteditor
* Einen USB-Loader

#### Anleitung

##### Abschnitt 1 - Einstieg

1. [Gehe auf die RiiTag-Website.](https://tag.rc24.xyz/)
2. Gehe auf `Log In` und melde dich mit deinem Discord-Konto an.
3. Ein Fenster wird auftauchen und dich fragen, ob du `RiiConnect24 Login` Zugriff auf Discord geben möchtest. Wähle `Autorisieren`.
4. Klicke auf dein Profil oben rechts auf dem Bildschirm, danach `Edit RiiTag` und passe anschließend deinen Tag nach Belieben an. Du kannst Hintergründe, Overlays, Flags, Nicknamen und Wii-Nummern hinzufügen. Klicke auf das grüne Speichersymbol in der Ecke, um deine Änderungen zu speichern.
5. Klicke auf dein Profil oben rechts auf dem Bildschirm und danach auf `Account`. Klicke auf `Copy` unter `RiiTag Private Key`. Dies ist nicht notwendig, wenn du den USB Loader GX verwendest, da sich der Schlüssel in einer heruntergeladenen Datei befindet.

Teile deinen RiiTag-Schlüssel mit niemandem! Falls du das tust, können andere deinen Tag missbrauchen.
{: .notice--warning}

##### Abschnitt 2 - Verbinden deines USB-Loaders

Die Schritte zur Verbindung von RiiTag mit deinem USB-Loader hängen von deinem verwendeten USB-Loader ab.

###### USB Loader GX

1. Öffne USB Loader GX auf deiner Wii.
2. Gehe auf `Einstellungen` > `Features` und schalte `Wiinnertag` ein. Wähle bei allen Fenstern, die auftauchen, `Ja` oder `OK`.
3. Stelle sicher, dass `Initialisiere Netzwerk` eingeschaltet ist.
4. Beende USB Loader GX.
5. Verbinde die SD-Karte bzw. das USB-Laufwerk mit deinen USB Loader GX-Daten mit deinem Computer.
6. Klicke auf dein Profil oben rechts auf dem Bildschirm und danach auf `Account`. Klicke auf `You can also download your Wiinnertag.xml.` wodurch die benötigte Datei heruntergeladen wird, welche für die Benutzung von RiiTag mit dem USB Loader GX benötigt wird.
7. Speichere die XML-Datei in den `/apps/usbloader_gx`-Ordner auf deiner SD-Karte oder deinem USB-Laufwerk und ersetze die vorhandene `Wiinnertag.xml`.
8. Du hast jetzt RiiTag eingerichtet. Du kannst jetzt ein beliebiges Spiel starten, um zu sehen, dass es korrekt funktioniert.

###### WiiFlow

1. Verbinde die SD-Karte bzw. das USB-Laufwerk mit deinen WiiFlow-Daten mit deinem Computer.
2. Öffne `/apps/wiiflow/wiiflow.ini` mit einem Texteditor. (Wenn du WiiFlow Lite verwendest, sollte der Pfad `wiiflow_lite` anstelle `wiiflow` lauten.)
3. Suche nach `gamercards` und ersetze die Zeile mit `gamercards=wiinnertag`.
4. Suche nach `wiinnertag_url` und ersetze die Zeile mit `wiinnertag_url=https://tag.rc24.xyz/wii?game={ID6}&key={KEY}`.
5. Suche nach `wiinnertag_key` und ersetze die Zeile mit `wiinnertag_key=<key>`, wobei du `<key>` mit dem Schlüssel ersetzt, den du dir in Abschnitt 1 notiert hast.
6. Suche nach `gamercards_enable` und ersetze die Zeile mit `gamercards_enable=yes`.
7. Speichere die bearbeitete `wiiflow.ini`-Datei.
8. Du hast jetzt RiiTag eingerichtet. Du kannst jetzt ein beliebiges Spiel starten, um zu sehen, dass es korrekt funktioniert.

###### Emulatoren

RiiTag unterstützt Dolphin, Citra, und Cemu. Du benötigst ein Discord-Konto, damit dies funktioniert.
{: .notice--info}

1. [Tritt dem RiiConnect24 Discord-Server bei](https://discord.gg/rc24), falls du es nicht schon getan hast.
2. Stelle sicher, dass du Discord Präsenz in den Emulator-Einstellungen aktivierst.
3. Stelle sicher, dass dein Discord-Client geöffnet ist (nicht der webbasierte Client, sondern die eigenständige Anwendung)
4. Spiele ein Spiel und RiiTag wird automatisch deinen Tag aktualisieren, sobald du das Spiel spielst.

Ein Discord-Bot wird verwendet, um deine Aktivität zu erkennen und deinen RiiTag entsprechend zu aktualisieren. Wenn du den Bot auf deinen Server einladen möchtest, [verwende diesen Link](https://discord.com/oauth2/authorize?client_id=596108891071447052&scope=bot).

###### Configurable USB Loader

Wir bieten keine Unterstützung für den Configurable USB Loader an, da er im Vergleich zu USB Loader GX und WiiFlow veraltet ist.
{: .notice--info}

Du kannst das `CfgLoaderConfigurator.exe`-Programm (nur für Windows) verwenden, anstelle die `config.txt`-Datei wie unten beschrieben zu editieren.
{: .notice--info}

1. Verbinde die SD-Karte oder das USB-Laufwerk welche die Configurable USB Loader-Daten enthält mit deinem Computer.
2. Öffne `/usb-loader/config.txt` mit einem Texteditor.
3. Ersetze die Zeile (oder füge sie hinzu) `gamercard_url` durch `gamercard_url = http://tag.rc24.xyz/wii?game={ID6}&key={KEY}`.
4. Ersetze die Zeile (oder füge sie hinzu) `gamercard_key` durch `gamercard_key = <key>`, und trage bei `<key>` den Schlüssel ein, welchen du dir in Abschnitt 1 notiert hast.
5. Speichere die modifizierte `config.txt`-Datei.
6. Du hast jetzt RiiTag eingerichtet. Du kannst jetzt ein beliebiges Spiel starten, um zu sehen, dass es korrekt funktioniert.

#### RiiTag-Kanal

Wir haben einen RiiTag-Kanal, den du auf deiner Wii installieren kannst. Wenn der Kanal gestartet ist, wird der Internet-Kanal geöffnet und deinen RiiTag anzeigen, was es einfach macht diesen zu sehen, wenn du deine Wii benutzt. Du musst den Internet-Kanal installiert haben, um RiiTag nutzen zu können.
{: .notice--info}

1. [Gehe auf die RiiTag-Website.](https://tag.rc24.xyz/)
2. Klicke auf `Log In` und melde dich mit deinem Discord-Konto an.
3. Ein Fenster wird auftauchen und dich fragen, ob du `RiiConnect24 Login` Zugriff auf Discord geben möchtest. Klicke auf `Authorize`.
4. Klicke auf dein Profil oben rechts auf dem Bildschirm und danach auf `Profile`. Klicke auf `RiiTag Channel` um die WAD herunterzuladen.
5. Lege die WAD auf deine SD-Karte oder dein USB-Laufwerk.
6. Installiere die WAD mit deinem bevorzugten WAD-Manager ([Wii Mod Lite](wiimodlite) wird empfohlen).
7. Stelle sicher, dass der Internet-Kanal installiert ist.
8. Der RiiTag-Kanal sollte jetzt in deinem Wii-Menü vorhanden sein.

[Entdecke RiiTag-RPC](https://github.com/RiiConnect24/RiiTag-RPC/releases/latest)<br> Jetzt wo du RiiTag eingerichtet hast, kannst du als nächstes RiiTag-RPC einrichten, um deinen Discord-Freunden zu zeigen, was du gerade auf der Wii spielst.
{: .notice--info}

[Fortfahren in der Seitennavigation](site-navigation)<br> Wir haben viele weitere Tutorials, welche dir gefallen könnten.
{: .notice--info}
