
## _Práctica 7_ 

_**Ciclo Formativo de Grado Superior: Administración de Sistemas Informáticos en Red. Módulo: Gestión de Bases de Datos (GBD)**_ 

## _**Título de la práctica**_ 

_**Práctica 7:** Implantando un diseño BD de una biblioteca_ 
_**Profesor:** Pedro Guerrero López_


## _**Enunciado**_ 

En esta práctica se aprenderá a **implantar una BD** , previamente analizada por un analista y diseñada por un diseñador. En la siguiente unidad se aprenderá a analizar y a diseñar BD Realiza las siguientes operaciones partiendo de cero con una base de datos que se llamará **tunúmero  06 tunombresignificativo biblioteca.accdb (no es necesario hacer pantallazos)** : 

1. Crea una tabla llamada **tblSocio** con los campos (datos de los socios): a. **CódigoSocio** : Alfanumérico incremental. Con la descripción “Identificador único de socio”, por tanto tendrá que cumplir esta premisa. 

   - b. **NIF** : tipo adecuado, tamaño máximo de 12, indexado sin duplicados, es imprescindible rellenarlo, con máscara de entrada 8 dígitos y seguido de la letra en mayúscula escriba como se escriba. Tiene que ser de este tipo: 12.345.678-A (con esos puntos y guión) 

   - c. **Nombre** : de tipo adecuado con un tamaño máximo de 25 caracteres. 
   
   - d. **Apellido1** : de tipo adecuado, se puede duplicar, no puede quedar vacío. 
   
   - e. **Apellido2** : de tipo adecuado, máximo 25 caracteres, se puede duplicar. 
   
   - f. **Dirección** : contiene el tipo de vía, el nombre de la vía, el número, piso, puerta y escalera si es el caso. 

   - g. **Ciudad** : de tipo texto. Indexado. 
   
   - h. **Provincia** : de tipo texto. Por defecto será Pamplona lo que aparezca. i. **CP** : de tipo de dato adecuado, tamaño de 6, con una máscara de entrada del tipo 28.038 (con ese punto) 

   - j. **Teléfono** : de 15 caracteres con máscara de entrada (123) 456-78-90 
   - k. **FechaAlta** : Fecha corta. Necesario rellenarlo e indexado. 
   - l. **FechaBaja** : Fecha corta. 
   - m. **Cuota** : relacionado con la tabla **tblCuota** 
   - n. **Foto** : de tipo objeto incrustado. 
   - o. **Observaciones** : admite un texto ilimitado 


2. Crea una tabla llamada **tblCuota** con los campos (los tipos de cuotas a la que pueden acogerse los socios): 

- a. **IdCuota** : se trata de un texto con la descripción de “identificador único de cuota”. Máximo de 3 caracteres, requerido. 

- b. **Cuota** : es de tipo texto y alberga el nombre de la cuota: mensual, trimestral, semestral o anual. 

- c. **Importe** : valor en euros. 

- 3. Crea la tabla **tblLibro** con los campos (datos de los libros): a. **IdLibro** : será la clave primaria, autonumérico. 

   - b. **Isbn** : con máscara de entrada de isbn. 

   - c. **Titulo** : de tipo adecuado para contener el título de un libro. d. **FechaPublicación** : Fecha corta e. **FechaEntrada** : Fecha corta y nunca puede quedar sin rellenar. Indexado. f. **Seccion** : De tipo adecuado que contendrá la sección en la que se encuentra el libro. Relacionado con la tabla **tblSeccion** . 

   - g. **Descripcion** : contiene el abstract del libro, de tipo adecuado. 

4. Crea una tabla llamada **tblPago** con los campos (pagos realizados por los socios): 

   - a. **CPago** : número asignado por el SGBD automáticamente y único. 
   - b. **FechaPago** : Fecha corta, requerida e indexada. 
   - c. **Pagado** : booleano que indica si ha pagado o no. 
   - d. **Socio** : relacionado con la tabla tblSocio . Requerido e indexado 

5. Crea una tabla llamada **tblSeccion** con los campos (secciones a la que pertenecen los libros): 

   - a. **CodSeccion** : de tipo texto, máximo de 3 caracteres, identifica de forma única a la sección en esta tabla. 

   - b. **Seccion** : sin duplicados y no se puede dejar vacía 

6. Crea una tabla llamada **tblEmpleado** con los campos (datos de los empleados que tramitan el préstamo): 

   - a. **IdEmpleado** : autonumérico y clave 

   - b. **Nombre** : tipo adecuado 

   - c. **Apellidos** : tipo adecuado requerido 

   - d. **Dirección** : igual que en socios 

   - e. **Ciudad** : igual que en socios 
   
   - f. **Provincia** : por defecto Pamplona 
   
   - g. **CP** : igual que en socios 

   - h. **Teléfono** : igual que en socios 

   - i. **FechaAlta** : fecha corta 

7. Crea una tabla llamada **tblPrestamos** con los campos: 

   - a. **NumPrestamo** : autonumérico y clave. 

   - b. **FechaSalida** : Fecha corta, imprescindible, indexada c. **FechaDevolución** : nada especial 

   - d. **Retraso** : indica si hay retraso o no en la devolución. Tipo adecuado. 
   
   - e. **DiasRetraso** : exactamente eso. Tipo adecuado. 
   
   - f. **Socio** : imprescindible, indexada. Relacionado con la tabla **tblSocio** 
   
   - g. **Libro** : imprescindible, indexada. Relacionado con la tabla **tblLibro** 

   - h. **Empleado** : imprescindible, indexada, Relacionado con la tabla **tblEmpleado** 
   
   - i. **Los libros se prestan por 3 días, de forma que a partir del tercer día empieza a contar los días de retraso.** 

8. Crear las relaciones todas con integridad referencial: 

   - a. La relación entre la tblSocio y tblPago es de borrado en cascada. 

   - b. La relación entre la tblSocio y tblCuota es de actualización en cascada. c. La relación entre la tblSocio y tblPrestamo es de borrado en cascada. 

   - d. La relación entre la tblPrestamo y tblLibro es de borrado en cascada. 

   - e. La relación entre la tblLibro y tblSeccion es de actualización en cascada. 

   - f. La relación entre la tblPrestamo y tblEmpleado, no permite el borrado en cascada. 

9. Proporcionar los medios adecuados mediante  desplegables para que el usuario pueda rellenar las tablas de forma fácil y sencilla, usando las distintas variedades que ofrecen los controles. 

10. Rellena todas las tablas con la variedad de datos suficiente que permita demostrar su correcto funcionamiento. 

11. Escribe el orden en que has rellenado las tablas. 
