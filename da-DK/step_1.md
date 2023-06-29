# Installer Python moduler med pip

`pip` eller `pip3` er en kommandolinje værktøj til at installere Python 3 moduler.

Moduler kan hentes som pakker fra [Python Package Index](https://pypi.python.org/pypi) og installeres på din computer automatisk.

For at installere et modul, brug `pip3 install navnet_på_modulet` kommandoen, hvor du erstatter `navnet_på_modulet` med det modul du vil installere.

Følg instrukser nedunder som svarer til dit operativ system.

## Raspberry Pi

+ Åben en terminal vindue ved at trykke **Menu** > **Accessories** > **Terminal**.

+ Brug denne kommando til at installere et modul:

```bash
sudo pip3 install navnet_på_modulet
```

![pi pip install](images/pi_pip_install.gif)

Hvis du har problemer, så kig på denne guide [_Using pip on Raspberry Pi_](https://projects.raspberrypi.org/en/projects/using-pip-on-raspberry-pi).

## Windows

+ Åben en kommandoprompt ved at trykke på **Start** > **Windows System** > **Command Prompt**, eller ved at skrive 'kommando' i start menuen's søgefelt.

![windows command prompt](images/windows_command_prompt_app.PNG)

+ Skriv denne kommando for at installere et modul:

```bash
pip3 install navnet_på_modulet
```

![windows pip install](images/windows_pip_install.gif)

Hvis du har problemer så kig på denne guide [_Using pip on Windows_](https://projects.raspberrypi.org/en/projects/using-pip-on-windows).

## macOS

+ Åben en terminal ved at trykke på **Applications** > **Utilities** > **Terminal**, eller ved at skrive 'terminal' i skrivebordets søgefelt.

+ Skriv denne kommando for at installere et modul:

```bash
pip3 install navnet_på_modulet
```

![mac pip install](images/mac_pip_install.gif)

## Linux

+ Åben et terminalvindue

+ Skriv denne kommando for at installere et modul:

```bash
sudo pip3 install navnet_på_modulet
```

![linux pip install](images/linux_pip_install.gif)

## Fejlfinding i installeringsproblemer

Der er omfattende dokumentation for pip på [pip.pypa.io](https://pip.pypa.io) hvilket vil hjælpe dig med at fejlfinde. Her er et par almindelige problemer der kan hjælpe dig.

**Installations problemer**

Hvis installationen af en pakke fejler kan det være du ser en fejlbesked der ligner en af disse:

```bash
Could not find a version that satisfies the requirement <package-name (from versions: )>
```

```bash
No matching distribution found for <package-name>
```

Den mest almindelige fejlkilde er et pakkenavn der er stavet forkert.

Du burde også tjekke om du bruger pakke anvnet og ikke modulnavnet. F.eks. er pakkenavnet for PIL (Python Imaging Library) faktisk `pillow` og ikke `PIL`.

**Modul import problemer**

Hvis pakken installerer men en fejl forekommer når du prøver at importere modulet, så tjek følgende:

1. Hvilken version af Python pip installeres pakkerne ind i?

    Hvis du har flere versioner af Python på din computer, kan det være pip installerer modulerne ind til en anden version af Python end det program du bruger.

    Det kan være du ikke bruger den rigtige version af pip. Vær sikker på at du bruger `pip3`.

2. Er pakken inkluderet i din pakkeliste?

    Du kan bruge følgende kommando til at liste alle Python pakker du har installeret.

    ```bash
    pip3 list
    ```

## Opgradering af en pakke

Når du installerer en Python pakke der allerede er på din computer, så vil den ikke automatisk opdatere til seneste version.

Brug denne kommando til at opdatere en Python pakke til den seneste version:

```bash
pip3 install --upgrade navnet_på_modulet
```

## Afinstallering af en pakke

Brug denne kommando til at afinstallere en Python pakke:

```bash
pip3 uninstall navnet_på_modulet
```
