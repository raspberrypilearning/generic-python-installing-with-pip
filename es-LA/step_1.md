# Instalar módulos Python con pip

`pip` o `pip3` es la herramienta de línea de comandos para instalar módulos de Python 3.

Los módulos se pueden descargar como paquetes desde el [Índice de paquetes de Python](https://pypi.python.org/pypi) e instalar en el computador de manera automática.

Para instalar un módulo, usa el comando `pip3 install name_of_module`, al reemplazar el `nombre_de_módulo` con el módulo que deseas instalar.

Sigue las siguientes instrucciones para el sistema operativo.

## Raspberry Pi

+ Abra una ventana de terminal haciendo clic en **Menú** > **Accesorios** > **Terminal**.

+ Escribe este comando para instalar el módulo:

```bash
sudo pip3 install name_of_module
```

![Instalación de pi pip](images/pi_pip_install.gif)

Si tienes problemas, echa un vistazo a nuestra guía [_Usar pip en Raspberry Pi_](https://projects.raspberrypi.org/en/projects/using-pip-on-raspberry-pi).

## Windows

+ Abra un símbolo del sistema haciendo clic en **Inicio** > **Sistema Windows** > **Símbolo del sistema**o escribiendo "comando" en la barra de búsqueda del menú de inicio.

![símbolo del sistema de windows](images/windows_command_prompt_app.PNG)

+ Escribe este comando para instalar el módulo:

```bash
pip3 install name_of_module
```

![Instalación de pip de windows](images/windows_pip_install.gif)

Si tienes problemas, consulta nuestra guía [_Usar pip en Windows_](https://projects.raspberrypi.org/en/projects/using-pip-on-windows).

## macOS

+ Abra una ventana de terminal haciendo clic en **Aplicaciones** > **Utilidades** > **Terminal**, o escribiendo 'terminal' en la barra de búsqueda del escritorio.

+ Escribe este comando para instalar el módulo:

```bash
pip3 install name_of_module
```

![Instalación de mac pip](images/mac_pip_install.gif)

## Linux

+ Abra una ventana de terminal.

+ Escribe este comando para instalar el módulo:

```bash
sudo pip3 install name_of_module
```

![Instalación de Linux pip](images/linux_pip_install.gif)

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
