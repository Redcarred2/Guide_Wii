---
title: "Wilbrand"
---

{% include toc title="Índice" %}

Wilbrand, like LetterBomb, is an exploit for the Wii that is triggered using the Wii Message Board.

Unlike LetterBomb, Wilbrand supports Wii menu versions down to 3.0.
{: .notice--info}

There are two methods listed on this page used to create the proper Wilbrand exploit. Wilbrand Web is recommended for its ease of use.
{: .notice--info}

### Wilbrand Web (Recommended)

#### Requisitos

* An SD card formatted to FAT32/MS-DOS (FAT)
* A Wii on at least version 3.0

SD cards larger than 2GB will not work on Wii menu versions before 4.0.
{: .notice--warning}

#### Instrucciones

1. Enciende la consola.
1. Ve a la `Configuración de Wii`.
1. Take note of the letter next to the system version, in the top-right corner of the screen.
    + Esta letra corresponde a la región del menú de tu consola, que necesitarás saber para los pasos pertinentes.

    ![](/images/wii/SystemMenuVersion.png)

1. Navigate to `Internet` > `Console Information`.
1. Take note of your FULL MAC address.

    ![](/images/wii/MacAddress.png)

1. On your computer, open the browser and go to [wilbrand.donut.eu.org](https://wilbrand.donut.eu.org/).
1. Input your Wii MAC, version and region.
1. Ensure `Bundle the HackMii Installer for me!` is checked.
1. Cut either wire.

    ![](/images/exploits/wilbrand/web.png)

1. Click on "Download your .zip".
1. Inserta tu tarjeta SD en tu ordenador.
1. Copy the `private` folder and the `boot.elf` file from the downloaded `.zip` file to the root of your SD card.
1. Reinsert your SD card into your console.
    + The SD card must be inserted in the SD card slot located in the front of the Wii. Using a USB to SD adapter plugged into the Wii's USB port will not work.
1. On your Wii, return to the Wii Menu.
1. Launch the Wii Message Board on your Wii.
1. Open the green letter with a bomb.
    + Ensure the date on your Wii is correct, or you might be unable to find the letter.
    + In some cases, you may need to check the messages for tommorow or yesterday for the letter to show up.
    + If you don't see the green letter, check if any errors appear in the SD card section of `Data Management`. If there are errors, there may be an issue with the SD card format or the Wii’s SD card reader.

    ![](/images/exploits/wilbrand/msgboard.png)

1. Si el exploit ha tenido éxito, tu dispositivo habrá ejecutado el instalador de HackMii.
    + If this didn't work for you, try [Wilbrand CLI](#wilbrand-cli) or [try another exploit](get-started) (ie. Letterbomb).

[Continue to Homebrew Channel and BootMii Installation](hbc)
{: .notice--info}

### Wilbrand CLI

#### Requisitos

* A computer running Windows, macOS or Linux
* An SD card formatted to FAT32/MS-DOS (FAT)
* A Wii on version 3.0 or newer
* [Wilbrand](https://static.wiidatabase.de/Wilbrand.zip)
* [Instalador de HackMii v1.2](https://bootmii.org/download/)

SD cards larger than 2GB will not work on Wii menu versions before 4.0.
{: .notice--warning}

#### Instrucciones

1. Enciende la consola.
1. Ve a la `Configuración de Wii`.
1. Take note of the letter next to the system version, in the top-right corner of the screen.
    + Esta letra corresponde a la región del menú de tu consola, que necesitarás saber para los pasos pertinentes.

    ![](/images/wii/SystemMenuVersion.png)

1. Navigate to `Internet` > `Console Information`.
1. Take note of your FULL MAC address.

    ![](/images/wii/MacAddress.png)

1. Copy all files from the Wilbrand `.zip` to a folder on your computer
1. Inserta tu tarjeta SD en tu ordenador.
1. Open a terminal inside the folder Wilbrand was extracted to.
1. Using your Wii's version and MAC address, run the following command:

    + Windows: `.\Wilbrand.exe AA-BB-CC-DD-EE-FF MM/DD/YYYY VERSION X:`
        + `X:` is the drive letter of your SD card.

        ![](/images/exploits/wilbrand/windows.png)

    + Linux/macOS: `./Wilbrand AA-BB-CC-DD-EE-FF MM/DD/YYYY VERSION /media/mount_dir`
        + If you have not opened your terminal directly in the folder Wilbrand was extracted to, use `cd` to enter it first, eg. `cd ~/Desktop/Wilbrand`
        + `/media/mount_dir` is the folder your SD card is mounted in. This may vary depending on your Linux distro.

        ![](/images/exploits/wilbrand/linux.png)

1. Copy all files from the hackmii_installer_v1.2 `.zip` to a folder on your computer.
1. Copy `boot.elf` from the hackmii_installer_v1.2 `.zip` to the root of your SD card.
1. Reinsert your SD card into your console.
    + The SD card must be inserted in the SD card slot located in the front of the Wii. Using a USB to SD adapter plugged into the Wii's USB port will not work.
1. On your Wii, return to the Wii Menu.
1. Launch the Wii Message Board.
1. Open the green letter with a bomb.
    + Ensure the date on your Wii is correct, or you might be unable to find the letter.
    + In some cases, you may need to check the messages for tommorow or yesterday for the letter to show up.
    + If you don't see the green letter, check if any errors appear in the SD card section of `Data Management`. If there are errors, there may be an issue with the SD card format or the Wii’s SD card reader.

    ![](/images/exploits/wilbrand/msgboard.png)

1. Si el exploit ha tenido éxito, tu dispositivo habrá ejecutado el instalador de HackMii.

[Continue to Homebrew Channel and BootMii Installation](hbc)
{: .notice--info}
