# Python-modules installeren met pip

`pip` of `pip3` is een opdrachtregelprogramma voor het installeren van Python 3-modules.

Modules kunnen worden gedownload als pakketten van de [Python Package Index](https://pypi.python.org/pypi) en automatisch op je computer worden geïnstalleerd.

Om een module te installeren, gebruik je de opdracht `pip3 install naam_van_module`, waarbij `naam_van_module` wordt vervangen door de module die je wilt installeren.

Volg de onderstaande instructies voor jouw besturingssysteem.

## Raspberry Pi

+ Open een terminalvenster door te klikken op **Menu** > **Accessoires** > **Terminal**.

+ Voer deze opdracht in om een module te installeren:

```bash
sudo pip3 install naam_van_module
```

![pi pip install](images/pi_pip_install.gif)

Als je problemen ervaart, kijk dan in onze gids [_Pip gebruiken op Raspberry Pi_](https://projects.raspberrypi.org/nl-NL/projects/using-pip-on-raspberry-pi).

## Windows

+ Open een opdrachtprompt door te klikken op **Start** > **Windows Systeem** > **Opdrachtprompt**, of door 'command' te typen in de zoekbalk van het startmenu.

![Windows-opdrachtprompt](images/windows_command_prompt_app.PNG)

+ Voer deze opdracht in om een module te installeren:

```bash
pip3 install naam_van_module
```

![Windows pip install](images/windows_pip_install.gif)

Als je problemen ondervindt, raadpleeg je onze gids [_Pip gebruiken op Windows_](https://projects.raspberrypi.org/nl-NL/projects/using-pip-on-windows).

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

## Troubleshooting installation issues

There is comprehensive documentation for pip at [pip.pypa.io](https://pip.pypa.io) which will help you with troubleshooting. Here are a few of the common issues, to help you identify problems.

**Installation issues**

If the installation of a package fails you may see an error message similar to these:

```bash
Could not find a version that satisfies the requirement <package-name (from versions: )>
```

```bash
No matching distribution found for <package-name>
```

The most common source of these errors is a misspelled package name.

You should also check that you are using the package name and not the module name. e.g. the package name for PIL (Python Imaging Library) is `pillow` and not `PIL`.

**Module import issues**

If the package installs but an error occurs when you try to import the module, check the following:

1. Which version of Python pip is installing packages into?

    If you have multiple versions of Python on your computer, pip might be installing modules for a different version than the one your program is using.

    It may be a case of using the right version of the pip command, make sure you are using `pip3`.

2. Is the package included in your package list?

    You can use the following command to list all the Python packages you have installed.

    ```bash
    pip3 list
    ```

## Upgrading a package

When you install a Python package that is already on your computer, it will not update it to the latest version.

Use this command to update a Python package to the latest version:

```bash
pip3 install --upgrade name_of_module 
```

## Uninstalling a package

Use this command to uninstall a Python package:

```bash
pip3 uninstall name_of_module
```
