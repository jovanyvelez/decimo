# Guía de Estudio: Expresiones Aritméticas, Lógicas y Estructuras de Control

**Curso de Programación - Nivel Básico**  
**Duración total: 4 horas (240 minutos)**  
**Público objetivo: Jóvenes de 15-16 años**

---

## 📋 Introducción

¡Bienvenido a esta guía de estudio sobre expresiones y control de flujo en programación! En los próximos 240 minutos, explorarás los conceptos fundamentales que permiten que los programas tomen decisiones y realizen cálculos. Estos temas son la base de todo lenguaje de programación y te abrirán las puertas a crear programas interactivos y funcionales.

### 🎯 Objetivos de Aprendizaje

Al finalizar este material, serás capaz de:

- Comprender y evaluar expresiones aritméticas
- Utilizar operadores relacionales para comparar valores
- Aplicar operadores lógicos para combinar condiciones
- Entender el concepto de expresiones booleanas
- Implementar estructuras de control (if/else, while, for)
- Traducir situaciones reales a expresiones lógicas

---

# 📅 Sesión 1: Fundamentos de Expresiones

## ⏱️ Tiempo estimado: 120 minutos + descanso de 15 minutos

---

## 1. Expresiones Aritméticas

Las expresiones aritméticas son combinaciones de números, variables y operadores que producen un resultado numérico. Son el lenguaje matemáticas de la programación.

### 1.1 Operadores Aritméticos Básicos

| Símbolo | Nombre | Ejemplo | Resultado |
|:-------:|--------|---------|:---------:|
| `+` | Suma | `5 + 3` | **8** |
| `-` | Resta | `10 - 4` | **6** |
| `*` | Multiplicación | `6 * 7` | **42** |
| `/` | División | `15 / 4` | **3.75** |
| `%` | Módulo (resto) | `17 % 5` | **2** |
| `**` | Potencia | `2 ** 3` | **8** |

### 1.2 Orden de Operaciones (Precedencia)

Cuando hay múltiples operaciones, Python las evalúa en un orden específica:

1. **Paréntesis** `()` - Se evalúa primero
2. **Potencia** `**`
3. **Multiplicación, División, Módulo** `* / %`
4. **Suma y Resta** `+ -`

#### Ejemplos Resueltos

**Ejemplo 1:**
```
Expresión: 3 + 4 * 2
Paso 1: 4 * 2 = 8    (multiplicación primero)
Paso 2: 3 + 8 = 11
Resultado: 11
```

**Ejemplo 2:**
```
Expresión: (3 + 4) * 2
Paso 1: 3 + 4 = 7    (paréntesis primero)
Paso 2: 7 * 2 = 14
Resultado: 14
```

**Ejemplo 3:**
```
Expresión: 10 - 2 * 3 + 8 / 4
Paso 1: 2 * 3 = 6
Paso 2: 8 / 4 = 2
Paso 3: 10 - 6 = 4
Paso 4: 4 + 2 = 6
Resultado: 6
```

### 1.3 Variables en Expresiones Aritméticas

Las variables pueden almacenar valores que luego usamos en cálculos:

```python
edad = 15
altura = 1.70
peso = 65

# Calcular el índice de masa corporal (IMC)
imc = peso / (altura ** 2)
print(imc)  # Resultado: 22.5
```

---

## 📝 Actividad 1: Evaluación de Expresiones Aritméticas

**Instrucciones:** Calcula el resultado de cada expresión sin usar la computadora. Luego, verifica con un programa.

| # | Expresión | Tu respuesta | Verificación |
|:---:|:-----------|:------------:|:------------:|
| 1 | `7 + 3 * 2` | | |
| 2 | `(7 + 3) * 2` | | |
| 3 | `10 / 2 - 3` | | |
| 4 | `17 % 5` | | |
| 5 | `2 ** 3 + 1` | | |
| 6 | `10 - 3 - 2` | | |
| 7 | `8 / (2 + 2)` | | |
| 8 | `25 % 6` | | |

<details>
<summary>✅ Ver respuestas - Actividad 1</summary>

