# Documentación del Parcial

---

## Ejercicio 1: Paradigma Estructural

**Descripción:**  
Este ejercicio permite contar elementos pares en una lista, útil en análisis de datos como conteo de eventos o filtrado de registros.

**Código recibido:**
```python
def cuenta_pares(lista):
    contador = 0
    for n in lista:
        if n % 2 = 0:
            contador += 1
    return contador

print(cuenta_pares([1,2,3,4,5,6]))
```

**Error:**  
Se encontro un error en la línea #7, se usó el operador de asignación `=` en lugar del operador de comparación `==` en la condición del `if`.

**Solución:**
```python
if n % 2 == 0:
```

**Justificación:**  
El operador `=` asigna valores (util para variables), por otro lado el operador `==` compara valores. Para verificar si un número es par, se debe comparar el residuo de la división entre 2 con cero usando `==`, ya que este si es un operador para comparar y no para asignar como `=`.

---

## Ejercicio 2: Paradigma Programacion orientada a objetos

**Descripción:**
Este ejercicio modela figuras geométricas, útil en aplicaciones de diseño asistido por computadora o cálculo de áreas.

**Codigo recibido:**

```python
class Rectangulo:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura
    def area(self):
        return base * altura

r = Rectangulo(3, 4)
print(r.area())
```

**Error:**
El error encontrado fue que en la linea numero 9 no se estaba accediendo a los valores del objeto, si no que se estaban operando dos variables que no existian.

**Solución:**
```python
        return self.base * self.altura
```

**Justificación:**
Se arreglo el problema modificando las supuestas variables existentes de "base" y "altura" por las variables existentes creadas desde el init: "self.base" y "self.altura" ya que asi se accede a los valores almacenados en la instancia.

---