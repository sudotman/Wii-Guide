---
title: "cIOS"
---

{% include toc title="Table of Contents" %}

Acest tutorial îți va arăta cum să instalezi cIOS (IOS personalizat). Acesta este necesar dacă vrei să încarci jocuri printr-un USB Loader. Unele aplicații homebrew s-ar putea să funcționeze mai bine folosind cIOS.

![d2x cIOS Installer](/images/cios/cIOS.png)

Dacă ai un Wii U (vWii), urmează [acest ghid](https://wiiu.hacks.guide/#/vwii-modding) în schimb pentru a instala cIOS. Orice alt cIOS nu va merge instalat pe vWii.
{: .notice--info}

Dacă ai un Wii mini, instalează [acest cIOS](cios-mini) în schimb. Orice alt cIOS nu va merge instalat pe Wii mini.
{: .notice--info}

#### De ce ai nevoie

- Un Wii
- Un card SD sau o unitate USB
- [d2x cIOS Installer](https://hbb1.oscwii.org/hbb/d2x-cios-installer/d2x-cios-installer.zip)

Asigură-te că dacă folosești un card SD, comutatorul de blocare este în poziția deblocată, altfel nu vei putea să selectezi opțiunile corecte în instalator
{: .notice--warning}

#### Instrucțiuni

<button class="tablinks btn btn--large btn--primary" id="defaultOpen" onclick="openTab(event, 'with-connection')">Cu o conexiune de Internet la consola Wii</button>
<button class="tablinks btn btn--large btn--info" onclick="openTab(event, 'without-connection')">Fără o conexiune de Internet la consola Wii</button>

<div id="with-connection" class="blanktabcontent" markdown="1">

##### Secțiunea I - Descărcare

1. Descarcă d2x cIOS Installer și extrage-l în rădăcina cardului tău SD sau unității tale USB.
1. Introduce cardul tău SD sau unitatea ta USB în Wii, și pornește d2x cIOS Installer din Homebrew Channel.
</div>
<div id="without-connection" class="blanktabcontent" markdown="1">

##### Secțiunea I - Descărcare

1. Descarcă, extrage și deschide [NUS Downloader](https://github.com/WiiDatabase/nusdownloader/releases/latest/download/NUSD-Mod-NUS-Fix.zip).
1. Alege "Database", "IOS", apoi "IOS57" și alege "v5918".
   - Asigură-te că "Pack WAD" este bifat și că "Patch IOS" nu este bifat.
1. Repetă pasul anterior pentru IOS56 v5661 și IOS38 v4123.
1. Odată ce ai descărcat toate cele trei IOS-uri, va exista un dosar numit `titles` în același dosar cu NUS Downloader. Deschide dosarul și navighează prin el până când găsești cele trei fișiere WAD pe care le-ai descărcat. Pune fiecare fișier WAD în rădăcina cardului tău SD sau unității tale USB.
1. Descarcă d2x cIOS Installer și extrage-l în rădăcina cardului tău SD sau unității tale USB.
1. Introduce cardul tău SD sau unitatea ta USB în Wii, și pornește d2x cIOS Installer din Homebrew Channel.
</div>

##### Secțiunea II - Instalare

1. Apasă continue, apoi setează opțiunile la următoarele:

```
Select cIOS: v10 beta52 d2x-v10-beta52
Select cIOS base: 57
Select cIOS slot: 249
Select cIOS version: 65535
```

![Install cIOS 249](/images/cios/Install249.png)

1. Odată setat, apasă A de două ori pentru a instala.
1. Când instalarea este gata, apasă A pentru a te întoarce, și setează opțiunile la următoarele:

```
Select cIOS: v10 beta52 d2x-v10-beta52
Select cIOS base: 56
Select cIOS slot: 250
Select cIOS version: 65535
```

![Install cIOS 250](/images/cios/Install250.png)

1. Odată setat, apasă A de două ori pentru a instala.
1. Când instalarea este gata, apasă A pentru a te întoarce, și setează opțiunile la următoarele:

```
Select cIOS: v10 beta52 d2x-v10-beta52
Select cIOS base: 38
Select cIOS slot: 251
Select cIOS version: 65535
```

![Install cIOS 251](/images/cios/Install251.png)

1. Odată ce este gata, apasă A de două ori din nou pentru a instala, apoi ieși după ce se termină.

#### Depanare

{% capture bruh %}
Deși majoritatea jocurilor ar trebui să meargă direct cu implicitele, unele s-ar putea să necesite folosirea unui cIOS specific pentru a merge, sau să utilizeze anumite funcții din joc.<br> Exemple includ:

- Folosirea unei tastaturi în Animal Crossing: City Folk.
- Rularea jocului SpongeBob's Boating Bash.

O lista vastă (deși incompletă) poate fi găsita [**aici**](https://wiki.gbatemp.net/wiki/Wii_cIOS_base_Compatibility_List)<br> Pentru a schimba cIOS-ul folosit pentru un joc specific, urmărește aceste instrucțiuni:
{% endcapture %}

<div class="notice--warning">{{ bruh | markdownify }}</div>

<button class="tablinks btn btn--large btn--primary" id="defaultOpen" onclick="openTab(event, 'usbloadergx')">USB Loader GX</button>
<button class="tablinks btn btn--large btn--info" onclick="openTab(event, 'wiiflow')">WiiFlow</button>

<div id="usbloadergx" class="blanktabcontent" markdown="1">
1. Alege jocul care nu merge.
1. Apasă pe Settings.
1. Alege `Game Load`.
1. Derulează jos la `Game IOS`.
1. Introduce slotul IOS pe care vrei să-l folosești.
    - Încearcă să folosești 250 sau 251, dacă 249 nu merge.
1. Apasă ok și încearcă să rulezi jocul.
</div>
<div id="wiiflow" class="blanktabcontent" markdown="1">
1. Alege jocul care nu merge.
1. Apasă iconița cu rotița.
1. Du-te la cIOS și folosește săgețile pentru a selecta slotul IOS pe care vrei să-l folosești.
    - Încearcă să folosești 250 sau 251, dacă 249 nu merge.
1. Apasă Save și încearcă să rulezi jocul.
</div>
##### Opțiuni după finalizare

[Continuă la Homebrew Browser](hbb)<br> Homebrew Browser este un loc bun de unde să-ți faci rost de aplicații homebrew pe consola ta Wii. Acesta este opțional de instalat.
{: .notice--info}

[Continuă la navigarea site-ului](site-navigation)<br> Avem multe alte tutoriale care s-ar putea să-ți placă.
{: .notice--info}

Acum poți folosi homebrew precum [USB Loader GX](usbloadergx) și [Wiiflow](wiiflow).
{: .notice--info}

<script>
    let tabcontent = document.getElementsByClassName("blanktabcontent");
    let tablinks = document.getElementsByClassName("tablinks");

    function openTab(evt, tabName) {
        let element;

        for (element of tabcontent) {
            element.style.display = "none";
        }

        for (element of tablinks) {
            element.className = element.className.replace("btn--primary", "btn--info");
            if (!element.className.includes('btn--info'))
                element.className += " btn--info";
        }

        document.getElementById(tabName).style.display = "block";
        evt.currentTarget.className = evt.currentTarget.className.replace("btn--info", "btn--primary");
    }

    // Get the element with id="defaultOpen" and click on it
    document.getElementById("defaultOpen").click();
</script>