| # | Expresión | Respuesta |
|:---:|:-----------|:---------:|
| 1 | `7 + 3 * 2` | **13** |
| 2 | `(7 + 3) * 2` | **20** |
| 3 | `10 / 2 - 3` | **2.0** |
| 4 | `17 % 5` | **2** |
| 5 | `2 ** 3 + 1` | **9** |
| 6 | `10 - 3 - 2` | **5** |
| 7 | `8 / (2 + 2)` | **2.0** |
| 8 | `25 % 6` | **1** |

</details>

---

## 2. Expresiones Relacionales

Las expresiones relacionales comparan dos valores y siempre producen un resultado **booleano** (verdadero o falso).

### 2.1 Operadores de Comparación

| Símbolo | Significado | Ejemplo | Resultado |
|:-------:|-------------|:-------:|:---------:|
| `==` | Igual a | `5 == 5` | **True** |
| `!=` | Diferente de | `3 != 5` | **True** |
| `>` | Mayor que | `7 > 3` | **True** |
| `<` | Menor que | `2 < 8` | **True** |
| `>=` | Mayor o igual | `5 >= 5` | **True** |
| `<=` | Menor o igual | `4 <= 2` | **False** |

### 2.2 Ejemplos con Valores

```python
# Comparaciones con números
print(10 > 5)     # True
print(3 == 3)     # True
print(7 != 7)     # False
print(5 >= 10)    # False

# Comparaciones con variables
edad = 16
print(edad >= 15)  # True (un joven de 16 años puede manejar)
print(edad < 18)   # True
```

### 2.3 Comparaciones con Strings

```python
nombre = "Ana"
print(nombre == "Ana")   # True
print(nombre != "Pedro") # True
```

---

## 📝 Actividad 2: Expresiones Relacionales

**Instrucciones:** Determina si cada expresión es True o False.

| # | Expresión | Tu respuesta |
|:---:|:-----------|:------------:|
| 1 | `8 > 3` | |
| 2 | `5 == 5` | |
| 3 | `10 < 5` | |
| 4 | `7 != 7` | |
| 5 | `12 >= 12` | |
| 6 | `4 <= 2` | |
| 7 | `15 != 15 + 1` | |
| 8 | `3 + 2 == 5` | |

<details>
<summary>✅ Ver respuestas - Actividad 2</summary>

| # | Expresión | Respuesta |
|:---:|:-----------|:---------:|
| 1 | `8 > 3` | **True** |
| 2 | `5 == 5` | **True** |
| 3 | `10 < 5` | **False** |
| 4 | `7 != 7` | **False** |
| 5 | `12 >= 12` | **True** |
| 6 | `4 <= 2` | **False** |
| 7 | `15 != 15 + 1` | **True** |
| 8 | `3 + 2 == 5` | **True** |

</details>

---

## ☕ DESCANSO - 15 minutos

**Hora: Transcurridos 120 minutos**

Es momento de descansar. Durante estos 15 minutos:

- 🚶 Muévete un poco
- 💧 Bebe agua
- 👀 Descansa la vista
- 💬 Conversa con tus compañeros

Volveremos renovados para continuar con expresiones booleanas y estructuras de control.

---

# 📅 Sesión 2: Lógica Booleana y Estructuras de Control

## ⏱️ Tiempo estimado: 105 minutos + descanso de 15 minutos

---

## 3. Expresiones Booleanas y Operadores Lógicos

Las expresiones booleanas son fundamentales en programación. Permiten tomar decisiones basándose en condiciones que pueden ser verdaderas o falsas.

### 3.1 El Tipo Booleano

El tipo booleano solo puede tener dos valores: `True` (verdadero) o `False` (falso).

```python
es_mayor = True
tiene_permiso = False
```

### 3.2 Operadores Lógicos

Los operadores lógicos combinan múltiples expresiones booleanas.

| Símbolo | Nombre | Descripción | Ejemplo | Resultado |
|:-------:|--------|-------------|:-------:|:---------:|
| `and` | Y | True solo si **ambos** son True | `True and False` | **False** |
| `or` | O | True si **al menos uno** es True | `True or False` | **True** |
| `not` | NO | Invierte el valor | `not False` | **True** |

### 3.3 Tablas de Verdad

#### Operador AND

