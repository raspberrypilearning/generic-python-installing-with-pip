`pip` or `pip3` is a command line tool for installing Python 3 modules.

The modules are in packages which are downloaded from the [Python Package Index](https://pypi.python.org/pypi) on the internet and installed on your computer automatically.

To install a module use the `pip3 install name_of_module` command, replacing *name_of_module* with the module you wish to install.

Following the instructions below for your operating system.

## Raspberry Pi

+ Open a terminal by clicking Menu, Accessories, Terminal.

+ Enter this command to install the module.

```bash
sudo pip3 install name_of_module
```

![pi pip install](images/pi_pip_install.gif)

## Windows

+ Open a command prompt by searching for *command prompt* and clicking on the app.

![windows command prompt](images/windows_command_prompt_app.PNG)

+ Enter this command to install the module.

```bash
pip3 install name_of_module
```

![windows pip install](images/windows_pip_install.gif)

If you experience problems, have a look at [Using pip on Windows](https://projects.raspberrypi.org/en/projects/using-pip-on-windows).

## Mac OS

## Linux

+ Open a terminal

+ Enter this command to install the module.

```bash
sudo pip3 install name_of_module
```

![linux pip install](images/linux_pip_install.gif)

## Other pip commands

Upgrade an already installed module.

```bash
pip3 install --upgrade name_of_module 
```

Uninstall a library.

```bash
pip3 uninstall name_of_module
```

List installed libraries.

```bash
pip3 list
```