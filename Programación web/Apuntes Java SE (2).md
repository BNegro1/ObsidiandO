Java es uno de los lenguajes de programación más populares y versátiles. Su sintaxis limpia, su amplia gama de características y su robusto ecosistema lo convierten en una opción ideal para una variedad de aplicaciones, desde desarrollo web hasta aplicaciones empresariales y móviles. En este documento, exploraremos los conceptos fundamentales de Java. Desde variables y tipos de datos hasta conceptos avanzados como herencia y encapsulación, 

---
## Conceptos principales
### Variables en Java:
En Java, una variable es un contenedor que almacena datos que pueden cambiar durante la ejecución del programa. Las variables tienen un tipo de datos y un nombre único. Los tipos de variables en Java incluyen primitivos y referencias a objetos.

### Tipos de Datos en Java:
Java tiene varios tipos de datos, que se dividen en primitivos y de referencia. Los tipos primitivos incluyen `int`, `double`, `boolean`, `char`, entre otros. Los tipos de referencia incluyen clases, interfaces y arreglos.

### Ciclo de Vida de un Objeto (Crear instancias):
El ciclo de vida de un objeto en Java consta de cuatro etapas: 

1) Creación.
2) Inicialización.
3) Uso.
4) Desreferenciación. 

La creación ocurre cuando se utiliza la palabra clave `new`, la inicialización asigna valores a los campos del objeto, el uso implica la manipulación del objeto y la desreferenciación ocurre cuando el objeto ya no es accesible y el recolector de basura lo elimina.

### Clases de Envoltorio:
Las clases de envoltorio (wrapper classes) proporcionan un medio para convertir tipos primitivos en objetos. Por ejemplo, `Integer` envuelve el tipo primitivo `int`. Estas clases son útiles cuando se necesita tratar un tipo primitivo como un objeto.

### Operadores:
Java admite una variedad de operadores, incluyendo aritméticos (+, -, *, /), de asignación (=), de comparación (==, !=, <, >), lógicos (&&, ||, !), entre otros.

### Instrucciones if y Operador Ternario:
La instrucción `if` se utiliza para tomar decisiones basadas en una condición. El operador ternario es una forma abreviada de la instrucción `if` y se utiliza para asignar un valor a una variable basado en una condición.

### Igualdad de Objetos:
En Java, el operador `==` se utiliza para comparar la igualdad de referencias, mientras que el método `equals()` se utiliza para comparar la igualdad de contenido de objetos.

### Switch:
La instrucción `switch` se utiliza para seleccionar uno de varios bloques de código para ejecutar, según el valor de una expresión.

### Arrays:
Los arrays son estructuras de datos que almacenan una colección de elementos del **mismo tipo**. Se declaran utilizando corchetes [] y pueden contener cualquier tipo de datos, incluidos tipos primitivos y objetos.

### Arrays Multidimensionales:
Java admite arrays multidimensionales, que son arrays que contienen otros arrays. Por ejemplo, un array bidimensional es una matriz de matrices.

### For y While:
Los bucles `for` y `while` se utilizan para repetir un bloque de código varias veces. El bucle `for` es útil cuando se conoce el número exacto de iteraciones, mientras que el bucle `while` se utiliza cuando se desconoce el número exacto de iteraciones.

### Break y Continue:
Las palabras clave `break` y `continue` se utilizan dentro de bucles para alterar el flujo de ejecución. `Break` se utiliza para salir del bucle, mientras que `continue` se utiliza para saltar a la siguiente iteración del bucle.

### Métodos en Java:
Los métodos son bloques de código que realizan una tarea específica. Pueden aceptar parámetros y devolver un valor. Los métodos se definen dentro de una clase y se pueden llamar desde cualquier parte del programa, sería una especie de función si lo vemos desde Python u otro lenguaje de programación.

### Paso de Parámetros en Métodos:
Los parámetros se pasan a los métodos en Java por valor. Esto significa que una copia del valor del argumento se pasa al parámetro. Para los tipos primitivos, se pasa una copia del valor, mientras que para los objetos, se pasa una copia de la referencia al objeto.

### Miembros Estáticos:
Los miembros estáticos en Java pertenecen a la clase en lugar de a instancias individuales de la clase. Esto significa que se comparten entre todas las instancias de la clase y se pueden acceder sin crear una instancia de la clase.

### Constructores:
Los constructores en Java son métodos especiales que se utilizan para inicializar objetos. Tienen el mismo nombre que la clase y no tienen tipo de retorno. Se llaman automáticamente cuando se crea una instancia de la clase.

### Modificadores de Acceso:
Java proporciona modificadores de acceso para controlar la visibilidad de clases, variables, métodos y constructores. Los principales modificadores de acceso son `public`, `protected`, `private` y el predeterminado (sin modificador).

### Encapsulación:
La encapsulación es un concepto de programación que consiste en ocultar los detalles de implementación de un objeto y exponer solo las partes necesarias para interactuar con él. En Java, se logra mediante el uso de modificadores de acceso y métodos getters y setters.

