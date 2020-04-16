# Python-modules installeren met pip

`pip` of `pip3` is een opdrachtregelprogramma voor het installeren van Python 3-modules.

Modules kunnen worden gedownload als pakketten van de [Python Package Index](https://pypi.python.org/pypi) en automatisch op je computer worden geïnstalleerd.

Om een module te installeren, gebruik je de opdracht `pip3 install naam_van_module`, waarbij `naam_van_module` wordt vervangen door de module die u wilt installeren.

Volg de onderstaande instructies voor jouw besturingssysteem.

## Raspberry Pi

+ Open een terminalvenster door te klikken op **Menu** > **Accessoires** > **Terminal**.

+ Voer deze opdracht in om een module te installeren:

```bash
sudo pip3 install naam_van_module
```

![pi pip install](images/pi_pip_install.gif)

Als je problemen ervaart, kijk dan in onze gids [_Pip gebruiken op Raspberry Pi_](https://projects.raspberrypi.org/en/projects/using-pip-on-raspberry-pi).

## Windows

+ Open een opdrachtprompt door te klikken op **Start** > **Windows Systeem** > **Opdrachtprompt**, of door 'command' te typen in de zoekbalk van het startmenu.

![Windows-opdrachtprompt](images/windows_command_prompt_app.PNG)

+ Voer deze opdracht in om een module te installeren:

```bash
pip3 install naam_van_module
```

![Windows pip install](images/windows_pip_install.gif)

Als je problemen ondervindt, raadpleeg je onze gids [_Pip gebruiken op Windows_](https://projects.raspberrypi.org/en/projects/using-pip-on-windows).

## macOS

+ Open een terminalvenster door op **Toepassingen** > **Hulpprogramma's** > **Terminal** te klikken of door 'terminal' in de zoekbalk van het bureaublad te typen.

+ Voer deze opdracht in om een module te installeren:

```bash
pip3 install naam_van_module
```

![mac pip-installatie](images/mac_pip_install.gif)

## Linux

+ Open een terminalvenster.

+ Voer deze opdracht in om een module te installeren:

```bash
sudo pip3 install naam_van_module
```

![Linux pip installatie](images/linux_pip_install.gif)

## Andere pip-opdrachten

Er is uitgebreide documentatie voor pip op [pip.pypa.io](https://pip.pypa.io); hier zijn een paar handige opdrachten:

+ Upgrade een reeds geïnstalleerde module:

```bash
pip3 install --upgrade naam_van_module 
```

+ Een module verwijderen:

```bash
pip3 uninstall naam_van_module
```

+ Lijst van geïnstalleerde modules:

```bash
pip3 list
```
