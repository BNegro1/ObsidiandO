
```python
# Productoria recursiva
El código entregado, mostrado en el código 1, consta de una función, llamada `sumatoria`, la cual recibe como entrada un número entero positivo y retorna un número entero positivo que representa la sumatoria desde 0 al número ingresado.

```python
# Modifique este código
def sumatoria(numero):
    '''
    Entrada: Número entero positivo
    Salida: Número entero positivo
    Proceso: Suma de los n primeros números enteros positivos
    '''
    if numero == 0:
        return 0
    return numero + sumatoria(numero - 1)
if __name__ == "__main__":
    # Estas líneas, correspondientes al bloque principal del programa, no se
    # ejecutarán si este módulo es importado. ¿Por qué?
    # Entrada
    n = int(input("Ingrese un número entero positivo: "))
    # Procesamiento
    res = sumatoria(n)
    # Salida
    print("La productoria de los", n, "primeros números es:", res)
```

**Código 1:** Código base con una sumatoria

Usando como base este código, escribe una función llamada `productoria` que, recibiendo el mismo tipo de entrada, retorne un número que represente la productoria del número 1 al número ingresado.

```python
# Modifique este código
def productoria(numero):
    '''
    Entrada: Número entero positivo
    Salida: Número entero positivo
    Proceso: Productoria de los n primeros números enteros positivos
    '''
    if numero == 1:
        return 1
    return numero * productoria(numero - 1)
```

Entrada a la función:

```python
2
```

Lo que debe retornar:

```python
2
```

Entrada a la función:

```python
15
```

Lo que debe retornar:

```python
1307674368000
```

Ten en cuenta que la función `productoria` ahora realiza la productoria en lugar de la sumatoria. Puedes agregar este código a tu entorno de desarrollo y ejecutarlo para probar los ejemplos proporcionados.