## ¿Qué es HTML5?
- HTML5 es la versión 5 del Lenguaje de Marcas de Hipertexto.
- Permite crear archivos web que serán servidos por un servidor y interpretados por un navegador.
- Implementa mejoras como una mejor descripción del contenido, nuevas formas de comunicación con el servidor, almacenamiento de datos en el lado del cliente, soporte nativo para contenido multimedia, gráficos vectoriales escalables (SVG), optimización de velocidad y uso de hardware, APIs para componentes de entrada/salida, y opciones de diseño más sofisticadas.

## Estructura de un documento HTML
- Está compuesto por un conjunto de etiquetas (tags) que tienen un significado específico para el navegador.
- Tiene una estructura estándar que comienza con la definición del tipo de documento (`<!DOCTYPE html>`), seguida de la etiqueta `<html>`, y las secciones `<head>` y `<body>`.
- La sección `<head>` se utiliza para configuraciones de la página, como el título, la codificación de caracteres y los metadatos.
- La sección `<body>` se utiliza para el diseño de la página mediante el uso de diferentes etiquetas.

```html
<!DOCTYPE html>
<html>
<head>
    <!-- Configuraciones de la página -->
    <title>Título de la Página</title>
    <meta charset="utf-8">
    <meta name="author" content="autor">
</head>
<body>
    <!-- Contenido de la página -->
    <h1>Encabezado</h1>
    <p>Párrafo</p>
</body>
</html>
```

# Introducción a las Hojas de Estilo

## ¿Qué es una hoja de estilo?

- Las hojas de estilo en cascada (CSS - Cascading Style Sheets) permiten definir reglas de estilo que se aplican al contenido de una página web.
- Las reglas de estilo se definen separadas del contenido HTML, lo que permite una independencia entre el diseño y el contenido.
- CSS surge como una forma de definir el diseño independiente del contenido.
- CSS3 es el complemento perfecto para HTML5.

## Formas de insertar una hoja de estilo

1. **CSS en línea**: Se aplica directamente en el elemento HTML utilizando el atributo `style`.
2. **CSS interno (embebido)**: Se define dentro del elemento `<style>` en la sección `<head>` del documento HTML.
3. **CSS externo**: Se crea en un archivo separado con extensión `.css` y se vincula al documento HTML mediante la etiqueta `<link rel="stylesheet" href="ruta/archivo.css">`.

## Selectores

Los selectores se utilizan para encontrar elementos HTML a los cuales se aplicarán los estilos CSS. Algunos tipos de selectores son:

- **Selector de elementos**: Selecciona elementos HTML según su nombre (etiqueta).
- **Selector de ID**: Selecciona un elemento específico mediante su atributo `id`.
- **Selector de clases**: Selecciona elementos HTML con un atributo de clase específico.
- **Selector universal**: Selecciona todos los elementos HTML de la página.
- **Selector de agrupación**: Selecciona todos los elementos HTML con las mismas definiciones de estilo.

## Modelo de Caja CSS

- El modelo de cajas es una característica clave de CSS, donde todos los elementos de una página se representan mediante cajas rectangulares.
- Las cajas pueden ser de tipo `block` o `inline`, lo que afecta su comportamiento en cuanto a ocupar todo el ancho disponible, forzar saltos de línea, respetar propiedades de ancho y alto, entre otros.
- Cada caja está compuesta por el contenido, el relleno (`padding`), el borde (`border`) y el margen (`margin`).
- La propiedad `display` permite definir el tipo de caja que se aplicará a un elemento.

## Colores

Los colores en CSS se pueden definir mediante:

- Nombre del color
- RGB (red, green, blue)
- Valores hexadecimales (HEX)
- HSL (Hue, Saturation, Light)
- RGBA (Red, Green, Blue, Alpha)
- HSLA (Hue, Saturation, Light, Alpha)

## Texto

Las reglas de estilo asociadas al texto permiten modificar propiedades como:

- Color
- Alineación
- Decoración
- Transformación
- Espaciado de caracteres
- Altura de línea
- Dirección del texto
- Espaciado entre palabras
- Sombra del texto

## Fuentes

Las reglas de estilo relacionadas con las fuentes permiten modificar:

- Familia de fuentes
- Estilo de la fuente
- Tamaño de la fuente
- Peso de la fuente

## Fondos

Las reglas de estilo de fondos permiten modificar características como:

- Color de fondo
- Imagen de fondo
- Repetición de la imagen de fondo en los ejes X y Y
- Ubicación (posición) de la imagen en el bloque

## Posicionamiento

- Los elementos se pueden alinear o "flotar" hacia la derecha o izquierda, rompiendo el algoritmo básico de dibujo de HTML.
- Se puede centrar horizontalmente un elemento de bloque utilizando la propiedad `margin` con el valor `auto`.
- El texto se puede alinear utilizando la propiedad `text-align` con el valor `center`.
Aquí está el resumen de los aspectos más importantes de Bootstrap sin incluir la sintaxis:

# Introducción a Bootstrap

## ¿Qué es Bootstrap?

- Bootstrap es un framework que permite crear interfaces web con CSS y JavaScript. 
- Su principal característica es el diseño web adaptable automáticamente a diferentes dispositivos (responsive design).
- Es de código abierto, tiene numerosos plugins y un buen soporte de la comunidad.

## Características de Bootstrap

- Sigue la filosofía "Mobile First", comenzando con el diseño para dispositivos móviles y escalando al resto.
- Se puede integrar descargando las librerías o utilizando un CDN (Content Delivery Network).

## Función y Estructuras

- Utiliza el concepto de `container` para definir el ancho máximo del contenido.
- `container-fluid` considera el 100% del ancho del dispositivo.
- `container-{breakpoint}` define el ancho hasta cierto tamaño de pantalla.

## Diseño del Framework

- Sistema de grilla con filas y columnas (12 columnas máximo).
- Las columnas se definen con la clase `col` y la especificación del ancho.
- Clases para puntos de quiebre específicos (sm, md, lg, xl) para definir el comportamiento de las columnas en diferentes tamaños de pantalla.

## Contenido del Framework

- Proporciona estilos predefinidos para elementos como encabezados, listas, tablas, formularios, direcciones e imágenes.

## Componentes del Framework

- Incluye componentes de interfaz de usuario como alertas, botones, barras de navegación, carrusel de imágenes, jumbotron, formularios, tablas, entre otros.