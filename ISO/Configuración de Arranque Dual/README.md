Contenido

[Objetivo](#objetivo)

[Inventario](#inventario)

[Ejecución](#ejecución)

[Preguntas](#preguntas)

[Consideraciones Finales](#consideraciones_finales)

# Objetivo

- Configuración de una máquina virtual con arranque dual de sistemas operativos Windows y Linux

# Inventario

- Imagen de disco de Windows y Linux (sus correspondientes ficheros .iso)
- Live CD de Ubuntu
- Creación de Máquina virtual con disco virtual de 50 Gigabytes

# Ejecución

![1](imágenes/Imagen1.png)

- Creamos una máquina virtual con VMWare.
- Especificamos que queremos el sistema operativo Windows con un disco virtual de 50GB.

![2](imágenes/Imagen2.png)

- Si bien le hemos indicado que su sistema operativo será Windows cargaremos el Live CD de Ubuntu para crear las particiones con GParted.

![3](imágenes/Imagen3.png)

- Aquí damos a la primera opción. Traducido Probar o Instalar Ubuntu.

![4](imágenes/Imagen4.png)

- Seleccionamos nuestro idioma, distribución de teclado y damos a Probar Ubuntu ya que no lo queremos instalar.

![5](imágenes/Imagen5.png)

- Desde el menú buscamos e iniciamos Gparted

![6](imágenes/Imagen6.png)

- Creamos una tabla de particiones

![7](imágenes/Imagen7.png)

- Seleccionamos formato msdos que es lo mismo que MBR aunque también podría ser GPT.

![8](imágenes/Imagen8.png)

- Damos en Nueva para crear nuestras particiones

![9](imágenes/Imagen9.png)

- Primero que nada, crearemos nuestra partición de arranque de 300MB con formato fat32

![imágenes/Imagen10.png](imágenes/Imagen10.png)

- Seguido crearemos nuestra partición de 30GB con el sistema de archivos ntfs y la etiquetamos con un nombre identificativo

![11](imágenes/Imagen11.png)

- Y ya, por último, crearemos nuestra partición de Ubuntu con el resto del espacio (20GB) con sistema de archivos ext4.

![12](imágenes/Imagen12.png)

- Damos al check o visto en verde para aplicar los cambios realizados

![13](imágenes/Imagen13.png)
![15](imágenes/Imagen15.png)


- Tras esto damos a Gestionar Opciones y marcamos la casilla "Boot"
- Esto le indicará al sistema operativo que la partición será arrancable o booteable.

![16](imágenes/Imagen16.png)

- Como hemos seleccionado MBR será de vital importancia seleccionar un firmware de tipo BIOS ya que UEFI solo trabaja con tablas de particiones de tipo GPT
- Como hemos cambiado la BIOS es posible que tengamos que seleccionar que queremos arrancar desde el CDROM pulsando "esc" para acceder a la BIOS

![17](imágenes/Imagen17.png)

- Apagaremos nuestra máquina
- Introducimos el iso de Windows y la encendemos nuevamente
- Daremos a "Enter" para arrancar desde el CD

<div align="center">
  <img src="imágenes/Imagen18.png" width="45%" />
  <img src="imágenes/Imagen19.png" width="45%" />
  <img src="imágenes/Imagen20.png" width="45%" />
  <img src="imágenes/Imagen21.png" width="45%" />
  <img src="imágenes/Imagen22.png" width="45%" />
  <img src="imágenes/Imagen23.png" width="45%" />    
</div>

- Proseguimos con la instalación del sistema operativo como es normal

<div>
  <img src="imágenes/Imagen24.png" width="45%" />
  <img src="imágenes/Imagen25.png" width="45%" />    
</div>

- Como vemos no nos dejará instalar Windows en la partición de Linux al estar formateado con ext4
- En cambio, seleccionaremos la partición 2 de 29.3GB de Windows

<div>
  <img src="imágenes/Imagen26.png" width="45%" />
  <img src="imágenes/Imagen27.png" width="45%" />
  <img src="imágenes/Imagen28.png" width="45%" />
  <img src="imágenes/Imagen29.png" width="45%" />  
  <img src="imágenes/Imagen30.png" width="45%" />
  <img src="imágenes/Imagen31.png" width="45%" />          
</div>

- Proseguimos con la instalación de Windows como es habitual
- Una vez finalizada la instalación apagamos la máquina, introducimos el disco de Ubuntu y volvemos a iniciarla

![32](imágenes/Imagen32.png)

- Rápidamente pulsamos "ESC" y seleccionamos para cargar desde el disco como hemos hecho anteriormente.
- Dentro del menú de GRUB seleccionamos "Try or Install Ubuntu"

<div>
  <img src="imágenes/Imagen33.png" width="45%" />
  <img src="imágenes/Imagen34.png" width="45%" />
  <img src="imágenes/Imagen35.png" width="45%" />
  <img src="imágenes/Imagen36.png" width="45%" />          
</div>

- Proseguimos con la instalación de Ubuntu como es habitual y a diferencia de la vez anterior damos en la primera opción para instalar

![37](imágenes/Imagen37.png)

- Cuando lleguemos a este punto nos ofrecerá instalar Ubuntu junto a Windows. Esto seleccionará las particiones de forma automática. Sin embargo, para evitar equivocaciones del instalador seleccionaremos una instalación manual

![38](imágenes/Imagen38.png)

- En este caso como es Bios y no UEFI dejaremos la partición de arranque como está
- Seleccionamos la partición que hemos creado para Linux y damos en "_Change_"

![39](imágenes/Imagen39.png)

- En "_Used as_" dejamos ext4 y Mount Point o punto de montado seleccionamos / (root o el directorio raíz)

![40](imágenes/Imagen40.png)

- Hecho eso, cuando nos aparezca el / en la columna de Mount Point damos a "_Next_"

![41](imágenes/Imagen41.png)

- Y continuamos con la instalación
- Si se congela a la mitad es aconsejable actualizar el instalador, tuve un problema con eso.

![42](imágenes/Imagen42.png)

- Una vez acabado damos en "Restart now" o reiniciar ahora
- En mi caso, me arrancaba Ubuntu de primero entonces he hecho lo siguiente

![43](imágenes/Imagen43.png)

- Me he puesto en modo superusuario
- He comprobado que detectaba Windows 10
- He obligado actualizar Grub, el gestor de arranque

![44](imágenes/Imagen44.png)

- Se han efectuado los cambios, ahora reiniciamos

![45](imágenes/Imagen45.png)

- Y como vemos ahora al reiniciar ya nos debería aparecer el menú de GRUB el cual nos permitirá arrancar tanto desde Ubuntu como Windows 10

![46](imágenes/Imagen46.png)

- La primera vez que ejecutamos Windows detecta que hemos hecho cambios, quizá nos pida reiniciar, pero en última instancia, lo permitirá

![47](imágenes/Imagen47.png)
![48](imágenes/Imagen48.png)


- Con esto concluye la práctica, muchas gracias.

# Preguntas

- ¿Por qué hay que instalar primero Windows y después Ubuntu? ¿Qué ocurre si lo instalas en orden inverso?

- Como fue explicado en clase Windows utiliza un gestor de arranque (Windows Boot Manager) que solo permite arrancar sistemas Windows. Windows sobrescribe el sector cero o gestor de arranque haciendo que el equipo inicie directamente Windows sin posibilidad de iniciar con Linux.
- Linux en cambio, tiene un gestor de arranque (GRUB) más amigable que si permite iniciar Windows como hemos atestiguado.

# Consideraciones Finales

- Esta práctica me ha ayudado a comprender mejor el particionamiento, los sistemas de archivos, las tablas de particiones y las diferencias entre estos.