| A | B | A and B |
|:-:|:-:|:-------:|
| True | True | **True** |
| True | False | **False** |
| False | True | **False** |
| False | False | **False** |

#### Operador OR

| A | B | A or B |
|:-:|:-:|:------:|
| True | True | **True** |
| True | False | **True** |
| False | True | **True** |
| False | False | **False** |

#### Operador NOT

| A | not A |
|:---:|:-----:|
| True | **False** |
| False | **True** |

### 3.4 Ejemplos Combinados

```python
edad = 16
tiene_licencia = True
tiene_coche = False

# ¿Puede conducir legalmente?
puede_conducir = edad >= 18 and tiene_licencia
print(puede_conducir)  # False (tiene 16 años)

# ¿Tiene vehículo o licencia?
tiene_alternativa = tiene_licencia or tiene_coche
print(tiene_alternativa)  # True

# ¿No es mayor de edad?
es_menor = not (edad >= 18)
print(es_menor)  # True
```

### 3.5 Precedencia de Operadores Lógicos

Orden de evaluación:
1. `not`
2. `and`
3. `or`

```python
# Ejemplo:
print(True or False and not False)
# Paso 1: not False = True
# Paso 2: False and True = False
# Paso 3: True or False = True
# Resultado: True
```

---

## 📝 Actividad 3: Operadores Lógicos

**Instrucciones:** Evalúa las siguientes expresiones booleanas.

Sean: `a = True`, `b = False`, `c = True`

| # | Expresión | Tu respuesta |
|:---:|:-----------|:------------:|
| 1 | `a and b` | |
| 2 | `a or b` | |
| 3 | `not b` | |
| 4 | `a and not b` | |
| 5 | `not a or b` | |
| 6 | `a and b or c` | |
| 7 | `not (a and b)` | |
| 8 | `a or b or not c` | |

<details>
<summary>✅ Ver respuestas - Actividad 3</summary>

Sean: `a = True`, `b = False`, `c = True`

| # | Expresión | Respuesta |
|:---:|:-----------|:---------:|
| 1 | `a and b` | **False** |
| 2 | `a or b` | **True** |
| 3 | `not b` | **True** |
| 4 | `a and not b` | **True** |
| 5 | `not a or b` | **False** |
| 6 | `a and b or c` | **True** |
| 7 | `not (a and b)` | **True** |
| 8 | `a or b or not c` | **True** |

</details>

---

## 4. Traducción de Condiciones Reales a Expresiones Lógicas

Esta es una skill fundamental: convertir situaciones de la vida real en código que la computadora pueda entender.

### 4.1 Pasos para la Traducción

1. **Identificar las condiciones** que deben cumplirse
2. **Determinar los operadores** necesarios (relacionales y lógicos)
3. **Construir la expresión** combinándolas

### 4.2 Ejemplos Resueltos

| Situación Real | Expresión Lógica | Explicación |
|---------------|------------------|-------------|
| "Un estudiante pasa si tiene nota >= 60" | `nota >= 60` | Condición simple |
| "Es mayor de edad y tiene identificación" | `edad >= 18 and tiene_id` | Ambas necesarias |
| "Puedo ir al cine si tengo dinero o mis papás me pagan" | `tengo_dinero or me_pagan` | Al menos una |
| "No está lloviendo y no hay tormenta" | `not esta_lloviendo and not hay_tormenta` | Equivale a `not (lloviendo or tormenta)` |
| "La edad está entre 13 y 19 años" | `edad >= 13 and edad <= 19` | Rango válido |

### 4.3 Casos Complejos

**Situación:** "Un adolescente puede crear una cuenta en una red social si tiene 13 años o más, y sus padres lo permiten o tiene correo electrónico verificado."

```python
edad = 15
padres_permiten = False
email_verificado = True

puede_crear_cuenta = edad >= 13 and (padres_permiten or email_verificado)
# Paso 1: edad >= 13 → True
# Paso 2: padres_permiten or email_verificado → False or True → True
# Paso 3: True and True → True
# Resultado: True (puede crear cuenta)
```

---

## 📝 Actividad 4: Traducción de Condiciones

**Instrucciones:** Convierte cada situación en una expresión lógica válida.

