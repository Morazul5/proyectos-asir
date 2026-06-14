
Contenido

[Objetivo](#objetivo)

[Inventario](#inventario)

[Ejecución](#ejecucion)

[Fdisk](#fdisk)

[Gparted](#gparted)

[Consideraciones Finales](#consideraciones-finales)

# Objetivo

El objetivo de esta práctica será particionar dos discos.

- En el primer disco crearemos:
  - 3 particiones primarias:
    - 1x 100 Mb
    - 1x 200 Mb
    - 1x 300 Mb (Activa)
- En el segundo disco crearemos:
  - 1x Partición primaria 200 Mb
  - 1x Partición extendida:
    - 1x unidad lógica 100 Mb
    - 1x unidad lógica 50 Mb
- Haremos esto mismo 3 veces:
  - La primera vez: con fdisk
  - La segunda vez: con Gparted
  - La tercera vez: con parted

# Inventario

Para ello necesitaremos una máquina virtual con las siguientes características:

- 1 CPU, 1 GB de RAM.
- Un HD de 2 Gbytes y otro HD de 4 Gbytes

# Ejecución

## Fdisk

![1](imágenes/Imagen1.png)
![2](imágenes/Imagen2.png)

- Ejecutaremos el comando _fdisk -l_ para ver los discos, sus sectores y particiones.
- Como vemos los dos discos que hemos añadido el kernel les ha llamado sdb y sdc

![3](imágenes/Imagen3.png)

- Accedemos al primer disco con fdisk

![4](imágenes/Imagen4.png)

- Le decimos que queremos crear una partición 1 de tipo primaria y que ocupe 100Mb

![5](imágenes/Imagen5.png)

- Para salir y guardar lo hacemos con "W"

![6](imágenes/Imagen6.png)

- Tras esto, crearemos la segunda partición de 200M

![7](imágenes/Imagen7.png)

- Y la tercera de 300M
- Además, le decimos que queremos que sea activa con el modificador -a

![8](imágenes/Imagen8.png)

- Ahora accedemos al segundo disco y creamos una partición de tipo primaria de 200M

![9](imágenes/Imagen9.png)

- Y ahora mediante el identificador -e creamos la segunda partición extendida

![10](imágenes/Imagen10.png)

- Ahora la siguiente vez que creemos una partición creará automáticamente unidades lógicas. Creamos dos: la primera 100Mib y la segunda de 50Mib

![11](imágenes/Imagen11.png)

## Gparted

![12](imágenes/Imagen12.png)

- Creamos una máquina con dos discos virtuales de las siguientes características:
  - 1er disco de 2 Gigabytes
  - 2do disco de 4 Gigabytes

![13](imágenes/Imagen13.png)

- Hemos hecho una Snapshot para poder volver al estado inicial.

![14](imágenes/Imagen14.png)

- Instalaremos GParted para realizar el particionamiento la primera vez.

![15](imágenes/Imagen15.png)

- Como vemos se nos instalará

![16](imágenes/Imagen16.png)

- Seleccionamos el primer disco

![17](imágenes/Imagen17.png)

- Antes de crear particiones tendremos que crear una tabla de particiones.

![18](imágenes/Imagen18.png)

- Daremos a Aplicar. Nos advierte que hacer esto eliminará todos los datos en el disco

![19](imágenes/Imagen19.png)

- Una vez creada la tabla de particiones podremos crear particiones

![20](imágenes/Imagen20.png)
![21](imágenes/Imagen21.png)
![22](imágenes/Imagen22.png)

- Crearemos tres particiones primarias

![23](imágenes/Imagen23.png)
![24](imágenes/Imagen24.png)
![25](imágenes/Imagen25.png)
![26](imágenes/Imagen26.png)
![27](imágenes/Imagen27.png)
![28](imágenes/Imagen28.png)

- Ahora seleccionamos el segundo disco y creamos una tabla de particiones.

![29](imágenes/Imagen29.png)

- Creamos una partición primaria de 200mb

![30](imágenes/Imagen30.png)

- Y una partición extendida con todo el tamaño libre que contendrá dos particiones lógicas

![31](imágenes/Imagen31.png)
![32](imágenes/Imagen32.png)

- Y dentro irán metidas las dos particiones lógicas

![33](imágenes/Imagen33.png)

- Así quedaría nuestro segundo disco tras realizar las operaciones. Con esto concluye la práctica.

# Consideraciones Finales

- Como vemos existen diversas opciones para realizar el particionamiento de un disco. Tanto gráficas como por línea de comandos.
- Son útiles porque no siempre queremos que el sistema operativo elija por nosotros las particiones.