### Conceptos de Herencia:
La herencia en Java permite a una clase heredar los campos y métodos de otra clase. Esto promueve la reutilización de código y facilita la creación de jerarquías de clases. La clase que hereda se llama subclase o clase derivada, mientras que la clase de la que se hereda se llama superclase o clase base.

Estos conceptos son fundamentales para entender y desarrollar aplicaciones en Java de manera efectiva y eficiente. Es esencial practicar y experimentar con estos conceptos para dominar el lenguaje y desarrollar aplicaciones robustas.

--- 

## Ejemplo de codificación 

### Variables en Java:
```java
int edad = 25;
double salario = 1500.50;
boolean esEstudiante = true;
char inicial = 'A';
String nombre = "Juan";
```

### Tipos de Datos en Java:
```java
int numero = 10;
double decimal = 3.14;
boolean esVerdadero = true;
char caracter = 'A';
String texto = "Hola Mundo";
```

### Ciclo de Vida de un Objeto:
```java
// Creación de un objeto
Persona persona = new Persona();

// Inicialización
persona.setNombre("Juan");
persona.setEdad(25);

// Uso del objeto
System.out.println("Nombre: " + persona.getNombre());
System.out.println("Edad: " + persona.getEdad());

// Desreferenciación (cuando el objeto ya no se necesita)
persona = null;
```

### Clases de Envoltorio:
```java
// Envolver un tipo primitivo en un objeto Integer
Integer numeroEntero = Integer.valueOf(10);

// Desenvolver el objeto en un tipo primitivo
int valor = numeroEntero.intValue();
```

### Operadores:
```java
int a = 10;
int b = 5;
int suma = a + b;
int resta = a - b;
double division = a / (double)b;
int multiplicacion = a * b;
boolean esMayor = a > b;
```

### Instrucciones if y Operador Ternario:
```java
// Instrucción if
int edad = 20;
if (edad >= 18) {
    System.out.println("Es mayor de edad");
} else {
    System.out.println("Es menor de edad");
}

// Operador ternario
String mensaje = (edad >= 18) ? "Es mayor de edad" : "Es menor de edad";
System.out.println(mensaje);
```

### Igualdad de Objetos:
```java
String texto1 = "Hola";
String texto2 = "Hola";
boolean sonIguales = texto1.equals(texto2); // true
```

### Switch:
```java
int opcion = 2;
switch (opcion) {
    case 1:
        System.out.println("Opción 1 seleccionada");
        break;
    case 2:
        System.out.println("Opción 2 seleccionada");
        break;
    default:
        System.out.println("Opción no válida");
}
```

### Arrays:
```java
int[] numeros = {1, 2, 3, 4, 5};
String[] nombres = new String[3];
nombres[0] = "Juan";
nombres[1] = "María";
nombres[2] = "Carlos";
```

### Arrays Multidimensionales:
```java
int[][] matriz = {{1, 2}, {3, 4}, {5, 6}};
```

### For y While:
```java
// Bucle for
for (int i = 0; i < 5; i++) {
    System.out.println("Iteración " + i);
}

// Bucle while
int contador = 0;
while (contador < 5) {
    System.out.println("Iteración " + contador);
    contador++;
}
```

### Break y Continue:
```java
// Uso de break
for (int i = 0; i < 10; i++) {
    if (i == 5) {
        break; // Sale del bucle cuando i es igual a 5
    }
    System.out.println(i);
}

// Uso de continue
for (int i = 0; i < 5; i++) {
    if (i == 2) {
        continue; // Salta a la siguiente iteración cuando i es igual a 2
    }
    System.out.println(i);
}
```

### Métodos en Java:
```java
public class Calculadora {
    public int sumar(int a, int b) {
        return a + b;
    }

    public double dividir(double a, double b) {
        return a / b;
    }
}
```

### Paso de Parámetros en Métodos:
```java
public class Ejemplo {
    public void modificar(int numero) {
        numero = 20;
    }

    public static void main(String[] args) {
        int valor = 10;
        Ejemplo ejemplo = new Ejemplo();
        ejemplo.modificar(valor);
        System.out.println(valor); // Salida: 10
    }
}
```

### Miembros Estáticos:
```java
public class Contador {
    public static int contador = 0;

    public Contador() {
        contador++;
    }
}
```

### Constructores:
```java
public class Persona {
    private String nombre;
    private int edad;

    // Constructor
    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    // Métodos getter y setter
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }
}
```

### Modificadores de Acceso:
```java
public class Ejemplo {
    private int edad; // Acceso privado
    protected String nombre; // Acceso protegido
    public double salario; // Acceso público

    // ...
}
```

### Encapsulación:
```java
public class Persona {
    private String nombre;
    private int edad;

    // Constructor
    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    // Métodos getter y setter
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }
}
```

### Conceptos de Herencia:
```java
public class Empleado extends Persona {
    private double salario;

    public Empleado(String nombre, int edad, double salario) {
        super(nombre, edad);
        this.salario = salario;
    }

    // Métodos getter y setter para salario
    public double getSalario() {
        return salario;
    }

    public void setSalario(double salario) {
        this.salario = salario;
    }
}
```