**Contexto:** Crea las variables que consideres necesarias.

| # | Situación | Tu expresión lógica |
|:---:|:-----------|:---------------------|
| 1 | "Un joven puede conducir si tiene 18 años o más" | |
| 2 | "El clima está bueno si no llueve y no hay viento" | |
| 3 | "Puedes entrar al espectáculo si tienes boleto Y (eres mayor O un adulto te acompaña)" | |
| 4 | "La nota es excelente si es >= 90" | |
| 5 | "El número es divisible por 3 Y por 5" | |

---

## 5. Estructuras de Control

Las estructuras de control permiten que un programa tome decisiones y repita acciones basándose en condiciones booleanas.

### 5.1 Estructura Condicional (if/else)

La estructura `if` ejecuta código solo cuando una condición es verdadera.

```python
edad = 16

if edad >= 18:
    print("Eres mayor de edad")
    print("Puedes votar")
else:
    print("Eres menor de edad")
    print("No puedes votar todavía")
```

### if/elif/else (múltiples condiciones)

```python
nota = 85

if nota >= 90:
    print("Excelente")
elif nota >= 80:
    print("Muy bueno")
elif nota >= 70:
    print("Bueno")
elif nota >= 60:
    print("Aprobado")
else:
    print("Reprobado")
```

### 5.2 Estructura Repetitiva (while)

Repite código mientras una condición sea verdadera.

```python
# Contar del 1 al 5
contador = 1

while contador <= 5:
    print(contador)
    contador = contador + 1  # o contador += 1

print("¡Terminó el conteo!")
```

### 5.3 Estructura Repetitiva (for)

Itera sobre una secuencia de valores.

```python
# Iterar sobre una lista
frutas = ["manzana", "banana", "cereza"]

for fruta in frutas:
    print(f"Me gusta la {fruta}")

# Iterar con range
for i in range(1, 6):
    print(f" número {i}")
```

### 5.4 Break y Continue

```python
# Break: salir del ciclo
for i in range(10):
    if i == 5:
        break  # Sale cuando i es 5
    print(i)

# Continue: saltarse una iteración
for i in range(5):
    if i == 2:
        continue  # Saltar cuando i es 2
    print(i)  # Imprime 0, 1, 3, 4
```

---

## 📝 Actividad 5: Estructuras de Control

**Instrucciones:** Escribe el código para cada situación.

### Ejercicio A: Clasificador de edad

```python
# Escribe un programa que clasifique la edad:
# 0-12: Niño
# 13-19: Adolescente
# 20-59: Adulto
# 60+: Adulto mayor
```

### Ejercicio B: Tabla de multiplicar

```python
# Escribe un programa que muestre la tabla de multiplicar del 5
# Usando un ciclo for
```

### Ejercicio C: Adivina el número

```python
# Crea un juego donde el usuario debe adivinar un número
# Usa un ciclo while con una condición de terminación
```

---

## ☕ DESCANSO - 15 minutos

**Hora: Transcurridos ~195 minutos**

¡Excelente progreso! Has cubierto casi todo el material. Este segundo descanso es ideal para:

- 🧠 Procesar lo aprendido
- 💬 Discutir dudas con compañeros
- 🚶 Moverse un poco

Volveremos para los ejercicios finales y la resolución guiada.

---

# 📅 Sesión 3: Práctica y Resolución de Ejercicios

## ⏱️ Tiempo estimado: 30 minutos

---

## 6. Análisis de Sentencias Lógicas en Lenguaje Natural

Esta actividad desarrolla tu capacidad de leer descripciones verbales y convertirlas en lógica de programación.

### 6.1 Ejercicios de Análisis

**Instrucciones:** Para cada sentencia, identifica:
1. Las condiciones involucradas
2. Los operadores necesarios
3. La expresión lógica final

