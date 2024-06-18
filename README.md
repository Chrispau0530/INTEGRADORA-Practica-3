### 5. Cuadros para codigp o reseñas (BLOCKQUOTES)

Estos elementos son utilizados para resaltar instrucciones especificas para la instalacion, configuracion y/o  mostar secciones de codigo fuente. Se maqueta inciando el texto con un simbolo de mayor que (/>)

**EJEMPLO:**
para alistar las carpetas y archivos en desde una terminal de sistemas operativos de windos debemos ingresar el comando:

> C:/dir 
Despues oprimimos la tecla "Enter".
Tambien podemos ingresar texto multilinea

**EJEMPLO:**

>Aqui se ingresa un conjuto de instrucciones 
>Para explicar al usuario, como instalar el 
>sofware que hemos diseñado

Y si deseamos incluir viñetas par enlistar pasos podemos utilizar el caracter - dentro del texto a documentar. 

**EJEMPLO:**

*PASOS PARA INSTALAR LA BASE DE DATOS*

>- Decargar MySQL Server del Sitio Oficial 
>- instalar el Sistema Gestor de Base de Datos definiendo el puesto y la contraseña para el usuario **root**
>- Descargamos el archivo de respaldo de la base de datos (.sql)
>- restauramos la Base de Datos usando el comando mysql
>> C:/ProgramFiles/MySQL/MYSQLServer8.0/bin/mysql-u root -p password  respaldo sql

### 6. Listas ordenadas y Desordenadas*

sí en nuestra documentación necesitamos incluir información de texto en modo de lista, un elemento tras otro podemos
hacerlo utilizando los números con un punto decimal si las deseamos ordenadas o un guion en medio - si solo queremos una viñeta 

**EJEMPLO:**

Para poder crear tu primero repositorio en GitHub deveras;
  
1. Contar con una cuenta GitHub
   
2 .Dar clic en el botón *Nuevo Repositorio

3. Asignarle un nombre a tu repositorio, por ejemplo: 'ptactica03-3b'

4 .Asignarle un nivel de privacidad entre 

-**PUBLICO:** Si quieres que este disponible para todos los usuarios.

-**PRIVADO:** Si deseas que solo a quien decidas puedan colaborar con tu proyecto.

10. Definir si incluye un archivo de descripción llamado: README.md

11. Definir si habrá exclusiones de archivo a través del archivo a través del archivo : gitignore

12. Guardar los cambios 


#### 7. Ligas (Hipervínculos)

las ligas utilizadas para vincular elementos o referencias del proyecto dentro del mismo repositorio o fuera de el. Y se maquetan utilizando lo corchetes \[ \], inmediatamente después pondremos la liga de referencia entre paréntesis /()

**EJEMPLO:**

Mi buscardor favorito es:[www.google.com] / (https://www.google.com)
Pero si deseas poner solo las ligas directas a un correo electronico podemos utilizar los simbolos \<\>

**EJEMPLO:**
Documetacion creada por: ***Christian Paul Rodriguez Perez***
(<cg419370@gmail.com>)

(<http://www.utxicotepec.edu.mx>)

### 8. Tablas (TABLES)
Si la documentación lo requiere podemos presentar información en formato de tablas con filas y columnas, para maquetarlas podemos utiliziar el carácter delimitar /| para delifitar las columnas y /- para delimitar las filas.
**EJEMPLO:

|Encabezado 1 |Encabezado 2 |Encabezado 3 |Encabezado 4|
|-------------|-------------|-------------|------------|
|Fila 1 Celda 1|Fila 1 celda 2|Fila 1 celda 3|Fila 1 celda 4|
|Fila 2 Celda 1|Fila 2 celda 2|Fila 2 celda 3|Fila 2 celda 4|
|Fila 3 Celda 1|Fila 3 celda 2|Fila 3 celda 3|Fila 3 celda 4|

En caso de necesitar la funsión de celdas en columnas usaremos la proiedad "colspan" del tag <td< y en el caso de necesitar la fusión de las filas utilizaremos la propiedad rowspan.

**EJEMPLO:**

|Encabezado 1 |Encabezado 2 |Encabezado 3 |Encabezado 4|
|-------------|-------------|-------------|------------|
|Fila 1 Celda 1|Fila 1 celda 2|Fila 1 celda 3|Fila 1 celda 4|
|Fila 2 Celda 1|Fila 2 celda 2|              |Fila 2 celda 4|
|Fila 3 Celda 1|Fila 3 celda 2|Fila 3 celda 3|Fila 3 celda 4|
|              |Fila 4 celda 2|Fila 4 celda 3|Fila 4 celda 4|
|              |Fila 5 celda 2|Fila 5 celda 3|Fila 5 celda 4|
|Fila 6 Celda 1|Fila 6 celda 2|Fila 6 celda 3|Fila 6 celda 4|

Dado que en el ejemplo pasado usando solo markdown no se puede realizar la funcion de las filas debemos utilizar el estandar de HTML, usando los tags: <th> para los encabezados, <tr> para las filas y para las celdas, y en ellos utilizar la propiedad de colspan y rowspan

**EJEMPLO:**
<table>
<tr>
<th>Encabezado 1 </th>
<th>Encabezado 2</th>
<th>Encabezado 3 </th>
<th>Encabezado 4</th>
</tr>
<tr>
<td>Fila 1 Celda 1</td>
<td>Fila 1 Celda 2</td>
<td>Fila 1 Celda 3</td>
<td>Fila 1 Celda 4</td>
</tr>
<tr>

  <td>Fila 2 Celda 1</td>
  <td colspan=3 aling="center"> Fila 2 Celda 2 </td>
</tr>
<tr>
<td rowspan=3> Fila 3 Celda 1</td>
<td>Fila 3 Celda 2</td>
<td>Fila 3 Celda 3</td>
<td>Fila 3 Celda 4</td> 
</tr>


<tr>
<td>Fila 4 Celda 2 </td>
<td>Fila 4 Celda 3</td>
<td>Fila 4 Celda 4</td>
</tr>

<tr>
<td>Fila 5 Celda 2</td>
<td>Fila 5 Celda 3</td>
<td>Fila 5 Celda 4</td>
</tr>
<tr>
<td>Fila 5 Celda 1</td>
<td>Fila 5 Celda 2</td>
 <td>Fila 5 Celda 3</td> 
  <td>Fila 5 Celda 4</td>
</tr>

  
</table>


### 9.Agregacion de imagenes



![Aqui se ira los logos](https://github.com/Chrispau0530/INTEGRADORA-Practica-3/blob/main/LOGO%20TIC%20(4).png)
