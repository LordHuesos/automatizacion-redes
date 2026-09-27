# automatizacion-redes

# 1. Datos del equipo
Integrantes<br>
Joshua García Huerta<br>
Victor Martinez Curiel<br>
Jonathan de Luna <br>

Nombre de la materia: Automatización de Infraestructura Digital I

Carrera: Tecnologías de la Información Área Infraestructura de Redes Digitales

Fecha: Septiembre de 2026

# 2. Propósito de la práctica

El propósito de esta práctica fue preparar y configurar una estación de trabajo para realizar actividades de automatización de redes. Se instalaron y configuraron diferentes herramientas necesarias para desarrollar, probar y administrar proyectos relacionados con redes y máquinas virtuales.

También se verificó el funcionamiento de las herramientas mediante comandos y pruebas básicas.

# 3. Herramientas instaladas

Las principales herramientas utilizadas fueron:

Python 3.14.7: lenguaje de programación utilizado para desarrollar scripts de automatización.
Visual Studio Code: editor de código utilizado para crear y ejecutar programas en Python.
Git: sistema de control de versiones para administrar los cambios del proyecto.
GitHub: plataforma utilizada para almacenar y documentar el proyecto.
Postman: herramienta utilizada para realizar pruebas y solicitudes a APIs.
OpenConnect: herramienta utilizada para establecer conexiones VPN.
GNS3: plataforma para crear y simular topologías de redes.
GNS3 VM: máquina virtual utilizada junto con GNS3 para ejecutar dispositivos de red.
VMware Workstation: plataforma utilizada para ejecutar la GNS3 VM.
Docker: plataforma utilizada para crear y ejecutar contenedores.

# 4. Configuración realizada

Durante la práctica se realizaron las siguientes configuraciones:

Instalación y verificación de Python.
Instalación y configuración de Visual Studio Code.
Creación de un entorno virtual de Python mediante .venv.
Configuración del intérprete de Python en Visual Studio Code.
Creación y ejecución de un programa básico en Python.
Instalación y configuración de Git.
Configuración del nombre y correo electrónico de Git.
Creación del repositorio automatizacion-redes en GitHub.
Creación de la estructura básica del proyecto.
Instalación y verificación de Postman.
Instalación de OpenConnect.
Instalación y configuración de Docker.
Configuración de WSL2 para utilizar Docker.
Ejecución y comprobación del contenedor hello-world.
Ejecución de un contenedor Ubuntu.
Instalación/configuración de VMware Workstation.
Configuración de GNS3 VM.
Integración de GNS3 GUI con GNS3 VM mediante VMware Workstation.
Configuración de vmrun.exe para permitir que GNS3 pudiera comunicarse con VMware Workstation.

# 5. Verificación del entorno

Se realizaron diferentes pruebas para comprobar que las herramientas funcionaran correctamente.

Python

Se ejecutó:

python --version

Resultado obtenido:

Python 3.14.7

También se ejecutó un programa básico en Python mostrando el mensaje:

Hola Mundo!
Git

Se verificó la instalación mediante:

git --version

También se configuraron los datos del usuario mediante:

git config --global user.name "Tu Nombre"
git config --global user.email "tu-correo"
Docker

Se verificó Docker mediante:

docker --version

Posteriormente se ejecutó:

docker run hello-world

El resultado mostró:

Hello from Docker!
This message shows that your installation appears to be working correctly.

También se comprobó la ejecución de un contenedor Ubuntu.

WSL2

Se verificó la configuración mediante:

wsl --status

Y:

wsl -l -v

Se comprobó que Ubuntu y docker-desktop utilizaran la versión 2 de WSL.

GNS3 y GNS3 VM

Se configuró GNS3 para utilizar la GNS3 VM mediante VMware Workstation.

También se verificó la existencia de vmrun.exe mediante:

where vmrun

Resultado:

C:\Program Files\VMware\VMware Workstation\vmrun.exe

Con esto se comprobó que GNS3 podía localizar la herramienta necesaria para comunicarse con VMware Workstation.

# 6. Estructura del proyecto

La estructura principal del repositorio es:

automatizacion-redes/ <br>
│<br>
├── README.md<br>
├── requirements.txt<br>
│<br>
├── src/<br>
│<br>
├── tests/<br>
│<br>
├── data/<br>
│<br>
└── docs/<br>
    │<br>
    └── practica-01/<br>
        │<br>
        ├── evidencias/<br>
        ├── instalacion.md<br>
        ├── configuracion.md<br>
        └── verificacion.md<br>

La carpeta src contiene el código fuente, tests las pruebas, data los datos utilizados y docs la documentación y evidencias de la práctica.

# 7. Problemas encontrados y soluciones

Problema 1: Docker no detectaba la virtualización

Problema: Docker Desktop mostró un mensaje indicando que no se detectaba el soporte de virtualización.

Solución: Se comprobó que la virtualización estuviera habilitada en Windows y se configuró WSL2. Posteriormente se verificó que Docker pudiera ejecutar contenedores correctamente.

Problema 2: Error con WSL

Problema: Los comandos de WSL fueron escritos inicialmente con espacios incorrectos.

Solución: Se utilizaron los comandos correctos:

wsl --status
wsl -l -v

Se comprobó que Ubuntu funcionara con WSL2.

Problema 3: GNS3 no encontraba VMware vmrun

Problema: Al activar GNS3 VM apareció el error:

Could not find VMware vmrun, please make sure it is installed.

Solución: Se localizó el archivo vmrun.exe en:

C:\Program Files\VMware\VMware Workstation\vmrun.exe

Después se agregó la carpeta de VMware Workstation a las variables de entorno Path de Windows para que GNS3 pudiera encontrar vmrun.

# Conclusión Joshua

La práctica permitió instalar y configurar las herramientas necesarias para crear un entorno de automatización de redes. Se comprobó el funcionamiento de Python, Git, Docker, GNS3 y VMware, adquiriendo conocimientos para trabajar con diferentes tecnologías utilizadas en infraestructura de redes.

# Conclusión Victor

Durante la práctica se aprendió a preparar un entorno de trabajo para la automatización y administración de redes. Además de instalar las herramientas, se realizaron pruebas para verificar su funcionamiento y se resolvieron problemas relacionados con Docker, WSL2 y la conexión entre GNS3 y GNS3 VM.

# Conclusión Jonathan 

Con esta práctica se obtuvo un entorno funcional para realizar futuras actividades de redes y automatización. La configuración de las herramientas permitió comprender la importancia de utilizar correctamente sistemas de virtualización, contenedores, control de versiones y simuladores de red.
