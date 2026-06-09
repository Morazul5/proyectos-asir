
> **Curso:** ASIR1
>
> **Alumno:** Pablo Andrés Mora Suárez
>
> **Nº Lista:** 14
>
> **Profesor:** Alfredo Abad
>
> **Módulo**: PAR
>
> **Fecha:** 07/01/2025

**PARP301:**

Proyecto de Cableado Estructurado en una oficina de dos plantas

# Contenido {#contenido .TOC-Heading}

[Introducción](#introducción)

[Planos originales](#planos-originales)

[Planta 1](#planta-1)

[Planta 2](#planta-2)

[Situación del edificio](#situación-del-edificio)

[]()

[Especificaciones del cliente](#especificaciones-del-cliente)

[Objetivos del proyecto](#objetivos-del-proyecto)

[Soluciones Propuestas](#soluciones-propuestas)

[Elección y compra de materiales](#elección-y-compra-de-materiales)

[Subsistema de Cableado Horizontal](#subsistema-de-cableado-horizontal)

[Subsistema de Cableado Vertical](#subsistema-de-cableado-vertical)

[Racks de la Planta 1 y 2](#racks-de-la-planta-1-y-2)

[Elementos del Rack de la Planta 1 y 2](#elementos-del-rack-de-la-planta-1-y-2)

[Planos posteriores](#planos-posteriores)

[Planta 1](#planta-1-1)

[Planta 2](#planta-2-1)

[Topología De La Red](#topología-de-la-red)

[Subsistemas De Red](#subsistemas-de-red)

[Cronograma / Diagrama de Gantt](#cronograma-diagrama-de-gantt)

[Inventario Cables](#inventario-cables)

[Etiquetado de los cables](#etiquetado-de-los-cables)

[Inventario de tomas de datos](#inventario-de-rosetas-y-puntos-de-red)

[Presupuesto](#presupuesto)

[Contrato](#contrato)

# Introducción

## El Cliente

**Abogados España S.A** es un Despacho especializado con más de 25 años
de experiencia prestando servicios jurídicos en Madrid, así como el
resto de España. Cuenta con Abogados expertos en extranjería, así como
otras especialidades del Derecho. Este año han decidido mudar sus
oficinas ubicadas en la calle Orense para ampliar y modernizar sus
instalaciones a un edificio empresarial de varias plantas. Sin embargo,
antes de migrar todo el mobiliario y sus trabajadores, es necesario
cablear el edificio por lo que han solicitado nuestros servicios.

![Ilustración](media/image2.jpeg){width="3.3328707349081363in"
height="3.3328707349081363in"}

## El Contratista

**CE Solutions** es una empresa de ingeniería de sistemas con sede en
Madrid, especializada en el diseño, despliegue y certificación de
infraestructuras de telecomunicaciones. Fundada por *Pablo Andres Mora
Suarez,* nuestra firma nace como una startup en 2025 con la misión de
transformar el cableado pasivo en un activo estratégico para las
empresas que no pueden permitirse fallos de conexión.

[]{#_Toc218710169
.anchor}![](media/image3.png){width="4.091666666666667in"
height="2.233634076990376in"}

# PLANOS ORIGINALES

## Planta 1

![Diagrama, Dibujo de ingeniería El contenido generado por IA puede ser
incorrecto.](media/image4.jpeg){width="6.268055555555556in"
height="3.4583333333333335in"}

**Características:**

- 15 Oficinas Privadas

- 3 Salas de Apoyo

  - Recepción

  - Sala de Conferencias

  - Sala de Descanso

  - Cuarto de Almacenamiento

    - Sala de Telecomunicaciones (TD) /Sala de Equipamiento (ER)

      - Rack

- Trabajadores (estimado):

  - 1era Planta

    - 15 abogados

    - 1 recepcionista

      - Total: 16 trabajadores

- Dimensiones:

  - Largo: 75 Pies = 22,86 Metros

  - Ancho: 47 Pies = 14,32 Metros

## Planta 2

![Diagrama, Dibujo de ingeniería El contenido generado por IA puede ser
incorrecto.](media/image5.jpeg){width="5.45in"
height="2.966666666666667in"}

**Características**:

- 23 Oficinas Privadas

- 4 Salas De Apoyo

  - Sala De Copiado

  - Sala De Descanso

  - Librería

  - Sala De Telecomunicaciones (TD)

  - Cuarto de Limpieza

  - Cuarto de Configuración

  - Cuarto de Almacenamiento

- Trabajadores (estimado):

  - 2da Planta

    - 23 abogados

    - 1 administrativo

    - 1 fotocopiador

    - 4 paralegales

      - Total: 29 trabajadores

- Total (entre ambas plantas): 45 trabajadores

- Dimensiones:

  - Largo: 152 Pies = 46,3 Metros

  - Ancho: 55 Pies = 16,7 Metros

*\*

# Situación del edificio

El edificio empresarial en la Calle Orense, 40 fue construido a mediados
de los años 80 y presenta una estructura de hormigón armado macizo y una
distribución eléctrica que no fue diseñada para la densidad de los
dispositivos digitales actuales. Al ser un edificio antiguo, no existen
"patinillos" por lo que la comunicación entre plantas sube por un tubo
rígido de acero (EMT) atravesando el hormigón. Además, las paredes son
de ladrillo macizo lo que impide el paso de cables por el interior.
Salvo en una sala de la 1era planta no hay suelo técnico por lo que las
canalizaciones se tendrán que realizar por las paredes.

# Especificaciones del cliente

- Internet cableado de alta velocidad (al menos 1 Gigabit)

- Debe haber al menos 1 punto de red para voz y datos por cada empleado

<!-- -->

- Redes inalámbricas para abogados y clientes

- Sistema de Videovigilancia CCTV

- Se espera un crecimiento del 40% en tres años

- Se espera adquirir una tercera planta

- Se espera trasladar a la mitad de la plantilla el 3 de enero

- El plazo máximo para acabar el proyecto será de 30 días laborables.

# Objetivos del proyecto

- Minimizar Interferencia electromagnética (EMI)

- Redundancia en subsistema de cableado vertical (Backbone)

- Garantizar la escalabilidad del cableado

- Asegurar una buena conexión de red inalámbrica

- Independencia de Redes

# Soluciones Propuestas

- Cableado de categoría 6A F/UTP de hasta 10 Gbps

- Uso de Rejiband oculto bajo techo

- Fibra óptica multimodo (OM4) entre los armarios de ambas plantas

- Instalación del doble de puntos de red necesarios en oficinas y salas
  de apoyo

- Puntos de acceso (AP) en lugares clave como la sala de espera o sala
  de conferencias

- VLANs para crear dos redes diferentes (red de abogados y de invitados)

- Ofrecemos descuentos de costes de instalación a cambio de un contrato
  de mantenimiento por dos años

# Elección y compra de materiales

## Subsistema de Cableado Horizontal

Cableado elegido: F/UTP Categoría 6ª (cat 6a)

El cable **U/FTP de Categoría 6** (Cat 6) es un tipo de cable de red
diseñado para ofrecer un alto rendimiento y una protección superior
contra las interferencias. Sus siglas significan *Unshielded Foiled
Twisted* *Pair* que significa que no tiene una protección global pero
sus pares de hilos están envueltos individualmente en una capa de
aluminio.

![CABLE U/FTP CAT6 LSHZ DCA DRAKA AZUL C.305 \|
Cablecel](media/image6.jpeg){width="3.635323709536308in"
height="1.53125in"}

**Características**:

- Velocidad de Transmisión: Hasta 10 Gbps (Gigabit por segundo).

- Ancho de Banda: Hasta 500 MHz.

- Distancia Máxima: Hasta 100 metros.

- Viene en rollos o bobinas de 305 metros. En nuestro caso hemos
  comprado 10 unidades al necesitar unos 2700 metros.

**Ventajas**:

- Ofrece una mejor protección contra interferencias electromagnéticas en
  comparación con Cat 5e.

**Bandeja Portacables**: Rejiband 60x100 mm 3mts

***Rejiband*** es una marca de bandeja portacables desarrollada por
*Pemsa*, aunque el termino se ha popularizado para referirse a cualquier
tipo de canalización eléctrica.

Son estructuras abiertas hechas de varillas de acero galvanizado que son
fáciles de instalar y sirven para guiar y soportar cables en
instalaciones profesionales

Viene en tiras de 3 metros que se juntan mediante uniones y se apoya al
forjado mediante soportes instalados cada 1,5 metros, por lo que no va
directamente apoyado sobre el falso techo. Los cables van sujetados por
bridas a la bandeja. La bajada de los cables se realizará utilizando
tubos rígidos.

En nuestro caso vamos a estar utilizando Rejiband al no haber falso
suelo ni poder atravesar los muros y estará situado oculto bajo techo
por motivos estéticos y de organización.

![](media/image7.png){width="4.781944444444444in" height="2.025in"}

**Canalizaciones**: Canaletas 6x9 mm de 2 mts

El recorrido desde la bajada de los tubos hasta las rosetas se realizará
mediante canaletas pegadas a la pared. Como hemos estimado serán
necesarios 380 mts de canaletas por lo que hemos comprado 190 unidades
de 2 mts

![Canaleta adhesiva TEHALIT blanca 6x9 mm de 2 metros -
1](media/image8.jpeg){width="2.2333333333333334in"
height="2.007173009623797in"}

**Rosetas**: Las rosetas son puntos de conexión en las áreas de trabajo
que permiten la conexión de dispositivos finales al sistema de cableado
estructurado.

Proporcionan un punto de terminación organizado para los cables de red.
y permiten a los usuarios conectar dispositivos como computadoras,
teléfonos, impresoras y otros equipos a la red.

Rosetas empleadas: de CAT6 FTP

- Rosetas simples: Admiten servicio de voz y datos. Se han instalado en
  puestos de trabajo individuales.

![Imagen de la pantalla de un celular El contenido generado por IA puede
ser incorrecto.](media/image9.jpeg){width="1.5858420822397201in"
height="1.6666666666666667in"}

- Rosetas dobles: Se han utilizado en espacios donde hay varios
  empleados.

![](media/image10.jpeg){width="1.7144531933508311in" height="1.575in"}

- Rosetas de 4 puertos: Se han utilizado en espacios compartidos donde
  hay 2 o más empleados y en salas de apoyo que cuentan con dispositivos
  (impresoras, escaners, fax, etc.)

![Imagen que contiene conector, electrónica, edificio, frente El
contenido generado por IA puede ser
incorrecto.](media/image11.png){width="1.7083333333333333in"
height="1.752965879265092in"}

**Conectores**: Pack 100 Conectores RJ-45

Se ha estimado un total de 234 conectores necesarios para 117
latiguillos (patch cords) por lo que se han adquirido 3 unidades de
conectores RJ-45 de categoría 6. Deben ser de tipo FTP para coincidir
con el tipo de cableado que hemos empleado.

![Imagen que contiene hombre El contenido generado por IA puede ser
incorrecto.](media/image12.png){width="2.917694663167104in"
height="3.25in"}

**Punto de Acceso Wifi** (APs): Ubiquiti U7 Lite

Se han instalado Puntos de Acceso Wi-Fi 7 de 2,5 GbE en puntos clave del
despacho como la sala de recepción o la sala de conferencias para
garantizar una buena conexión a las redes inalámbricas de abogados e
invitados. Se conectarán al switch PoE en la primera planta.

![Ubiquiti U7 Lite Punto de Acceso WiFi 7 con 4 Flujos Espaciales y
Enlace Ascendente de 2.5GbE
PoE](media/image13.jpeg){width="2.6333333333333333in"
height="2.7017311898512686in"}

**Cámara para exteriores IP**: Reolink P320

Se instalarán cámara IP para monitorizar las principales entradas del
despacho las cuales tienen una resolución de 2880 x 1620 píxeles, visión
nocturna,110° FOV, al igual que los APs, se conectarán mediante cable
Ethernet al switch PoE de 24 puertos en la primera planta.

![Reolink P320](media/image14.jpeg){width="4.266666666666667in"
height="2.2519827209098864in"}

**Etiquetas y Bridas**

Los cables se etiquetarán con un nombre identificativo y las bridas nos
ayudarán a organizar los cables sobre el Rejiband

![Etiquetas para cables Panduit 17.8x33.8x8.4 mm \| Sunpro Redes y
Sistemas](media/image15.jpeg){width="2.3in" height="2.3in"}![cubierta y
el aislamiento del cable durante el
tendido](media/image16.png){width="3.4in" height="2.2831157042869643in"}

## Subsistema de Cableado Vertical

**Fibra Óptica**

La Fibra Óptica empleada entre plantas será Multimodo OM4 (Optical
Multimode) de 6 hilos que permite alcanzar velocidades de entre 40 y 100
Gbps hasta los 150 metros asegurando la escalabilidad del proyecto ante
la posible adquisición de una tercera planta.

A diferencia de la fibra OM3, la fibra OM4 tiene un ancho de banda mayor
lo que permite que la señal llegue más lejos cubriendo cómodamente la
altura del edificio

Se ha optado por fibra óptica de 6 hilos (3 pares) de los cuales:

- Emplearemos 1 par para datos

- Emplearemos 2 pares de reserva en caso de futuras expansiones o
  reparaciones en caso de rotura.

![Imagen que contiene Diagrama El contenido generado por IA puede ser
incorrecto.](media/image17.jpeg){width="6.268055555555556in"
height="1.5694444444444444in"}

**Conectores:** LC Multimodo OM4 (Little Conector)

![Conector LC multimodo,
simple](media/image18.jpeg){width="2.464284776902887in"
height="2.464284776902887in"}

**Transceptor de Fibra:** SFP-10G-SR300m

![](media/image19.png){width="2.415277777777778in"
height="1.6145833333333333in"}

Es un módulo óptico enchufable que permite transmitir datos a 10
Gigabits por segundo hasta 300 metros usando fibra multimodo (MMF),
Convierte las señales eléctricas en luz y viceversa para conectar
equipos de red como switches y routers.

## Racks de la Planta 1 y 2

Rack 1:

Panel portacables

Panel de Conexión de 48 Puertos (Compartido)

Switch de 48 Puertos

Ventilación

Espacio de Reserva

Router

SAI

Multiplicador de puertos

Switch PoE de 16 Puertos

![Ventilación](media/image20.png){width="2.615301837270341in"
height="3.586699475065617in"}

Rack 2:

Ventilación

Ventilación

Switch de 48 Puertos

Panel de Conexión de 48 Puertos

Panel Portacables

Switch de 48 Puertos

Espacio de Reserva

Multiplicador de Puertos

Switch PoE de 16 puertos

Panel Portacables

SAI

Panel de Conexión de 48 Puertos (Compartido)

![](media/image21.png){width="2.537037401574803in"
height="3.408569553805774in"}

## Elementos del Rack de la Planta 1 y 2

**Rack**: Armario de 18U

Los racks son estructuras diseñadas para montar y organizar equipos
electrónicos en un sistema de cableado estructurado.

![Bastidor de Pared Lanberg WF01-6618-10B 18U 60kg 19\" Acero Negro IP20
Autoinstalable](media/image22.jpeg){width="2.9375in" height="2.9375in"}

**\**

Los dispositivos de red que alberga el rack incluyen:

**Switch**: Switch TP-Link TL-SG1048 de 48 Puertos, TP-LINK TL-SG1024
Switch de 24 Puertos y HP 2530 de 24 Puertos Con Alimentación PoE+

Los switches son componentes clave en una red, permitiendo la conexión
de múltiples dispositivos en una red local. Pueden ser switches de
acceso, distribución o núcleo, dependiendo de su ubicación en la red.
Los switches se montan típicamente en un rack para facilitar la gestión
del cableado y el acceso para el mantenimiento.

![](media/image23.png){width="5.563999343832021in"
height="1.4269050743657044in"}

**Routers**: Fortinet FG-60F-EU

Los routers se utilizan para enrutar el tráfico entre redes. En un
entorno de cableado estructurado, los routers pueden montarse en racks
para facilitar su acceso y mantenimiento.

![](media/image24.png){width="3.922636701662292in"
height="3.001304680664917in"}

**Patch Panels (Paneles de Conexión)**

Los patch panels, que actúan como puntos de terminación organizados para
los cables de red, son comúnmente montados en racks. Esto facilita la
gestión del cableado y la conexión ordenada de cables desde las áreas de
trabajo hacia los dispositivos de red.

![Texto Descripción generada automáticamente con confianza
media](media/image25.png){width="6.621094706911636in"
height="2.652173009623797in"}

**Equipos de Energía (PDU)**:

Los racks a menudo incluyen unidades de distribución de energía (PDU,
por sus siglas en inglés) para gestionar y distribuir la energía
eléctrica de manera eficiente a los dispositivos conectados en el rack.

![Jual Indorack Power Distribution unit 6 Outlet With Ampere n Volt
Meter - Jakarta Pusat - Power Solution Pws \|
Tokopedia](media/image26.png){width="5.139535214348206in"
height="3.7329407261592302in"}

# Planos posteriores

## Planta 1

![Diagrama El contenido generado por IA puede ser
incorrecto.](media/image27.jpeg){width="8.489583333333334in"
height="5.148458005249344in"}

## Planta 2

![Diagrama El contenido generado por IA puede ser
incorrecto.](media/image28.jpeg){width="9.973663604549431in"
height="4.416666666666667in"}

+-------------------------------------------------------------------------------------------------------------+
| Elementos del plano                                                                                         |
+:=====================================================================:+:===================================:+
| ![](media/image29.png){width="0.5595231846019247in"                   | Número de Oficina o Sala de Apoyo   |
| height="0.5024289151356081in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image30.png){width="1.3762325021872266in"                   | Fibra Óptica del Demarc             |
| height="0.2111111111111111in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image31.png){width="1.4305555555555556in"                   | Cable RJ-45 (HC)                    |
| height="0.16972659667541556in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image32.png){width="1.3055555555555556in"                   | Canaletas                           |
| height="0.12462160979877515in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image33.png){width="1.3263888888888888in"                   | Rejiband oculto bajo falso techo    |
| height="0.27360454943132106in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image34.png){width="0.2820516185476815in"                   | Roseta Simple / Doble               |
| height="0.26286964129483814in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image35.png){width="0.7564107611548556in"                   | Roseta de 4 Puertos                 |
| height="0.2579472878390201in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image36.png){width="0.24880577427821524in"                  | Toma de Red Empotrada en Pared      |
| height="0.9414687226596675in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![Icono Descripción generada                                          | Punto de Acceso (AP)                |
| automáticamente](media/image37.png){width="0.3472222222222222in"      |                                     |
| height="0.4599573490813648in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image38.png){width="0.4382863079615048in"                   | Cámaras                             |
| height="0.5512817147856518in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image39.png){width="0.4871795713035871in"                   | Sala de Recepción                   |
| height="0.45027230971128607in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image40.png){width="0.4615387139107612in"                   | Sala de Descanso                    |
| height="0.44980424321959755in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image41.png){width="0.5320505249343832in"                   | Sala de Conferencia / Sala de       |
| height="0.4877132545931758in"}![](media/image42.png){width="0.5375in" | Copiado                             |
| height="0.5076377952755905in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image43.png){width="0.5096237970253719in"                   | Librería                            |
| height="0.49677602799650045in"}                                       |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image44.png){width="0.5206353893263342in"                   | Área Compartida                     |
| height="0.4994717847769029in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+
| ![](media/image45.png){width="0.49771872265966755in"                  | Sala de Reuniones                   |
| height="0.4852755905511811in"}                                        |                                     |
+-----------------------------------------------------------------------+-------------------------------------+

# Topología De La Red

La topología de red es la propiedad que indica la forma física de la
red. Aunque

La red está diseñada con una topología en estrella jerárquica. En este
modelo, cada punto de red se conecta mediante un enlace al patch panel
del rack de comunicaciones correspondiente a su planta que luego irá
conectado al switch.

Los racks de cada planta se interconectan entre sí mediante enlaces de
fibra óptica. Esta topología facilita el mantenimiento, la localización
de averías y la ampliación futura de la red.

![Red en estrella - Wikipedia, la enciclopedia
libre](media/image46.png){width="2.1333333333333333in"
height="2.0833333333333335in"}

# Subsistemas De Red

En un proyecto de cableado estructurado los cables se estructuran
segmentando la red en módulos independientes llamados subsistemas de red
de la siguiente manera:

- **Entrada de Servicio**:

la conexión con proveedores externos de servicios como la compañía
telefónica o proveedores de servicios de Internet.

- **Subsistema Distribuidor**:

El lugar central donde se alojan los dispositivos de red, como hubs,
switches, routers, entre otros dispositivos.

**\**

- **Subsistema Vertical (Backbone)**:

También llamado "Backbone" o troncal conecta los cuartos de equipos a lo
largo de diferentes pisos y áreas del edificio. Puede ser cableado de
fibra óptica o par trenzado.

- **Subsistema Horizontal o de planta**:

Conecta los paneles de conexión en los cuartos de telecomunicaciones a
las tomas de red en las áreas de trabajo. Los cables se desplazan en
canaletas o subsuelos.

- **Área de Trabajo**:

Incluye las tomas de red y dispositivos finales en las áreas de trabajo,
como escritorios y puestos de trabajo.

![Una guía completa de cableado estructurado \| Experto en redes de 10
Gigabit y soluciones de fibra óptica
-CRXCONEC](media/image47.jpeg){width="6.268055555555556in"
height="3.7305555555555556in"}

# Cronograma / Diagrama de Gantt

![Gráfico, Gráfico de rectángulos El contenido generado por IA puede ser
incorrecto.](media/image48.png){width="6.268055555555556in"
height="2.73125in"}

El proyecto dará a inicio el 2 de enero del 2026 y tendrá una duración
de 21 laborales hasta el día 2 de febrero del 2026 y tendrá un plazo
máximo de 30 días laborales, es decir hasta el 17 de febrero

![Escala de tiempo El contenido generado por IA puede ser
incorrecto.](media/image49.png){width="6.268055555555556in"
height="2.09375in"}

![Tabla El contenido generado por IA puede ser
incorrecto.](media/image50.png){width="2.072108486439195in"
height="2.638323490813648in"}Los días feriados ni los fines de semana
contarán para la realización de las obras.

Los días laborales se representan en azul.

[Enlace al cronograma](Cronograma/Cronograma%20CE.xlsx)

# Inventario Cables

  --------------------------------
      Total (mts)      692,980542
  ------------------- ------------
   número de cables        50
         RJ-45        

     Fibra Óptica      25,783784
  --------------------------------

En la primera planta se han contabilizado 50 latiguillos (Patch Cords) y
más de 600 metros de cable y 25 metros de fibra óptica.

  -------------------------------
      Total (mts)      2058,6358
  ------------------- -----------
   número de cables       69
         RJ-45        

  -------------------------------

En la segunda planta se han contabilizado 64 cables RJ-45 y más de 2000
metros de cable.

  ----------------------------------------------------------------
  **Ubicación**              **Longitud   **Cantidad   **Total
                             (mts)**      (ud)**       (mts)**
  -------------------------- ------------ ------------ -----------
  **Rack (Switch a Patch     0,5          119          59,5
  Panel)**                                             

  **Puesto (Roseta a         3            119          357
  PC/AP)**                                             

  **TOTAL LATIGUILLOS**                   **238**      **416,5**
  ----------------------------------------------------------------

Por otro lado se ha hecho una estimación de los latiguillos que conectan
el switch con el panel de conexión y la conexión final de la roseta al
equipo final.

  --------------------------------
       **RJ45**       
  ------------------- ------------
  **Metros en Total**   3168,11634

  **Cables en Total**          357

    **Conectores en            714
        Total**       
  --------------------------------

  -------------------------------
   **Fibra Óptica**   
  ------------------- -----------
  **Metros en Total**   25,783784

  -------------------------------

En total tenemos 3168 metros de cable, (unas 11 bobinas de 305 metros),
357 cables en total y en fibra óptica tan solo 25 metros al solo haber
empleado fibra óptica para conectar ambas plantas.

Enlace al [Inventario de Los
Cables](Presupuesto/Inventario%20de%20Cables.xlsx)

[]{#_Toc218710188 .anchor}

# Etiquetado de los cables

*Los cables estarán etiquetados en ambos extremos y seguirán la
siguiente nomenclatura*:

**Planta-Rack-Puerto**

**Planta-Rack-Dispositivo-Puerto**

Por ejemplo:

Origen Destino

P1-HC1-P1 P1-OF1-R1

P1-HC1-SW2-P1 P1-AP-1

# Inventario de rosetas y Puntos De Red

+-------------------------+------------+------------+------------+---+
| Espacio                 | simples    | dobles     | cuadruples |   |
|                         |            |            |            +---+
|                         |            |            |            |   |
+:==========:+:==========:+:==========:+:==========:+:==========:+:==+
| Planta 1                                                       |   |
+-------------------------+------------+------------+------------+---+
| Oficinas                | 30         |            |            |   |
+-------------------------+------------+------------+------------+---+
| Recepción               |            | 1          | 1          |   |
+-------------------------+------------+------------+------------+---+
| Sala de descanso        |            |            | 1          |   |
+-------------------------+------------+------------+------------+---+
| Sala de Conferencias    |            |            | 1          |   |
+-------------------------+------------+------------+------------+---+
| **Subtotal de Rosetas** | 34                                   |   |
+-------------------------+--------------------------------------+---+
| Planta 2                                                       |   |
+-------------------------+------------+------------+------------+---+
| Oficinas                | 46         |            |            |   |
+-------------------------+------------+------------+------------+---+
| Librería                |            | 1          | 1          |   |
+-------------------------+------------+------------+------------+---+
| Sala de Copiado         | 2          |            | 1          |   |
+-------------------------+------------+------------+------------+---+
| Area de Coworking       |            |            | 2          |   |
+-------------------------+------------+------------+------------+---+
| **Subtotal de Rosetas** | 53                                   |   |
+------------+------------+------------+------------+------------+---+
|            |            |            |            |            |   |
+------------+------------+------------+------------+------------+---+
| **Total por Tipo**      | 78         | 2          | 7          |   |
+-------------------------+------------+------------+------------+---+
| **Total de Rosetas**    | 87                                   |   |
+-------------------------+--------------------------------------+---+

+------------------+-----------+-----------+---+
| Puertos          | Planta 1  | Planta 2  |   |
|                  |           |           +---+
|                  |           |           |   |
+:================:+:=========:+:=========:+:==+
| Rosetas          | 44        | 66        |   |
+------------------+-----------+-----------+---+
| Access Points    | 3         | 3         |   |
| (APs)            |           |           |   |
+------------------+-----------+-----------+---+
| Cámaras de       | 3         |           |   |
| Vigilancia       |           |           |   |
+------------------+-----------+-----------+---+
| **Subtotal**     | 50        | 69        |   |
+------------------+-----------+-----------+---+
| **Total**        | 119                   |   |
+------------------+-----------------------+---+

+-----------------------------+--------------+--------------+--------------+--------------+--+
| Dispositivos                | Físicos      | Usados       | Activos      | Libres       |  |
|                             |              |              |              |              +--+
|                             |              |              |              |              |  |
+:============:+:============:+:============:+:============:+:============:+:============:+:=+
| Planta 1                                                                                |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Switch 1                    | 48           | 44           | 16           | 4            |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Switch 2 (PoE)              | 16           | 6            | 6            | 10           |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| **Subtotal**                | 64           | 50           | 22           | 14           |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Planta 2                                                                                |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Switch 1                    | 48           | 46           | 23           | 2            |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Switch 2 (PoE)              | 16           | 3            | 3            | 13           |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| Switch 3                    | 48           | 20           | 10           | 28           |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| **Subtotal**                | 112          | 69           | 36           | 43           |  |
+--------------+--------------+--------------+--------------+--------------+--------------+--+
|              |              |              |              |              |              |  |
+--------------+--------------+--------------+--------------+--------------+--------------+--+
| **Total**                   | 176          | 119          | 58           | 57           |  |
+-----------------------------+--------------+--------------+--------------+--------------+--+
| **Porcentaje (%) de escalabilidad**                       | 49,6                        |  |
+-----------------------------------------------------------+-----------------------------+--+

[Enlace al Inventario de Tomas de
datos](Presupuesto/Puntos%20de%20red.xlsx)

[]{#_Toc218710190 .anchor}

# Presupuesto

## Del Contratista

+-----------------------------------------------------------------------------------------------+
| Resumen                                                                                       |
+:=========:+:=========:+:=========:+:=========:+:=========:+:=========:+:=========:+:=========:+
| Subsistema de cableado horizontal                         | 7406,23                           |
+-----------------------------------------------------------+-----------------------------------+
| Subsistema de cableado vertical                           | 311,38 €                          |
+-----------------------------------------------------------+-----------------------------------+
| Racks Planta 1 y 2                                        | 5.092,56 €                        |
+-----------------------------------------------------------+-----------------------------------+
| Mano de Obra                                              | 10.128,00 €                       |
+-----------------------------------------------------------+-----------------------------------+
| Certificación                                             | 858,00 €                          |
+-----------------------------------------------------------+-----------------------------------+
| **Total (Sin IVA)**                                       | **23796,17**                      |
+-----------------------------------------------------------+-----------------------------------+
| **Total (Con IVA)**                                       | **28793,37**                      |
+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+-----------+-----------+
| Beneficios Estimados                                                                          |
+-----------------------------------------------------------+-----------------------------------+
| Ingreso total (PVP Cliente)                               | 37822,39                          |
+-----------------------------------------------------------+-----------------------------------+
| Costes directos                                           | -28.793,37 €                      |
+-----------------------------------------------------------+-----------------------------------+
| Amortización de herramientas                              | -300 €                            |
+-----------------------------------------------------------+-----------------------------------+
| **Beneficio neto estimado**                               | **8.729,02 €**                    |
+-----------------------------------------------------------+-----------------------------------+
| **Margen de ganancia (%)**                                | **23,1**                          |
+-----------------------------------------------------------+-----------------------------------+

## Del Cliente

+----------------------------------------------------------------------------+
| Resumen                                                                    |
+:==========================================:+:=============================:+
| Subsistema de cableado horizontal          | 7406,23                       |
+--------------------------------------------+-------------------------------+
| Subsistema de cableado vertical            | 311,38 €                      |
+--------------------------------------------+-------------------------------+
| Racks Planta 1 y 2                         | 5.092,56 €                    |
+--------------------------------------------+-------------------------------+
| Mano de Obra                               | 16.720,00 €                   |
+--------------------------------------------+-------------------------------+
| Certificación                              | 1.728,00 €                    |
+--------------------------------------------+-------------------------------+
| **Total (Sin IVA)**                        | **31258,17**                  |
+--------------------------------------------+-------------------------------+
| **Total (Con IVA)**                        | **37822,39**                  |
+--------------------------------------------+-------------------------------+

[]{#_Toc218710191 .anchor}

# Contrato

El contratista está obligado a realizar el trabajo que consta de:
*Subsistema Horizontal, Subsistema Vertical, Puntos de conectorización,
Redes Inalámbricas, Sistema de Videovigilancia*

El contratista cumplirá las fases del proyecto en las fechas propuestas:

- Semana 1: Pre-instalación, validación de diseño y montaje de
  racks/bandejas.

- Semana 2: Tendido de cableado horizontal (RJ45) y vertical (Fibra).

- Semana 3: Conectorización de puestos, instalación de WiFi 7 y
  certificación.

- Semana 4: Pruebas finales, limpieza y entrega de documentación.

El pago del servicio de instalación de cableado estructurado se
realizará en tres pagos, el primer pago será del 40 % en concepto de
acopio de materiales y reserva de fecha de inicio, el segundo pago
también será de 40% (15.128,956 €) una vez finalizada la fase de tendido
de cableado y montaje de infraestructura, y el tercer pago será del 20%,
es decir unos 7564,6 € El pago podrá realizarse mediante cheque o
mediante el ingreso del dinero a la cuenta bancaria que el proyectista
facilitará.

EL CONTRATISTA otorga una garantía de 25 años sobre los componentes
pasivos del sistema de cableado (cable, jacks, patch panels) y 2 años de
garantía sobre los equipos activos (puntos de acceso WiFi 7 y
transceptores ópticos).

En caso de retraso injustificado en la entrega de la obra por parte de
EL CONTRATISTA, se establece una penalidad diaria del 0.5% del valor
total del contrato, salvo causas de fuerza mayor debidamente
acreditadas.

[Enlace al Contrato](Contrato/Contrato.docx)
