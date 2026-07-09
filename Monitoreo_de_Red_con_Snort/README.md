La función de este proyecto es monitorear trafico de red entre maquinas con un IDS ( en este caso Snort ) para practicar técnicas de evasión usando Nmap.

Lo primero es configurar la red en la que vamos a trabajar:

![conf_de_Red](docs/images/Conf_de_red.png)

Confirmo con ipconfig desde una powershell:

```powershell
ipconfig
```
![Confirmacion_de_red](docs/images/Confirmacion_Red.png)

Así el sistema host actúa como router virtual. Instalo snort aqui para monitorear todo el trafico entre las maquinas. Así el sistema host actúa como router virtual.

Para ejecutar Snort abro una PowerShell.

Dentro me voy a la carpeta de Snort:

```powershell
cd C:\Snort\bin>
```

Y ejecuto el siguiente comando para identificar mi id de red:

```powershell
C:\Snort\bin> .\snort.exe -W
```

En este caso la mía es:

![num_red](docs/images/id_red.png)

Con esto ejecutamos el siguiente comando para correr Snort y dejarlo en escucha:

![comando](docs/images/comando_run.png)

Así se debería de ver:

![modo_escuha](docs/images/running.png)

Ahora pasamos con el primer escaneo de mi maquina Atacante a la red:

![comando](docs/images/scan1.png)

Snort funciona detectando así actividad maliciosa:

![respuesta](docs/images/res1.png)

Dejando el entorno listo para practicar técnicas de evasión.