| # | Sentencia | Condiciones | Operadores | Expresión |
|:---:|:-----------|:-------------|:------------:|:---------:|
| 1 | "Puedes ir a la fiesta si tienes 16 años o más, O si tus padres te dan permiso" | edad >= 18, padres_permiten | `or` | `edad >= 18 or padres_permiten` |
| 2 | "El examen está aprobado si sacaste al menos 60 Y entregaste a tiempo" | nota >= 60, entregado_a_tiempo | `and` | `nota >= 60 and entregado_a_tiempo` |
| 3 | "No puedes entrar si eres menor de 18 Y no tienes identificación" | edad < 18, tiene_id | `and` + `not` | `not (edad >= 18 or tiene_id)` |
| 4 | "El año es bisiesto si es divisible por 4 Y (no es divisible por 100 O es divisible por 400)" | divisible_4, divisible_100, divisible_400 | `and` + `or` | `(anio % 4 == 0) and (anio % 100 != 0 or anio % 400 == 0)` |

<details>
<summary>✅ Ver respuestas - Actividad 6.1</summary>

| # | Expresión Lógica |
|:---|:------------------|
| 1 | `edad >= 18 or padres_permiten` |
| 2 | `nota >= 60 and entregado_a_tiempo` |
| 3 | `edad < 18 and not tiene_id` o `not (edad >= 18 or tiene_id)` |
| 4 | `(anio % 4 == 0) and (anio % 100 != 0 or anio % 400 == 0)` |

</details>

### 6.2 Análisis Detallado

**Ejercicio 4 resuelto:**

Un año es bisiesto cuando:
- Es divisible por 4 **Y**
- No es divisible por 100, **O** es divisible por 400

```python
anio = 2024

es_bisiesto = (anio % 4 == 0) and (anio % 100 != 0 or anio % 400 == 0)

print(f"{anio} es bisiesto: {es_bisiesto}")
```

---

## 7. Ejercicios de Resolución con Acompañamiento

A continuación, resuelvan juntos estos ejercicios. Lee cada problema, discute la solución, y luego escribe el código.

### Ejercicio 1: Calculadora de IMC con Interpretación

```python
"""
Crea un programa que:
1. Pida al usuario su peso (kg) y altura (m)
2. Calcule el IMC = peso / altura²
3. Clasifique:
   - IMC < 18.5: Bajo peso
   - 18.5 <= IMC < 25: Normal
   - 25 <= IMC < 30: Sobrepeso
   - IMC >= 30: Obesidad
"""

# Solución guiada
peso = float(input("Ingresa tu peso en kg: "))
altura = float(input("Ingresa tu altura en metros: "))

imc = peso / (altura ** 2)

if imc < 18.5:
    clasificacion = "Bajo peso"
elif imc < 25:
    clasificacion = "Normal"
elif imc < 30:
    clasificacion = "Sobrepeso"
else:
    clasificacion = "Obesidad"

print(f"Tu IMC es: {imc:.2f}")
print(f"Clasificación: {clasificacion}")
```

### Ejercicio 2: Sistema de Login

```python
"""
Crea un sistema de login que:
1. Tenga un usuario y contraseña predefinidos
2. Pida usuario y contraseña
3. Verifique las credenciales
4. Muestre mensaje de éxito o error
"""

usuario_correcto = "jovenprogramador"
contrasena_correcta = "python123"

usuario = input("Usuario: ")
contrasena = input("Contraseña: ")

if usuario == usuario_correcto and contrasena == contrasena_correcta:
    print("✅ Login exitoso")
elif usuario != usuario_correcto:
    print("❌ Usuario incorrecto")
else:
    print("❌ Contraseña incorrecta")
```

### Ejercicio 3: Juego de Adivinanza

```python
"""
Crea un juego donde:
1. La computadora elige un número aleatorio del 1 al 100
2. El usuario intenta adivinar
3. Se da pistas de "mayor" o "menor"
4. Se cuenta los intentos
"""

import random

numero_secreto = random.randint(1, 100)
intentos = 0
adivinado = False

print("¡Adivina el número entre 1 y 100!")

while not adivinado:
    intento = int(input("Tu intento: "))
    intentos += 1
    
    if intento == numero_secreto:
        adivinado = True
        print(f"🎉 ¡Correcto! Lo adivinaste en {intentos} intentos")
    elif intento < numero_secreto:
        print("El número es mayor")
    else:
        print("El número es menor")
```

---

## 📝 Actividad Final: Proyecto Integrador

**Instrucciones:** Combina todos los conceptos aprendidos para crear un pequeño programa.

