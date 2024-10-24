Inicio: 07/12/2023
Link: https://www.youtube.com/watch?v=r-uOLxNrNk8

# Parte 1 - Introducción

### ¿Qué es el análisis de datos'
Proceso de inspección, transformación, limpieza y modelado de datos, con el objetivo de descubrir información útil. Sacar conclusiones y ayudar la decisión tomada. Los datos son la transformación de la información recopilada.

### ¿Qué busca?
Recopilar datos, limpiarlos y transformarlos para su análisis.
Se utilizará pandas para leer y transformar datos.

### ¿Cómo se trabajará?
Análisis estadístico: Con Pandas, Matplotlib y Seaborn.

### ¿Qué se descubrirá?
Patrones o anomalías que puedan surgir. La información es clave. Transformaremos DATOS en INFORMACIÓN.
### ¿Cuál es el objetivo?
Todo esto es lo que se necesita para proporcionar una evidencia en nuestros hallazgos, crear informes, etc.

### Proceso de análisis de datos
1) Obtención de datos.
2) Limpiar los datos.
3) Reorganizar y remodelar los datos.
4) Análisis.
5) Acción.

### Ecosistema de PyData

![[Pasted image 20231207043929.png]]
# Parte 2 - Ejemplo de proyecto de análisis real en Python/Pandas

### 1) Importar librerías
Antes de empezar a codificar en sí, hay que tener las librerias (pre requsisitos) instalados y cargados dentro del book.
![[Pasted image 20231207044748.png]]
### 2) Importar datos
En este caso, se importar un archivo con extensión ".csv".
![[Pasted image 20231207045142.png]]
### 3) Mostrar header
Se realiza para poder visualizar los principales datos del archivo importado.
![[Pasted image 20231207045218.png]]
### 4) Estructura
Se utiliza el método ".shape()" para obtener el total de filas y columnas respectivamente.
![[Pasted image 20231207045416.png]]
### 4) Mostrar información
Se utiliza el método ".info()" para entender los valores y tipos de datos con los que estaremos trabajando.
![[Pasted image 20231207045256.png]]
### 5) Describir datos
Utilizaremos el método ".describe()" para tener una idea de las propiedades estadisticas de cada campo del dataset (conteo, promedio, mínimo, etc). 

![[Pasted image 20231207045543.png]]