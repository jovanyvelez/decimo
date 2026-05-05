# Guía de Estudio: Subprogramas en PSeInt

> **Duración estimada:** 3 horas  
> **Nivel:** Jóvenes de 15 a 17 años  
> **Software:** PSeInt

---

## Tabla de Contenidos

1. [¿Qué son los subprogramas?](#1-qué-son-los-subprogramas)
2. [Modularidad y reutilización de código](#2-modularidad-y-reutilización-de-código)
3. [Procedimientos](#3-procedimientos)
4. [Funciones](#4-funciones)
5. [Parámetros y argumentos](#5-parámetros-y-argumentos)
6. [Ejercicios prácticos](#6-ejercicios-prácticos)
7. [Autoevaluación](#7-autoevaluación)

---

## 1. ¿Qué son los subprogramas?

### Concepto

Un **subprograma** (también llamado subrutina, submódulo o subalgoritmo) es un bloque de código que realiza una tarea específica y puede ser llamado desde cualquier parte del programa principal.

Piensa en un subprograma como una "mini-receta" dentro de un libro de cocina más grande. En lugar de escribir la misma receta una y otra vez cada vez que la necesitas, simplemente haces referencia a ella por su nombre.

### Analogía: La orquesta

Imagina una orquesta sinfónica. El director (programa principal) no toca cada instrumento nota por nota. En cambio, divide la sinfonía en secciones:

- Sección de cuerdas
- Sección de vientos
- Sección de percusión

Cada sección tiene su propia partitura (**subprograma**) y el director las coordina. Si el compositor cambia la melodía de los violines, solo modifica la partitura de cuerdas, no toda la sinfonía.

```pseint
// Programa principal
Algoritmo Orquesta
    Escribir "Inicia la sinfonía"
    SeccionCuerdas
    SeccionVientos
    SeccionPercusion
    Escribir "Fin de la sinfonía"
FinAlgoritmo
```

---

## 2. Modularidad y reutilización de código

### ¿Qué es la modularidad?

La **modularidad** consiste en dividir un programa grande en partes más pequeñas, llamadas módulos. Cada módulo se encarga de una tarea concreta.

#### Ventajas de la modularidad

| Ventaja | Explicación |
|---------|-------------|
| **Claridad** | El código es más fácil de leer y entender |
| **Mantenimiento** | Si hay un error, solo debes buscar en el módulo correspondiente |
| **Colaboración** | Varios programadores pueden trabajar en módulos distintos al mismo tiempo |
| **Reutilización** | Un módulo bien diseñado puede usarse en múltiples programas |

### ¿Qué es la reutilización de código?

La **reutilización** significa escribir código una sola vez y usarlo muchas veces. En lugar de copiar y pegar el mismo bloque de instrucciones, creas un subprograma y lo invocas cada vez que lo necesitas.

#### Ejemplo sin subprogramas (código repetido)

```pseint
Algoritmo SinReutilizacion
    // Calcular área de un círculo con radio 5
    area1 <- 3.1416 * 5 * 5
    Escribir "Área del círculo 1: ", area1

    // Calcular área de un círculo con radio 10
    area2 <- 3.1416 * 10 * 10
    Escribir "Área del círculo 2: ", area2

    // Calcular área de un círculo con radio 15
    area3 <- 3.1416 * 15 * 15
    Escribir "Área del círculo 3: ", area3
FinAlgoritmo
```

#### Ejemplo con subprogramas (código reutilizado)

```pseint
Algoritmo ConReutilizacion
    Escribir "Área del círculo 1: ", CalcularAreaCirculo(5)
    Escribir "Área del círculo 2: ", CalcularAreaCirculo(10)
    Escribir "Área del círculo 3: ", CalcularAreaCirculo(15)
FinAlgoritmo

Funcion resultado <- CalcularAreaCirculo(radio)
    Definir resultado Como Real
    resultado <- 3.1416 * radio * radio
FinFuncion
```

> **Reflexiona:** ¿Qué versión es más corta? ¿Cuál sería más fácil de modificar si cambia la fórmula del área?

---

## 3. Procedimientos

### Definición

Un **procedimiento** es un subprograma que ejecuta una tarea pero **no devuelve ningún valor** al programa que lo llamó. Su propósito es producir un efecto o resultado visible (como mostrar algo en pantalla o modificar datos).

### Sintaxis en PSeInt

```pseint
SubProceso NombreDelProcedimiento ( parametro1, parametro2, ... )
    // Instrucciones del procedimiento
    // ...
FinSubProceso
```

### Ejemplo 1: Mostrar un menú de opciones

```pseint
Algoritmo CalculadoraSimple
    Definir opcion Como Entero
    MostrarMenu
    Escribir "Elija una opción: "
    Leer opcion
FinAlgoritmo

SubProceso MostrarMenu
    Escribir "===== CALCULADORA ====="
    Escribir "1. Sumar"
    Escribir "2. Restar"
    Escribir "3. Multiplicar"
    Escribir "4. Dividir"
    Escribir "======================="
FinSubProceso
```

### Ejemplo 2: Dibujar una línea de separación reutilizable

```pseint
Algoritmo ConversorTemperatura
    DibujarLinea
    Escribir "Conversor de °C a °F"
    DibujarLinea
    Definir celsius, fahrenheit Como Real
    Escribir "Ingrese grados Celsius: "
    Leer celsius
    fahrenheit <- (celsius * 9/5) + 32
    Escribir "Equivalente en Fahrenheit: ", fahrenheit
    DibujarLinea
FinAlgoritmo

SubProceso DibujarLinea
    Escribir "----------------------------------------"
FinSubProceso
```

### Diferencia clave: Procedimiento vs. Función

| Característica | Procedimiento | Función |
|----------------|--------------|---------|
| ¿Devuelve un valor? | No | Sí |
| ¿Cómo se invoca? | Por su nombre, como una orden | Asignándola a una variable o dentro de una expresión |
| Uso típico | Mostrar datos, modificar variables | Cálculos matemáticos, validaciones |

---

## 4. Funciones

### Definición

Una **función** es un subprograma que realiza una tarea y **devuelve un valor** al programa que la invocó.

### Sintaxis en PSeInt

```pseint
Funcion variable_de_retorno <- NombreDeLaFuncion ( parametro1, parametro2, ... )
    Definir variable_de_retorno Como TipoDeDato
    // Instrucciones de la función
    // ...
FinFuncion
```

### Ejemplo 1: Función que calcula el cuadrado de un número

```pseint
Algoritmo PruebaCuadrado
    Definir num, resultado Como Entero
    Escribir "Ingrese un número: "
    Leer num
    resultado <- CalcularCuadrado(num)
    Escribir "El cuadrado de ", num, " es: ", resultado
FinAlgoritmo

Funcion cuadrado <- CalcularCuadrado(n)
    Definir cuadrado Como Entero
    cuadrado <- n * n
FinFuncion
```

### Ejemplo 2: Función que determina si un número es par

```pseint
Algoritmo VerificarParidad
    Definir n Como Entero
    Escribir "Ingrese un número: "
    Leer n

    Si EsPar(n) Entonces
        Escribir n, " es par"
    SiNo
        Escribir n, " es impar"
    FinSi
FinAlgoritmo

Funcion resultado <- EsPar(numero)
    Definir resultado Como Logico
    Si numero MOD 2 = 0 Entonces
        resultado <- Verdadero
    SiNo
        resultado <- Falso
    FinSi
FinFuncion
```

### Ejemplo 3: Función que calcula el promedio de tres notas

```pseint
Algoritmo CalculoPromedio
    Definir nota1, nota2, nota3, promedio Como Real
    Escribir "Ingrese las tres notas:"
    Leer nota1, nota2, nota3
    promedio <- PromedioNotas(nota1, nota2, nota3)
    Escribir "El promedio es: ", promedio

    Si promedio >= 3.0 Entonces
        Escribir "APROBADO"
    SiNo
        Escribir "REPROBADO"
    FinSi
FinAlgoritmo

Funcion prom <- PromedioNotas(n1, n2, n3)
    Definir prom Como Real
    prom <- (n1 + n2 + n3) / 3
FinFuncion
```

---

## 5. Parámetros y argumentos

### Conceptos clave

- **Parámetros:** Son las variables que aparecen en la *definición* del subprograma. Funcionan como "huecos" o "espacios a rellenar".
- **Argumentos:** Son los valores reales que se pasan al subprograma en el momento de *invocarlo*.

### Analogía: La licuadora

```
Parámetros = El vaso de la licuadora (el espacio donde van los ingredientes)
Argumentos = Los ingredientes reales (fresas, leche, azúcar)
```

Puedes usar la misma licuadora (subprograma) con diferentes ingredientes (argumentos) para hacer batidos distintos.

### Tipos de paso de parámetros en PSeInt

| Tipo | Palabra clave | ¿Qué pasa? |
|------|--------------|------------|
| **Por valor** | (por defecto) | Se envía una copia. El original no cambia. |
| **Por referencia** | `Por Referencia` | Se envía la variable original. Los cambios la afectan. |

### Ejemplo: Paso por valor

El subprograma recibe una **copia** del valor. El valor original no se modifica.

```pseint
Algoritmo EjemploPorValor
    Definir miNumero Como Entero
    miNumero <- 10
    Escribir "Antes de llamar: ", miNumero   // Muestra 10
    DuplicarPorValor(miNumero)
    Escribir "Después de llamar: ", miNumero // Muestra 10 (no cambió)
FinAlgoritmo

SubProceso DuplicarPorValor(n)
    n <- n * 2
    Escribir "Dentro del subproceso: ", n    // Muestra 20
FinSubProceso
```

### Ejemplo: Paso por referencia

El subprograma recibe la **variable original**. Los cambios se conservan.

```pseint
Algoritmo EjemploPorReferencia
    Definir miNumero Como Entero
    miNumero <- 10
    Escribir "Antes de llamar: ", miNumero    // Muestra 10
    DuplicarPorReferencia(miNumero)
    Escribir "Después de llamar: ", miNumero  // Muestra 20 (cambió)
FinAlgoritmo

SubProceso DuplicarPorReferencia(n Por Referencia)
    n <- n * 2
    Escribir "Dentro del subproceso: ", n     // Muestra 20
FinSubProceso
```

> **Regla práctica:** Usa paso **por valor** cuando solo necesites el dato para un cálculo. Usa paso **por referencia** cuando necesites modificar la variable original.

---

## 6. Ejercicios prácticos

> **Instrucciones:** Resuelve los siguientes ejercicios en PSeInt. Cada sección indica el tiempo sugerido. ¡No pases al siguiente nivel sin haber entendido el anterior!

---

### Nivel 1: Calentamiento (30 minutos)

#### Ejercicio 1.1 — Saludo personalizado
Crea un procedimiento llamado `Saludar` que reciba un nombre como parámetro y muestre: _"¡Hola, [nombre]! Bienvenido/a a la programación modular."_

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo PruebaSaludo
    Definir nombre Como Caracter
    Escribir "¿Cómo te llamas?"
    Leer nombre
    Saludar(nombre)
FinAlgoritmo

SubProceso Saludar(nombre)
    Escribir "¡Hola, ", nombre, "! Bienvenido/a a la programación modular."
FinSubProceso
```
</details>

#### Ejercicio 1.2 — Suma de dos números (función)
Crea una función llamada `Sumar` que reciba dos números y devuelva su suma.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo PruebaSuma
    Definir a, b Como Real
    Escribir "Ingrese el primer número: "
    Leer a
    Escribir "Ingrese el segundo número: "
    Leer b
    Escribir "La suma es: ", Sumar(a, b)
FinAlgoritmo

Funcion resultado <- Sumar(x, y)
    Definir resultado Como Real
    resultado <- x + y
FinFuncion
```
</details>

#### Ejercicio 1.3 — ¿Es mayor de edad? (función lógica)
Crea una función llamada `EsMayorDeEdad` que reciba una edad y devuelva `Verdadero` si es mayor o igual a 18, o `Falso` en caso contrario.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo VerificarEdad
    Definir edad Como Entero
    Escribir "Ingrese su edad: "
    Leer edad

    Si EsMayorDeEdad(edad) Entonces
        Escribir "Eres mayor de edad."
    SiNo
        Escribir "Eres menor de edad."
    FinSi
FinAlgoritmo

Funcion resultado <- EsMayorDeEdad(e)
    Definir resultado Como Logico
    resultado <- e >= 18
FinFuncion
```
</details>

---

### Nivel 2: Afianzando conceptos (45 minutos)

#### Ejercicio 2.1 — Área y perímetro de un rectángulo
Crea dos funciones: `CalcularArea` y `CalcularPerimetro`. Cada una recibe la base y la altura de un rectángulo y devuelve el valor correspondiente.

Fórmulas:
- Área = base × altura
- Perímetro = 2 × (base + altura)

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo GeometriaRectangulo
    Definir base, altura Como Real
    Escribir "Ingrese la base del rectángulo: "
    Leer base
    Escribir "Ingrese la altura del rectángulo: "
    Leer altura

    Escribir "Área: ", CalcularArea(base, altura)
    Escribir "Perímetro: ", CalcularPerimetro(base, altura)
FinAlgoritmo

Funcion area <- CalcularArea(b, h)
    Definir area Como Real
    area <- b * h
FinFuncion

Funcion perimetro <- CalcularPerimetro(b, h)
    Definir perimetro Como Real
    perimetro <- 2 * (b + h)
FinFuncion
```
</details>

#### Ejercicio 2.2 — Conversor de monedas
Crea tres funciones que conviertan una cantidad en pesos colombianos (COP) a:
1. Dólares estadounidenses (USD) → tasa: 1 USD = 3,900 COP
2. Euros (EUR) → tasa: 1 EUR = 4,200 COP
3. Bolívares venezolanos (VES) → tasa: 1 VES = 0.11 COP

Cada función debe recibir la cantidad en pesos y devolver la cantidad convertida.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo ConversorMonedas
    Definir pesos Como Real
    Definir opcion Como Entero

    Escribir "Ingrese la cantidad en pesos colombianos: "
    Leer pesos

    Escribir "Convertir a:"
    Escribir "1. Dólares (USD)"
    Escribir "2. Euros (EUR)"
    Escribir "3. Bolívares (VES)"
    Leer opcion

    Segun opcion Hacer
        1: Escribir pesos, " COP = ", PesosADolar(pesos), " USD"
        2: Escribir pesos, " COP = ", PesosAEuro(pesos), " EUR"
        3: Escribir pesos, " COP = ", PesosABolivar(pesos), " VES"
        De Otro Modo:
            Escribir "Opción inválida"
    FinSegun
FinAlgoritmo

Funcion usd <- PesosADolar(p)
    Definir usd Como Real
    usd <- p / 3900
FinFuncion

Funcion eur <- PesosAEuro(p)
    Definir eur Como Real
    eur <- p / 4200
FinFuncion

Funcion ves <- PesosABolivar(p)
    Definir ves Como Real
    ves <- p / 0.11
FinFuncion
```
</details>

#### Ejercicio 2.3 — Intercambiar valores (por referencia)
Crea un procedimiento `Intercambiar` que reciba dos variables por referencia e intercambie sus valores. Luego, desde el programa principal, ingresa dos números y muestra el resultado del intercambio.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo PruebaIntercambio
    Definir a, b Como Entero
    Escribir "Ingrese el valor de A: "
    Leer a
    Escribir "Ingrese el valor de B: "
    Leer b

    Escribir "Antes del intercambio: A = ", a, ", B = ", b
    Intercambiar(a, b)
    Escribir "Después del intercambio: A = ", a, ", B = ", b
FinAlgoritmo

SubProceso Intercambiar(x Por Referencia, y Por Referencia)
    Definir temporal Como Entero
    temporal <- x
    x <- y
    y <- temporal
FinSubProceso
```
</details>

---

### Nivel 3: Integración (45 minutos)

#### Ejercicio 3.1 — Calculadora modular
Construye una calculadora completa usando subprogramas. Debe incluir:
- Procedimiento `MostrarMenuOpciones` para mostrar el menú
- Funciones `Sumar`, `Restar`, `Multiplicar` y `Dividir`
- El programa debe seguir corriendo hasta que el usuario elija la opción "Salir"

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo CalculadoraModular
    Definir opcion Como Entero
    Definir a, b Como Real

    Repetir
        MostrarMenuOpciones
        Leer opcion

        Si opcion >= 1 Y opcion <= 4 Entonces
            Escribir "Ingrese el primer número: "
            Leer a
            Escribir "Ingrese el segundo número: "
            Leer b
        FinSi

        Segun opcion Hacer
            1: Escribir "Resultado: ", Sumar(a, b)
            2: Escribir "Resultado: ", Restar(a, b)
            3: Escribir "Resultado: ", Multiplicar(a, b)
            4: Escribir "Resultado: ", Dividir(a, b)
            5: Escribir "¡Hasta luego!"
            De Otro Modo:
                Escribir "Opción no válida. Intente de nuevo."
        FinSegun

        Escribir ""
    Hasta Que opcion = 5
FinAlgoritmo

SubProceso MostrarMenuOpciones
    Escribir "===== CALCULADORA MODULAR ====="
    Escribir "1. Sumar"
    Escribir "2. Restar"
    Escribir "3. Multiplicar"
    Escribir "4. Dividir"
    Escribir "5. Salir"
    Escribir "==============================="
    Escribir "Elija una opción: "
FinSubProceso

Funcion r <- Sumar(x, y)
    Definir r Como Real
    r <- x + y
FinFuncion

Funcion r <- Restar(x, y)
    Definir r Como Real
    r <- x - y
FinFuncion

Funcion r <- Multiplicar(x, y)
    Definir r Como Real
    r <- x * y
FinFuncion

Funcion r <- Dividir(x, y)
    Definir r Como Real
    Si y = 0 Entonces
        Escribir "Error: No se puede dividir por cero."
        r <- 0
    SiNo
        r <- x / y
    FinSi
FinFuncion
```
</details>

#### Ejercicio 3.2 — Juego: Adivina el número
Crea un juego en el que la computadora genera un número aleatorio entre 1 y 100, y el jugador debe adivinarlo. Usa:
- Función `GenerarNumeroSecreto` para crear el número aleatorio
- Procedimiento `DarPista` que reciba el intento y el número secreto y diga si es "muy alto" o "muy bajo"
- El programa cuenta los intentos y felicita al jugador al final

> **Nota:** En PSeInt, `azar(n)` genera un número aleatorio entre 1 y n.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo AdivinaElNumero
    Definir secreto, intento, contador Como Entero

    secreto <- GenerarNumeroSecreto(100)
    contador <- 0

    Escribir "¡Adivina el número entre 1 y 100!"

    Repetir
        contador <- contador + 1
        Escribir "Intento ", contador, ": "
        Leer intento

        Si intento <> secreto Entonces
            DarPista(intento, secreto)
        FinSi
    Hasta Que intento = secreto

    Escribir "¡Felicidades! Adivinaste en ", contador, " intentos."
FinAlgoritmo

Funcion num <- GenerarNumeroSecreto(maximo)
    Definir num Como Entero
    num <- azar(maximo)
FinFuncion

SubProceso DarPista(intento, secreto)
    Si intento > secreto Entonces
        Escribir "El número es más BAJO. Intenta de nuevo."
    SiNo
        Escribir "El número es más ALTO. Intenta de nuevo."
    FinSi
FinSubProceso
```
</details>

---

### Nivel 4: Desafío (30 minutos)

#### Ejercicio 4.1 — Sistema de calificaciones
Diseña un programa modular que:
1. Reciba el número de estudiantes
2. Para cada estudiante, reciba 3 notas
3. Use una función `CalcularDefinitiva` que calcule el promedio de las 3 notas
4. Use una función `ObtenerConcepto` que devuelva una cadena:
   - "Excelente" si la nota ≥ 4.5
   - "Bueno" si la nota ≥ 3.5
   - "Aceptable" si la nota ≥ 3.0
   - "Insuficiente" si la nota < 3.0
5. Use un procedimiento `MostrarResumen` que reciba nombre, definitiva y concepto, y muestre todo en pantalla
6. Al final, muestre cuántos estudiantes aprobaron y cuántos reprobaron

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo SistemaCalificaciones
    Definir n, i, aprobados, reprobados Como Entero
    Definir nombre, concepto Como Caracter
    Definir n1, n2, n3, definitiva Como Real

    aprobados <- 0
    reprobados <- 0

    Escribir "¿Cuántos estudiantes va a procesar?"
    Leer n

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir ""
        Escribir "--- Estudiante ", i, " ---"
        Escribir "Nombre: "
        Leer nombre
        Escribir "Nota 1: "
        Leer n1
        Escribir "Nota 2: "
        Leer n2
        Escribir "Nota 3: "
        Leer n3

        definitiva <- CalcularDefinitiva(n1, n2, n3)
        concepto <- ObtenerConcepto(definitiva)
        MostrarResumen(nombre, definitiva, concepto)

        Si definitiva >= 3.0 Entonces
            aprobados <- aprobados + 1
        SiNo
            reprobados <- reprobados + 1
        FinSi
    FinPara

    Escribir ""
    Escribir "===== RESUMEN FINAL ====="
    Escribir "Aprobados: ", aprobados
    Escribir "Reprobados: ", reprobados
FinAlgoritmo

Funcion prom <- CalcularDefinitiva(n1, n2, n3)
    Definir prom Como Real
    prom <- (n1 + n2 + n3) / 3
FinFuncion

Funcion c <- ObtenerConcepto(nota)
    Definir c Como Caracter
    Si nota >= 4.5 Entonces
        c <- "EXCELENTE"
    SiNo
        Si nota >= 3.5 Entonces
            c <- "BUENO"
        SiNo
            Si nota >= 3.0 Entonces
                c <- "ACEPTABLE"
            SiNo
                c <- "INSUFICIENTE"
            FinSi
        FinSi
    FinSi
FinFuncion

SubProceso MostrarResumen(nom, def, con)
    Escribir "-------------------------"
    Escribir "Estudiante: ", nom
    Escribir "Definitiva: ", def
    Escribir "Concepto:   ", con
    Escribir "-------------------------"
FinSubProceso
```
</details>

#### Ejercicio 4.2 — Validación de contraseña (función con lógica)
Crea una función `ValidarClave` que reciba una contraseña (cadena de texto) y verifique que cumpla con los siguientes requisitos:
- Tener al menos 8 caracteres
- Contener al menos una letra mayúscula
- Contener al menos un número

La función debe devolver `Verdadero` solo si se cumplen los tres requisitos.

> **Ayuda:** En PSeInt puedes usar las funciones `Longitud(cadena)`, `Mayusculas(cadena)`, `Minusculas(cadena)` y comparar subcadenas con `Subcadena(cadena, inicio, fin)`.

<details>
<summary>Ver solución</summary>

```pseint
Algoritmo ValidacionClave
    Definir clave Como Caracter
    Escribir "Cree una contraseña segura:"
    Leer clave

    Si ValidarClave(clave) Entonces
        Escribir "¡Contraseña válida!"
    SiNo
        Escribir "La contraseña NO cumple los requisitos:"
        Si Longitud(clave) < 8 Entonces
            Escribir "- Debe tener al menos 8 caracteres."
        FinSi
        Si NoTieneMayuscula(clave) Entonces
            Escribir "- Debe contener al menos una mayúscula."
        FinSi
        Si NoTieneNumero(clave) Entonces
            Escribir "- Debe contener al menos un número."
        FinSi
    FinSi
FinAlgoritmo

Funcion valida <- ValidarClave(c)
    Definir valida Como Logico
    Definir tieneLargo, tieneMayus, tieneNum Como Logico

    tieneLargo <- Longitud(c) >= 8
    tieneMayus <- c <> Minusculas(c)
    tieneNum <- ContieneNumero(c)

    valida <- tieneLargo Y tieneMayus Y tieneNum
FinFuncion

Funcion r <- ContieneNumero(c)
    Definir r Como Logico
    Definir i Como Entero
    Definir caracter Como Caracter
    r <- Falso

    Para i <- 1 Hasta Longitud(c) Con Paso 1 Hacer
        caracter <- Subcadena(c, i, i)
        Segun caracter Hacer
            "0","1","2","3","4","5","6","7","8","9":
                r <- Verdadero
        FinSegun
    FinPara
FinFuncion
```
</details>

---

## 7. Autoevaluación

Responde las siguientes preguntas para medir tu comprensión. Revisa las respuestas al final.

### Preguntas de selección múltiple

**1. ¿Cuál es la principal diferencia entre un procedimiento y una función?**

A. El procedimiento usa `Definir` y la función no.  
B. El procedimiento no devuelve un valor; la función sí.  
C. La función puede tener parámetros y el procedimiento no.  
D. No hay diferencia, son lo mismo.

**2. ¿Qué imprime el siguiente código?**

```pseint
Algoritmo Prueba
    Definir x Como Entero
    x <- 5
    Cambiar(x)
    Escribir x
FinAlgoritmo

SubProceso Cambiar(n Por Referencia)
    n <- n + 10
FinSubProceso
```

A. 5  
B. 10  
C. 15  
D. 0

**3. ¿Cuál es una ventaja de la modularidad?**

A. El código ocupa más espacio en disco.  
B. El programa se ejecuta más lento.  
C. Facilita encontrar y corregir errores.  
D. Hace que todas las variables sean globales.

**4. ¿Qué palabra clave se usa en PSeInt para pasar un parámetro por referencia?**

A. `Por Referencia`  
B. `Por Valor`  
C. `Referencia`  
D. `Global`

**5. Observa el siguiente código. ¿Qué valor se muestra?**

```pseint
Algoritmo Prueba2
    Definir a, b Como Entero
    a <- 5
    b <- 3
    Escribir Calcular(a, b)
FinAlgoritmo

Funcion r <- Calcular(x, y)
    Definir r Como Entero
    r <- (x + y) * 2
FinFuncion
```

A. 13  
B. 16  
C. 5  
D. 11

---

### Respuestas

<details>
<summary>Ver respuestas</summary>

1. **B** — La función devuelve un valor usando `FinFuncion`; el procedimiento no.
2. **C** — Al pasar `x` por referencia, el procedimiento modifica la variable original. `5 + 10 = 15`.
3. **C** — La modularidad permite aislar errores en módulos específicos, facilitando la depuración.
4. **A** — La sintaxis es `Por Referencia` después del nombre del parámetro.
5. **B** — `(5 + 3) * 2 = 16`.

</details>

---

## Resumen visual

```
┌─────────────────────────────────────────────────────┐
│                  PROGRAMA PRINCIPAL                  │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐       │
│  │ SubProceso│  │ SubProceso│  │  Función  │       │
│  │  (hacer)  │  │  (mostrar)│  │ (calcular)│       │
│  └───────────┘  └───────────┘  └─────┬─────┘       │
│                                       │              │
│                                  retorna valor       │
└─────────────────────────────────────────────────────┘
```

> **Recuerda:** Divide y vencerás. Un problema grande se resuelve más fácilmente cuando lo partes en problemas pequeños.

---

## Créditos

Material diseñado para estudiantes de grado décimo como introducción a la programación estructurada usando PSeInt.

---

*"Cualquier problema puede ser resuelto dividiéndolo en partes más pequeñas." — Principio de divide y vencerás*