### Requisitos del Programa

Crea una "Calculadora de Actividades según el clima" que:

1. **Pida la temperatura actual** (número)
2. **Pida si está lloviendo** (si/no)
3. **Use expresiones lógicas** para recomendar actividades:

| Condición | Actividad recomendada |
|:----------|:---------------------|
| Temperatura > 30 y no llueve | **"Ve a la playa"** |
| Temperatura entre 15-30 y no llueve | **"Sal a caminar"** |
| Temperatura < 15 y no llueve | **"Practica deporte en interior"** |
| Está lloviendo | **"Lee un libro o mira películas"** |

### Plantilla

```python
# Variables de entrada
temperatura = float(input("Temperatura actual: "))
llueve_input = input("¿Está lloviendo? (si/no): ")
llueve = llueve_input.lower() == "si"

# Tu código aquí
# Usa if, elif, else y operadores lógicos
```

---

## 📊 Resumen de Conceptos

### Operadores Aritméticos
```
+  -  *  /  %  **
```

### Operadores Relacionales
```
==  !=  >  <  >=  <=
```

### Operadores Lógicos
```
and   or   not
```

### Estructuras de Control
```python
if condición:
    # código

if condición:
    # código
else:
    # código

while condición:
    # código

for variable in secuencia:
    # código
```

---

## 🔬 Autoevaluación

Responde estas preguntas para verificar tu comprensión:

| # | Pregunta | Tu respuesta |
|:---:|:----------|:---------------:|
| 1 | ¿Cuál es el resultado de `10 + 5 * 2`? | |
| 2 | ¿Qué operador usas para verificar si dos valores son iguales? | |
| 3 | ¿Cuál es el resultado de `True and False`? | |
| 4 | ¿Qué estructura usas para repetir código mientras una condición sea verdadera? | |
| 5 | ¿Cómo traduces "tienes 15 años O tus padres permiten"? | |
| 6 | ¿Qué valor produce `not (True or False)`? | |

<details>
<summary>✅ Respuestas - Autoevaluación</summary>

| # | Pregunta | Respuesta |
|:---:|:----------|:---------------:|
| 1 | ¿Cuál es el resultado de `10 + 5 * 2`? | **20** (porque 5*2=10, luego 10+10=20) |
| 2 | ¿Qué operador usas para verificar si dos valores son iguales? | **`==`** |
| 3 | ¿Cuál es el resultado de `True and False`? | **False** |
| 4 | ¿Qué estructura usas para repetir código mientras una condición sea verdadera? | **while** |
| 5 | ¿Cómo traduces "tienes 15 años O tus padres permiten"? | `edad >= 15 or padres_permiten` |
| 6 | ¿Qué valor produce `not (True or False)`? | **False** (porque True or False = True, y not True = False) |
| 7 | ¿Qué estructura usarías para dar una de varias opciones según una nota? | **if/elif/else** |

</details>
| 7 | ¿Qué estructura usarías para dar una de varias opciones según una nota? | |

---

## 📚 Recursos Adicionales

### Práctica Online
- [Programiz - Python Operators](https://www.programiz.com/python-programming/operators)
- [W3Schools - Python Conditions](https://www.w3schools.com/python/python_conditions.asp)

### Ejercicios Extra
1. Crea un convertidor de temperatura (Celsius a Fahrenheit)
2. Haz un programa que determine si un número es par o impar
3. Crea un generador de contraseñas simple
4. Desarrolla una calculadora básica (+, -, *, /)

---

## ✅ Conclusión

¡Felicitaciones! Has completado el material de estudio. Ahora dominas:

- ✅ Expresiones aritméticas y su orden de operaciones
- ✅ Operadores relacionales para comparar valores
- ✅ Lógica booleana (and, or, not)
- ✅ Estructuras de control condicionales (if/elif/else)
- ✅ Estructuras de control repetitivas (while, for)
- ✅ Traducción de condiciones reales a código

Estos conceptos son la base de la programación. Continúa practicando y pronto podrás crear programas más complejos.

**Recuerda:** La programación es como un músculo: mientras más practiques, más fuerte serás.

---

*Material creado para el curso de programación autoguiado*  
*Última actualización: 2026*
