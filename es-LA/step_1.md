# Instalación de módulos de Python con pip

`pip` o `pip3` es una herramienta de línea de comandos para instalar módulos de Python 3.

Los módulos se pueden descargar como paquetes desde el [índice de paquetes de Python](https://pypi.python.org/pypi) e instalarse en tu computadora automáticamente.

Para instalar un módulo, usa el comando `pip3 install nombre_de_módulo`, reemplazando `nombre_de_módulo` con el módulo que quieres instalar.

Sigue las instrucciones a continuación que correspondan a tu sistema operativo.

## Raspberry Pi

+ Abre una ventana de terminal haciendo clic en **Menú** > **Accesorios** > **Terminal**.

+ Introduce este comando para instalar un módulo:

```bash
sudo pip3 install nombre_de_módulo
```

![instalación de pip en Pi](images/pi_pip_install.gif)

Si tienes problemas, echa un vistazo a nuestra guía [_Usar pip en Raspberry Pi_](https://projects.raspberrypi.org/es-LA/projects/using-pip-on-raspberry-pi).

## Windows

+ Abre un símbolo del sistema haciendo clic en **Inicio** > **Sistema de Windows** > **Símbolo del Sistema**, o escribiendo 'comando' en la barra de búsqueda del menú de inicio.

![símbolo del sistema de Windows](images/windows_command_prompt_app.PNG)

+ Introduce este comando para instalar un módulo:

```bash
pip3 install nombre_de_módulo
```

![Instalación de pip en Windows](images/windows_pip_install.gif)

Si tienes problemas, echa un vistazo a nuestra guía [_Usar pip en Windows_](https://projects.raspberrypi.org/es-LA/projects/using-pip-on-windows).

## MacOS

+ Abre una ventana de terminal haciendo clic en **Aplicaciones** > **Utilidades** > **Terminal**, o escribiendo 'terminal' en la barra de búsqueda del escritorio.

+ Introduce este comando para instalar un módulo:

```bash
pip3 install nombre_de_módulo
```

![instalación de pip en Mac](images/mac_pip_install.gif)

## Linux

+ Abre una ventana de terminal.

+ Introduce este comando para instalar un módulo:

```bash
sudo pip3 install nombre_de_módulo
```

![Instalación de pip en Linux](images/linux_pip_install.gif)

## Solución de problemas de instalación

Hay documentación completa para pip en [pip.pypa.io](https://pip.pypa.io) que te ayudará con la solución de problemas. A continuación, se muestran algunos de los problemas habituales que te ayudarán a identificarlos.

**Problemas de instalación**

Si la instalación de un paquete falla, es posible que veas un mensaje de error similar a estos:

```bash
No se pudo encontrar una versión que cumpla con el requerimiento <package-name (from versions: )>
```

```bash
No se encontró ninguna distribución coincidente para <package-name>
```

La causa más común de estos errores es un nombre de paquete mal escrito.

También debes verificar que estás utilizando el nombre del paquete y no el nombre del módulo. Por ejemplo, el nombre del paquete para PIL (Python Imaging Library) es `almohada` y no `PIL`.

**Problemas de importación de módulos**

Si el paquete se instala pero se produce un error cuando intentas importar el módulo, verifica lo siguiente:

1. ¿En qué versión de Python está instalando pip los paquetes?

    Si tienes varias versiones de Python en tu computadora, pip podría estar instalando módulos para una versión diferente de la que está usando tu programa.

    Puede tener que ver con estar usando la versión correcta del comando pip; asegúrate de estar usando `pip3`.

2. ¿Está incluido el paquete en tu lista de paquetes?

    Puedes usar el siguiente comando para ver una lista de todos los paquetes de Python que has instalado.

    ```bash
    pip3 list
    ```

## Actualización de un paquete

Cuando instalas un paquete de Python que ya está en tu computadora, esta no lo actualizará a la última versión.

Usa este comando para actualizar un paquete de Python a la última versión:

```bash
pip3 install --upgrade nombre_de_módulo 
```

## Desinstalación un paquete

Usa este comando para desinstalar un paquete de Python:

```bash
pip3 uninstall nombre_de_módulo
```
