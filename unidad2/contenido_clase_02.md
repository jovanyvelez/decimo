# Tipos de Datos, Variables y Pseudocódigo

## Guía de Aprendizaje — Fundamentos de Programación

**Duración estimada:** 3 horas (180 minutos)
**Población:** Estudiantes de 10º grado (15-16 años)
**Modalidad:** Autoinstrucción con prácticas y evaluaciones integradas

---

## Tabla de Contenidos

1. [Información y Datos: Conceptos Fundamentales](#1-información-y-datos-conceptos-fundamentales)
2. [Clasificación de Tipos de Datos](#2-clasificación-de-tipos-de-datos)
3. [Campos y Registros: Organizando la Información](#3-campos-y-registros-organizando-la-información)
4. [Variables: Espacios con Nombre](#4-variables-espacios-con-nombre)
5. [Nombres, Declaraciones y Buenas Prácticas](#5-nombres-declaraciones-y-buenas-prácticas)
6. [Representación en Pseudocódigo](#6-representación-en-pseudocódigo)
7. [Práctica Dirigida: Declaración de Variables](#7-práctica-dirigida-declaración-de-variables)
8. [Quiz Final de Evaluación](#8-quiz-final-de-evaluación)
9. [Actividad Integradora](#9-actividad-integradora)

---

## 1. Información y Datos: Conceptos Fundamentales

### 1.1 ¿Qué es un dato?

Un **dato** es un hecho raw, sin contexto ni interpretación. Es un símbolo, un número, una letra que por sí sola no significa nada o que necesita ser procesada para adquirir sentido.

**Ejemplos de datos:**
- `17` → Solo un número, ¿edad? ¿nota? ¿cantidad?
- `"López"` → Solo un apellido
- `1.75` → Solo una medida, ¿altura? ¿peso?

### 1.2 ¿Qué es la información?

La **información** es un dato que ha sido **procesado, organizado o contextualizado** de manera que adquiere significado y utilidad para quien la recibe.

**El mismo dato, convertido en información:**

| Dato (Raw) | Contexto | Información |
|------------|----------|-------------|
| `17` | Edad de María | "María tiene 17 años" |
| `"López"` | Apellido del estudiante | "El estudiante López se registró" |
| `1.75` | Estatura en metros | "Juan mide 1.75 metros" |

### 1.3 La relación dato-información en sistemas

```
┌─────────┐    Procesamiento    ┌─────────────┐
│  DATOS  │ ──────────────────→ │ INFORMACIÓN │
│ (Input) │   (Transformación)  │  (Output)   │
└─────────┘                     └─────────────┘
```

**Ejemplo cotidiano:**

| Etapa | Descripción |
|-------|-------------|
| **Dato de entrada** | `150000`, `"Carlos"`, `85` |
| **Procesamiento** | Calcular descuento del 15% sobre 150000 |
| **Información de salida** | "Carlos, tu precio con descuento es 127.500" |

### 1.4 ¿Por qué importa esta distinción?

En programación, debes decidir:
- **Qué datos necesitas** capturar (entrada)
- **Cómo procesarlos** para convertirlos en información útil (proceso)
- **Cómo presentar** esa información al usuario (salida)

> **Recuerda:** El computador trabaja con datos. Tú diseñas algoritmos para transformar esos datos en información significativa.

---

## 2. Clasificación de Tipos de Datos

### 2.1 Tipos de Datos Primitivos

Los **tipos primitivos** son los bloques fundamentales que no pueden descomponerse en tipos más simples.

#### 2.1.1 Numéricos Enteros (int)

Representan números completos, sin parte decimal.

| Característica | Detalle |
|----------------|---------|
| **Qué almacena** | Números enteros: ..., -3, -2, -1, 0, 1, 2, 3, ... |
| **Rango típico** | -2.147.483.648 a 2.147.483.647 (32 bits) |
| **Ejemplos** | `42`, `-7`, `0`, `1000000`, `18` |
| **Usos comunes** | Edad, cantidad de artículos, año, número de hijos |

**Ejemplos en contexto:**
```
edad_estudiante = 16
cantidad_productos = 25
año_actual = 2026
```

#### 2.1.2 Numéricos Decimales (float / double)

Representan números con parte decimal (números reales).

| Característica | Detalle |
|----------------|---------|
| **Qué almacena** | Números con decimales: 3.14, -0.5, 99.9 |
| **Precisión** | Aproximada (no exacta para cálculos financieros) |
| **Ejemplos** | `3.14159`, `-0.5`, `98.6`, `1.75` |
| **Usos comunes** | Precios, estaturas, calificaciones, coordenadas |

> **Nota importante:** En programación se usa **punto (.)** para decimales, no coma.
> - Correcto: `3.5`
> - Incorrecto: `3,5`

**Ejemplos en contexto:**
```
precio_producto = 49990.99
estatura_juan = 1.73
promedio_clase = 8.7
temperatura = 36.5
```

#### 2.1.3 Texto / Cadenas de Caracteres (String)

Secuencias de caracteres que representan texto.

| Característica | Detalle |
|----------------|---------|
| **Qué almacena** | Letras, palabras, frases, combinaciones |
| **Delimitadores** | Comillas simples o dobles: `"texto"` o `'texto'` |
| **Ejemplos** | `"Hola"`, `'Ana'`, `"Calle 45 #12-30"`, `"123"` |
| **Usos comunes** | Nombres, direcciones, mensajes, códigos |

**Importante:** `"123"` **no es el número 123**, es texto. No puedes hacer operaciones matemáticas con él directamente.

**Ejemplos en contexto:**
```
nombre_cliente = "María González"
direccion = "Carrera 15 #45-30"
mensaje_bienvenida = "Bienvenido al sistema"
codigo_producto = "ABC-2026"
```

#### 2.1.4 Booleanos (bool)

Representan valores de lógica binaria: solo dos posibilidades.

| Característica | Detalle |
|----------------|---------|
| **Qué almacena** | Solo dos valores: verdadero o falso |
| **Valores posibles** | `True` / `False` (o `1` / `0` en algunos lenguajes) |
| **Ejemplos** | `True`, `False` |
| **Usos comunes** | Estados binarios, validaciones, condiciones |

**Ejemplos en contexto:**
```
es_mayor_de_edad = True
tiene_descuento = False
usuario_activo = True
contrasena_correcta = False
```

#### 2.1.5 Sin Valor (Null / None)

Representa la **ausencia intencional** de valor. No es lo mismo que cero ni que texto vacío.

| Característica | Detalle |
|----------------|---------|
| **Qué significa** | "No tiene ningún valor" |
| **Diferencia con vacío** | `""` es texto vacío; `null` es la ausencia de dato |
| **Ejemplos** | `null`, `None`, `NULL` |
| **Usos comunes** | Campos opcionales, datos pendientes, inicializaciones |

**Ejemplos en contexto:**
```
telefono_emergencia = None       // No proporcionó teléfono
fecha_nacimiento = None         // Dato pendiente por registrar
respuesta_encuesta = None       // Usuario no respondió
```

### 2.2 Tabla Resumen de Tipos Primitivos

| Tipo | Palabra clave | Ejemplos | Operaciones válidas |
|------|--------------|----------|---------------------|
| Entero | `int` | `42`, `-7`, `0`, `18` | `+`, `-`, `*`, `/`, `%`, comparaciones |
| Decimal | `float` | `3.14`, `1.5`, `99.9` | `+`, `-`, `*`, `/`, comparaciones |
| Texto | `str` | `"Hola"`, `'Ana'` | Concatenar, buscar, extraer |
| Booleano | `bool` | `True`, `False` | `and`, `or`, `not` |
| Sin valor | `null` | `None`, `null` | Comparar con null |

### 2.3 Tipos de Datos Compuestos (Introducción)

Los tipos compuestos se construyen combinando tipos primitivos.

#### 2.3.1 Arreglos (Arrays/Vectores)

Colección ordenada del mismo tipo de dato.

```
// Ejemplo: Lista de edades de 5 estudiantes
edades = [16, 17, 16, 18, 17]

// Ejemplo: Lista de nombres
nombres = ["Ana", "Carlos", "María", "Pedro"]
```

#### 2.3.2 Cadenas (Strings) — Ya vistas, pero son compuestas

Las cadenas son secuencias de caracteres, así que técnicamente son un tipo compuesto de caracteres.

```
nombre = "Juan"  // Secuencia de: 'J', 'u', 'a', 'n'
```

---

## 3. Campos y Registros: Organizando la Información

### 3.1 ¿Qué es un campo?

Un **campo** es un espacio de almacenamiento que tiene:
- Un **nombre** (identificador)
- Un **tipo de dato** (qué puede almacenar)
- Un **valor** (el dato actual)

| Parte | Descripción | Ejemplo |
|-------|-------------|---------|
| Nombre | Identificador del campo | `nombre` |
| Tipo | Qué tipo de dato acepta | `str` |
| Valor | El dato almacenado | `"Ana López"` |

**Analogía:** Un campo es como una **celda en Excel**:
- La columna tiene un nombre (encabezado)
- La celda contiene un valor
- Solo acepta cierto tipo de dato

### 3.2 ¿Qué es un registro?

Un **registro** es un conjunto de campos relacionados que juntos representan una entidad completa.

**Ejemplo: Registro de un estudiante**

| Campo | Valor | Tipo |
|-------|-------|------|
| nombre | "Ana López" | str |
| edad | 16 | int |
| promedio | 8.7 | float |
| activo | True | bool |
| direccion | None | null |

### 3.3 Tablas: Conjuntos de Registros

Cuando tienes múltiples registros del mismo tipo, formas una **tabla** (como en una hoja de cálculo o base de datos).

| nombre | edad | promedio | activo | direccion |
|--------|------|----------|--------|-----------|
| Ana López | 16 | 8.7 | True | "Calle 45" |
| Carlos Ruiz | 17 | 9.2 | True | None |
| María García | 16 | 7.5 | False | "Carrera 10" |

**Concepto clave:**
- **Campo** = Columna (una característica)
- **Registro** = Fila (un conjunto de características de una entidad)
- **Tabla** = Conjunto de registros del mismo tipo

### 3.4 Actividad de Refuerzo: Identificar Campos y Registros

**Situación:** Sistema de biblioteca escolar

Cada libro en el sistema tiene los siguientes datos:
- Título del libro
- Autor
- Año de publicación
- Número de páginas
- Disponible para préstamo (sí/no)
- Número de ejemplares

**Tarea:** Completa la siguiente tabla.

| Nombre del Campo | Tipo de Dato Sugerido |
|------------------|----------------------|
| titulo | str |
| autor | str |
| año_publicacion | int |
| numero_paginas | int |
| disponible | bool |
| ejemplares | int |

**Ahora, crea 3 registros de ejemplo:**

| titulo | autor | año_publicacion | numero_paginas | disponible | ejemplares |
|--------|-------|-----------------|----------------|------------|------------|
| 1. | | | | | |
| 2. | | | | | |
| 3. | | | | | |

---

## 4. Variables: Espacios con Nombre

### 4.1 Definición

Una **variable** es un espacio en la memoria del computador que:
- Tiene un **nombre** (identificador)
- Contiene un **valor** de un tipo específico
- Puede **cambiar** su valor durante la ejecución del programa

**Analogía:** Una variable es como una **caja etiquetada** en un almacén:
- La etiqueta es el nombre de la variable
- El contenido de la caja es el valor
- Puedes cambiar lo que hay dentro de la caja

```
    ┌─────────────┐
    │   edad      │  ← Nombre (etiqueta)
    │    16       │  ← Valor (contenido)
    │   (int)     │  ← Tipo (características de la caja)
    └─────────────┘
```

### 4.2 Partes de una Variable

| Parte | Descripción | Ejemplo |
|-------|-------------|---------|
| Nombre | Identificador de la variable | `nombre_estudiante` |
| Tipo | Tipo de dato que almacena | `str` |
| Valor | Contenido actual | `"Carlos Mendoza"` |

### 4.3 Declaración vs Asignación

#### Declaración

Indicar que una variable **existirá**, definiendo su nombre y tipo.

```
// Pseudocódigo
ENTERO edad
TEXTO nombre
DECIMAL promedio
```

#### Asignación

**Dar o cambiar** el valor de una variable.

```
// Asignar un valor por primera vez
edad = 16
nombre = "Carlos Mendoza"
promedio = 8.5

// Cambiar el valor posteriormente
edad = 17
promedio = 9.2
```

#### Declaración con Inicialización

Combinar ambos pasos en una sola línea.

```
ENTERO edad = 16
TEXTO nombre = "Carlos Mendoza"
DECIMAL promedio = 8.5
```

### 4.4 Ejemplos de Variables en Pseudocódigo

```
// Variables para un sistema de calificaciones
ENTERO cantidad_examenes = 3
TEXTO nombre_estudiante = "Ana López"
DECIMAL nota_examen_1 = 8.5
DECIMAL nota_examen_2 = 9.0
DECIMAL nota_examen_3 = 7.8
LOGICO asistencia_completa = True
TEXTO fecha_registro = "16/04/2026"

// Variables para una tienda
ENTERO cantidad_productos = 50
DECIMAL precio_unitario = 25990.00
DECIMAL descuento_porcentaje = 10.0
TEXTO nombre_cajero = "Pedro Martínez"
LOGICO esta_abierto = True
```

---

## 5. Nombres, Declaraciones y Buenas Prácticas

### 5.1 Reglas para Nombrar Variables

#### Reglas obligatorias (el código no funcionará si las incumples)

| Regla | Correcto | Incorrecto | ¿Por qué? |
|-------|----------|------------|-----------|
| Sin espacios | `nombre_cliente` | `nombre cliente` | Los espacios separan comandos |
| Sin iniciar con número | `nota1`, `precio2` | `1nota`, `2precio` | El intérprete lo confunde con números |
| Sin caracteres especiales | `contador_total` | `contador@total` | `@` no es válido en nombres |
| Sin palabras reservadas | `mi_edad` | `int` | `int` es una palabra del lenguaje |

#### Palabras reservadas comunes (no usar como nombres)

```
// NO usar estos nombres para variables:
int, float, str, bool, if, else, while, for, return,
True, False, None, and, or, not, def, class, print
```

### 5.2 Convenciones Recomendadas (Buenas Prácticas)

#### Convenciones de nombres por tipo de lenguaje

**PascalCase** (primera letra de cada palabra en mayúscula):
```
NombreCompleto
FechaNacimiento
PrecioUnitario
```

**camelCase** (primera palabra en minúscula, las demás con mayúscula inicial):
```
nombreCompleto
fechaNacimiento
precioUnitario
```

**snake_case** (todas en minúscula, palabras separadas por guiones bajos):
```
nombre_completo
fecha_nacimiento
precio_unitario
```

> **Recomendación:** Usaremos **snake_case** en pseudocódigo por ser el más legible y widely utilizado en Python.

### 5.3 Guía de Nombres Significativos

| ❌ Mal nombre | ✅ Buen nombre | ¿Por qué? |
|--------------|---------------|-----------|
| `x` | `edad_estudiante` | Describe qué almacena |
| `n` | `cantidad_productos` | Indica la naturaleza |
| `a` | `precio_unitario` | Es específico |
| `tmp` | `temporal_para_calculo` | Es descriptivo |
| `d` | `fecha_nacimiento` | Claramente identificable |

### 5.4 Tabla de Tipos en Pseudocódigo

| Tipo de Dato | Keyword en Pseudocódigo | Ejemplo |
|--------------|-------------------------|---------|
| Entero | `ENTERO` o `INT` | `ENTERO edad = 16` |
| Decimal | `DECIMAL` o `REAL` o `FLOAT` | `DECIMAL promedio = 8.7` |
| Texto | `TEXTO` o `CADENA` o `STRING` | `TEXTO nombre = "Ana"` |
| Booleano | `LOGICO` o `BOOLEANO` o `BOOL` | `LOGICO activo = True` |
| Sin valor | `NULO` o `NINGUNO` o `NULL` | `TEXTO telefono = NULO` |

### 5.5 Ejemplos de Declaraciones Correctas

```
// ============================================
// DECLARACIONES CORRECTAS EN PSEUDOCÓDIGO
// ============================================

// Variables simples
ENTERO edad = 16
ENTERO cantidad = 0
DECIMAL estatura = 1.73
DECIMAL precio = 49990.99
TEXTO nombre = "Juan Pérez"
TEXTO direccion = "Carrera 15 #45-30"
LOGICO es_estudiante = True
LOGICO tiene_beca = False
TEXTO telefono = NULO

// Constantes (valores que no cambian)
ENTERO DIAS_SEMANA = 7
DECIMAL PI = 3.14159
TEXTO NOMBRE_SISTEMA = "Sistema Escolar v1.0"

// Arreglos
ARREGLO ENTERO edades = [16, 17, 16, 18]
ARREGLO TEXTO nombres = ["Ana", "Carlos", "María"]
```

### 5.6 Errores Comunes a Evitar

| Código Incorrecto | Error | Corrección |
|-------------------|-------|------------|
| `TEXTO nombre completo = "Ana"` | Espacios en el nombre | `TEXTO nombre_completo = "Ana"` |
| `ENTERO 1nota = 8` | Inicia con número | `ENTERO nota1 = 8` |
| `ENTERO precio@unitario = 5000` | Caracter especial `@` | `ENTERO precio_unitario = 5000` |
| `ENTERO int = 5` | Palabra reservada | `ENTERO valor_int = 5` |
| `ENTERO edad = "dieciséis"` | Tipo incorrecto | `TEXTO edad_texto = "dieciséis"` |
| `promedio = 8.5` | Variable no declarada | `DECIMAL promedio = 8.5` |

---

## 6. Representación en Pseudocódigo

### 6.1 ¿Qué es el Pseudocódigo?

El **pseudocódigo** es un lenguaje de especificación informal que permite describir algoritmos usando una mezcla de:
- Español (u otro idioma natural)
- Convenciones de programación
- Estructuras lógicas simples

**Propósito:** Planificar soluciones antes de programar, sin preocuparse por la sintaxis de un lenguaje específico.

### 6.2 Estructura Básica de un Pseudocódigo

```
INICIO
    // Sección de DECLARACIÓN de variables
    <tipo> <nombre_variable> = <valor_inicial>
    <tipo> <nombre_variable>

    // Sección de ENTRADA (lectura de datos)
    LEER <variable>

    // Sección de PROCESO (cálculos y operaciones)
    <variable> = <expresión>

    // Sección de SALIDA (mostrar resultados)
    ESCRIBIR <mensaje o variable>
FIN
```

### 6.3 Palabras Clave Comunes

| Palabra | Función | Ejemplo |
|---------|---------|---------|
| `INICIO` | Marca el comienzo del algoritmo | `INICIO` |
| `FIN` | Marca el final del algoritmo | `FIN` |
| `LEER` | Captura datos del usuario | `LEER nombre` |
| `ESCRIBIR` | Muestra información | `ESCRIBIR "Hola"` |
| `//` | Comentario (no se ejecuta) | `// Esto es un comentario` |

---

### 6.4 Ejemplo Completo 1: Saludar al Usuario

**Problema:** Pedir el nombre del usuario y mostrar un saludo.

| Elemento | Descripción |
|----------|-------------|
| **ENTRADA** | nombre (texto) |
| **PROCESO** | Crear mensaje de saludo |
| **SALIDA** | Mensaje de saludo personalizado |

```
INICIO
    TEXTO nombre

    ESCRIBIR "Por favor, ingresa tu nombre:"
    LEER nombre

    ESCRIBIR "¡Hola, " + nombre + "! Bienvenido."
FIN
```

**Ejecución paso a paso:**

```
Paso 1: Se declara variable TEXTO nombre
Paso 2: Se muestra "Por favor, ingresa tu nombre:"
Paso 3: Usuario escribe "Carlos" y presiona Enter
Paso 4: Variable nombre = "Carlos"
Paso 5: Se evalúa "¡Hola, " + nombre + "!" → "¡Hola, Carlos!"
Paso 6: Se muestra en pantalla
```

---

### 6.5 Ejemplo Completo 2: Calcular el Área de un Rectángulo

**Problema:** Ingresar el ancho y alto de un rectángulo, calcular y mostrar su área.

| Elemento | Descripción |
|----------|-------------|
| **ENTRADA** | ancho (decimal), alto (decimal) |
| **PROCESO** | area = ancho × alto |
| **SALIDA** | valor del área |

```
INICIO
    DECIMAL ancho
    DECIMAL alto
    DECIMAL area

    ESCRIBIR "Ingresa el ancho del rectángulo (metros):"
    LEER ancho

    ESCRIBIR "Ingresa el alto del rectángulo (metros):"
    LEER alto

    area = ancho * alto

    ESCRIBIR "El área del rectángulo es: " + area + " metros cuadrados"
FIN
```

**Prueba con datos reales:**

```
Entrada: ancho = 5, alto = 3
Proceso: area = 5 * 3 = 15
Salida: "El área del rectángulo es: 15 metros cuadrados"
```

---

### 6.6 Ejemplo Completo 3: Determinar si un Estudiante Aprobó

**Problema:** Ingresar la calificación de un estudiante (0-10) y determinar si aprueba (nota >= 6.0).

| Elemento | Descripción |
|----------|-------------|
| **ENTRADA** | calificacion (decimal) |
| **PROCESO** | Si calificacion >= 6.0, entonces Aprobado |
| **SALIDA** | Mensaje indicando aprobación |

```
INICIO
    DECIMAL calificacion
    LOGICO aprobo

    ESCRIBIR "Ingresa tu calificación (0-10):"
    LEER calificacion

    aprobo = (calificacion >= 6.0)

    SI aprobo == True ENTONCES
        ESCRIBIR "¡Felicidades! Aprobaste la materia."
    SI_NO
        ESCRIBIR "Lo sentimos, no aprobaste. Deberás repetir."
    FIN_SI
FIN
```

**Pruebas:**

```
Prueba 1: calificacion = 8.5
          aprobo = (8.5 >= 6.0) = True
          Salida: "¡Felicidades! Aprobaste la materia."

Prueba 2: calificacion = 5.3
          aprobo = (5.3 >= 6.0) = False
          Salida: "Lo sentimos, no aprobaste. Deberás repetir."
```

---

### 6.7 Ejemplo Completo 4: Sistema de Descuento

**Problema:** Una tienda aplica 10% de descuento en compras mayores a $100.000. Ingresar el precio y mostrar el precio final.

```
INICIO
    DECIMAL precio_original
    DECIMAL porcentaje_descuento
    DECIMAL descuento
    DECIMAL precio_final
    LOGICO aplica_descuento

    precio_original = 0
    porcentaje_descuento = 10.0

    ESCRIBIR "Ingresa el precio del producto:"
    LEER precio_original

    aplica_descuento = (precio_original > 100000)

    SI aplica_descuento == True ENTONCES
        descuento = precio_original * (porcentaje_descuento / 100)
        precio_final = precio_original - descuento
        ESCRIBIR "¡Tienes un 10% de descuento!"
        ESCRIBIR "Descuento: $" + descuento
        ESCRIBIR "Precio final: $" + precio_final
    SI_NO
        precio_final = precio_original
        ESCRIBIR "No aplica descuento."
        ESCRIBIR "Precio final: $" + precio_final
    FIN_SI
FIN
```

---

### 6.8 Plantilla Base para tus Pseudocódigos

Usa esta plantilla como punto de partida:

```
// ============================================
// ALGORITMO: [Nombre del algoritmo]
// ============================================
// ENTRADA:  [Lista de datos de entrada con tipos]
// PROCESO:  [Descripción del proceso]
// SALIDA:   [Descripción del resultado]
// ============================================

INICIO
    // DECLARACIÓN DE VARIABLES
    [Tipo] [variable1]
    [Tipo] [variable2] = [valor_inicial]

    // ENTRADA DE DATOS
    ESCRIBIR "[Mensaje para el usuario]"
    LEER [variable]

    // PROCESAMIENTO
    [variable_resultado] = [expresión o cálculo]

    // SALIDA DE RESULTADOS
    ESCRIBIR "[mensaje o variable]"
FIN
```

---

## 7. Práctica Dirigida: Declaración de Variables

### 7.1 Práctica 1: Declara las Variables

**Instrucciones:** Para cada escenario, declara las variables necesarias con su tipo correcto.

---

**Escenario A: Registro de un libro en una biblioteca**

Necesitas almacenar: título, autor, año de publicación, número de páginas, si está disponible.

```
// Escribe tu código aquí:
```

**Solución sugerida:**
```
TEXTO titulo
TEXTO autor
ENTERO anio_publicacion
ENTERO numero_paginas
LOGICO disponible
```

---

**Escenario B: Sistema de calificaciones**

Necesitas almacenar: nombre del estudiante, tres notas parciales, promedio de las tres notas, si está eximido del examen final (promedio >= 9.0).

```
// Escribe tu código aquí:
```

**Solución sugerida:**
```
TEXTO nombre_estudiante
DECIMAL nota1
DECIMAL nota2
DECIMAL nota3
DECIMAL promedio
LOGICO eximido
```

---

**Escenario C: Carrito de compras en línea**

Necesitas almacenar: nombre del producto, precio unitario, cantidad deseada, subtotal, si hay descuento aplicado, precio final.

```
// Escribe tu código aquí:
```

**Solución sugerida:**
```
TEXTO nombre_producto
DECIMAL precio_unitario
ENTERO cantidad
DECIMAL subtotal
LOGICO hay_descuento
DECIMAL precio_final
```

---

### 7.2 Práctica 2: Identifica los Errores

**Instrucciones:** Lee cada pseudocódigo y encuentra los errores. Explica qué está mal y cómo corregirlo.

---

**Código 1:**
```
INICIO
    TEXTO nombre completo = "Ana López"
    ENTERO 1edad = 16
    DECIMAL precio-producto = 25990.99
FIN
```

**Errores encontrados:**
```
1. _______________________________________________________________
2. _______________________________________________________________
3. _______________________________________________________________
```

**Corrección:**
```
// Escribe la versión corregida:
```

---

**Código 2:**
```
INICIO
    ENTERO edad = "dieciséis"
    LOGICO activo = "sí"
    TEXTO telefono = 3001234567
    DECIMAL pi = 3.14159
FIN
```

**Errores encontrados:**
```
1. _______________________________________________________________
2. _______________________________________________________________
3. _______________________________________________________________
```

**Corrección:**
```
// Escribe la versión corregida:
```

---

**Código 3:**
```
INICIO
    TEXTO nombre = "Carlos"
    TEXTO apellido = "Mendoza"
    ENTERO int = 25
    LOGICO True = tienes_descuento
FIN
```

**Errores encontrados:**
```
1. _______________________________________________________________
2. _______________________________________________________________
3. _______________________________________________________________
```

**Corrección:**
```
// Escribe la versión corregida:
```

---

### 7.3 Práctica 3: Completa el Pseudocódigo

**Instrucciones:** Lee el problema y completa los espacios en blanco.

---

**Problema: Calculadora de IMC (Índice de Masa Corporal)**

| Elemento | Descripción |
|----------|-------------|
| **ENTRADA** | peso (kg), altura (metros) |
| **PROCESO** | IMC = peso / (altura × altura) |
| **SALIDA** | Valor del IMC |

```
INICIO
    // DECLARACIÓN DE VARIABLES
    ___________ peso
    ___________ altura
    ___________ imc
    ___________ categoria

    // ENTRADA DE DATOS
    ESCRIBIR "Ingresa tu peso en kilogramos:"
    ___________ peso

    ESCRIBIR "Ingresa tu altura en metros:"
    ___________ altura

    // PROCESAMIENTO
    imc = ___________ / (altura ___________ altura)

    // SALIDA DE RESULTADOS
    ESCRIBIR "Tu IMC es: " ___________ imc
FIN
```

**Tu tarea:** Completa con:
- Tipos de datos apropiados
- Comandos LEER/ESCRIBIR faltantes
- Operador de exponenciación (o multiplicación)

---

**Problema: Verificador de Votación**

| Elemento | Descripción |
|----------|-------------|
| **ENTRADA** | edad (entero) |
| **PROCESO** | Verificar si edad >= 18 |
| **SALIDA** | Mensaje de autorización |

```
INICIO
    ___________ edad
    ___________ puede_votar

    ESCRIBIR "Ingresa tu edad:"
    ___________ edad

    puede_votar = (edad ___________ 18)

    SI puede_votar == ___________ ENTONCES
        ESCRIBIR "¡Puedes votar!"
    SI_NO
        ESCRIBIR "No puedes votar aún."
    ___________ SI
FIN
```

---

### 7.4 Práctica 4: Escribe tu Propio Pseudocódigo

**Instrucciones:** Elige UNO de los siguientes problemas y escribe el pseudocódigo completo.

**Opciones:**

**A) Conversor de Temperatura**
- Pedir temperatura en Celsius
- Convertir a Fahrenheit: F = C × 9/5 + 32
- Mostrar el resultado

**B) Calculadora de Propina**
- Pedir el total de la cuenta de un restaurante
- Calcular la propina del 10%
- Mostrar total + propina

**C) Verificador de Contraseña**
- Pedir una contraseña
- Verificar si tiene más de 8 caracteres
- Mostrar si es válida o no

---

**Usa esta plantilla:**

```
// ============================================
// ALGORITMO: [Nombre]
// ============================================
// ENTRADA:  [¿Qué necesitas?]
// PROCESO:  [¿Qué cálculos haces?]
// SALIDA:   [¿Qué muestras?]
// ============================================

INICIO
    // Escribe tu pseudocódigo aquí










FIN
```

---

## 8. Quiz Final de Evaluación

### 8.1 Parte A: Preguntas de Opción Múltiple

**Instrucciones:** Selecciona la respuesta correcta.

---

**Pregunta 1.** ¿Cuál de los siguientes es un ejemplo de DATO (no información)?

A) "La temperatura es de 36.5 grados"
B) "María tiene 17 años"
C) `36.5` (solo el número, sin contexto)
D) "El paciente tiene fiebre"

---

**Pregunta 2.** ¿Qué tipo de dato es el valor `True`?

A) Texto (str)
B) Entero (int)
C) Booleano (bool)
D) Decimal (float)

---

**Pregunta 3.** ¿Cuál es la declaración CORRECTA de una variable en pseudocódigo?

A) `TEXTO nombre completo = "Ana"`
B) `ENTERO 1edad = 16`
C) `DECIMAL precio = 25990.99`
D) `LOGICO @ctivo = True`

---

**Pregunta 4.** ¿Qué significa el tipo de dato `null` o `None`?

A) El número cero
B) Un texto vacío
C) La ausencia intencional de valor
D) El valor negativo de algo

---

**Pregunta 5.** En una tabla de base de datos, ¿qué representa una FILA?

A) El tipo de datos de una columna
B) Un registro completo (conjunto de campos de una entidad)
C) El nombre de la tabla
D) Una fórmula de cálculo

---

**Pregunta 6.** ¿Cuál es la diferencia entre `DECIMAL precio = 150000` y `TEXTO precio = "150000"`?

A) No hay diferencia
B) El primero es un número y puede usarse en cálculos; el segundo es texto
C) El segundo es un número más preciso
D) El primero es más corto

---

**Pregunta 7.** ¿Cuál de los siguientes NO es un tipo de dato primitivo?

A) Entero
B) Booleano
C) Arreglo
D) Texto

---

**Pregunta 8.** ¿Qué palabra se usa en pseudocódigo para CAPTURAR datos del usuario?

A) ESCRIBIR
B) MOSTRAR
C) LEER
D) IMPRIMIR

---

### 8.2 Parte B: Preguntas de Completar

**Instrucciones:** Completa cada oración con la palabra o concepto correcto.

---

**Pregunta 9.** Un ___________ es un espacio en memoria con nombre que almacena un valor de un tipo específico.

**Pregunta 10.** El tipo de dato para números con decimales se llama ___________ (ejemplo: 3.14).

**Pregunta 11.** ___________ son los valores que solo pueden ser True o False.

**Pregunta 12.** En pseudocódigo, la palabra clave ___________ se usa para mostrar información al usuario.

**Pregunta 13.** Un ___________ es un conjunto de campos que representan una entidad completa.

**Pregunta 14.** La convención de nombres donde_separamos_con_guiones_bajos se llama ___________.

**Pregunta 15.** El valor `""` (comillas vacías) representa un texto ___________, mientras que `null` representa la ___________ de valor.

---

### 8.3 Parte C: Práctica de Código

**Instrucciones:** Escribe el pseudocódigo según las especificaciones.

---

**Pregunta 16.** Declara las variables necesarias para un sistema de registro de estudiantes con:
- Nombre completo
- Edad
- Promedio general
- Si es becaado o no

```
// Escribe tu declaración de variables:
```

---

**Pregunta 17.** Completa el siguiente pseudocódigo para calcular el 20% de IVA sobre un precio:

```
INICIO
    ___________ precio_sin_iva
    ___________ porcentaje_iva
    ___________ iva
    ___________ precio_final

    ESCRIBIR "Ingresa el precio sin IVA:"
    ___________ precio_sin_iva

    iva = precio_sin_iva ___________ 0.20
    precio_final = precio_sin_iva ___________ iva

    ESCRIBIR "El IVA es: $" + iva
    ESCRIBIR "El precio final es: $" + precio_final
FIN
```

---

### 8.4 Parte D: Análisis de Errores

**Pregunta 18.** Identifica Y corrige los errores en el siguiente pseudocódigo:

```
INICIO
    TEXTO nombre completo = "Juan"
    ENTERO edad = "dieciséis"
    DECIMAL altura = 1.73
    LOGICO activo = True
    TEXTO telefono = 3001234567
    DECIMAL resultado = "veinte"
FIN
```

**Errores encontrados:**
```
1. _______________________________________________________________
2. _______________________________________________________________
3. _______________________________________________________________
4. _______________________________________________________________
```

**Versión corregida:**
```
INICIO

FIN
```

---

## 9. Actividad Integradora

### Proyecto: Sistema de Registro de Productos

**Descripción:** Crearás el pseudocódigo para un pequeño sistema de inventario que permita registrar productos, calcular su precio con descuento y determinar si hay que reponer stock.

---

### Requisitos del Sistema

1. **Registro del producto:**
   - Nombre del producto (texto)
   - Precio unitario (decimal)
   - Cantidad en stock (entero)
   - Cantidad mínima para reponer (entero)

2. **Cálculos necesarios:**
   - Descuento del 15% si el precio es mayor a $50.000
   - Precio final con descuento (si aplica)
   - Determinar si necesita reposición (si stock < mínimo)

3. **Salida del programa:**
   - Datos del producto
   - Precio original
   - Mensaje si hay descuento y cuánto ahorra
   - Precio final
   - Mensaje si necesita reponer stock

---

### Plantilla del Pseudocódigo

```
// ============================================================
// ALGORITMO: Sistema de Registro de Productos
// ============================================================
// ENTRADA:
//   - nombre_producto (TEXTO)
//   - precio_unitario (DECIMAL)
//   - cantidad_stock (ENTERO)
//   - cantidad_minima (ENTERO)
// PROCESO:
//   - Calcular descuento si precio > 50000 (15%)
//   - Determinar precio final
//   - Verificar si necesita reponer stock
// SALIDA:
//   - Información del producto con cálculos
// ============================================================

INICIO
    // ============================================
    // DECLARACIÓN DE VARIABLES
    // ============================================









    // ============================================
    // ENTRADA DE DATOS
    // ============================================

    ESCRIBIR "=== SISTEMA DE REGISTRO DE PRODUCTOS ==="
    ESCRIBIR ""

    ESCRIBIR "Ingresa el nombre del producto:"
    LEER nombre_producto

    ESCRIBIR "Ingresa el precio unitario:"
    LEER precio_unitario

    ESCRIBIR "Ingresa la cantidad en stock:"
    LEER cantidad_stock

    ESCRIBIR "Ingresa la cantidad mínima para reponer:"
    LEER cantidad_minima

    // ============================================
    // PROCESAMIENTO
    // ============================================

    // Verificar si aplica descuento (15% si precio > 50000)






    // Verificar si necesita reponer stock




    // ============================================
    // SALIDA DE RESULTADOS
    // ============================================

    ESCRIBIR ""
    ESCRIBIR "=== RESULTADOS ==="
    ESCRIBIR "Producto: " + nombre_producto
    ESCRIBIR "Precio original: $" + precio_unitario

    // Mostrar información de descuento







    // Mostrar precio final







    // Mostrar estado de stock







FIN
```

---

### Criterios de Evaluación

| Criterio | Puntos |
|----------|--------|
| Declara todas las variables con tipos correctos | /15 |
| Captura todos los datos de entrada | /10 |
| Calcula el descuento correctamente (15% si > 50000) | /15 |
| Calcula el precio final correctamente | /10 |
| Determina si necesita reponer stock | /10 |
| Muestra todos los resultados relevantes | /10 |
| El pseudocódigo es claro y legible | /10 |
| Uso correcto de nombres y convenciones | /10 |
| Código sin errores de sintaxis | /10 |
| **Total** | **/100** |

---

### Ejemplo de Ejecución Esperada

```
=== SISTEMA DE REGISTRO DE PRODUCTOS ===

Ingresa el nombre del producto:
Portátil HP
Ingresa el precio unitario:
850000
Ingresa la cantidad en stock:
5
Ingresa la cantidad mínima para reponer:
3

=== RESULTADOS ===
Producto: Portátil HP
Precio original: $850000.0
¡Tienes un descuento del 15%!
Ahorro: $127500.0
Precio final: $722500.0
Stock actual: 5 unidades
Estado: Stock suficiente

---
OTRO CASO DE PRUEBA:

Ingresa el nombre del producto:
Cuaderno college
Ingresa el precio unitario:
12000
Ingresa la cantidad en stock:
2
Ingresa la cantidad mínima para reponer:
5

=== RESULTADOS ===
Producto: Cuaderno college
Precio original: $12000.0
No aplica descuento.
Precio final: $12000.0
Stock actual: 2 unidades
⚠️ ALERTA: ¡Necesita reponer stock!
```

---

## Autoevaluación Final

**Instrucciones:** Responde con honestidad para identificar qué necesitas repasar.

| Concepto | Lo entiendo bien | Necesito repasar | No lo entiendo |
|---------|------------------|------------------|----------------|
| Diferencia entre dato e información | ☐ | ☐ | ☐ |
| Tipos de datos primitivos | ☐ | ☐ | ☐ |
| Campos y registros | ☐ | ☐ | ☐ |
| Declaración de variables | ☐ | ☐ | ☐ |
| Nombres válidos y convenciones | ☐ | ☐ | ☐ |
| Pseudocódigo básico | ☐ | ☐ | ☐ |
| Uso de LEER y ESCRIBIR | ☐ | ☐ | ☐ |

---

## Resumen de Conceptos Clave

> **MENSAJES CLAVE**
>
> 1. **DATO** es un hecho raw; **INFORMACIÓN** es un dato con significado
>
> 2. Tipos primitivos: **ENTERO, DECIMAL, TEXTO, LOGICO, NULO**
>
> 3. Un **CAMPO** es una característica; un **REGISTRO** es la entidad completa
>
> 4. **VARIABLE** = espacio en memoria con nombre y tipo
>
> 5. Nombres significativos: `edad_estudiante` NO `x`
>
> 6. Pseudocódigo: **LEER** (entrada), proceso, **ESCRIBIR** (salida)
>
> 7. El computador hace lo que le dices, no lo que quieres → **Usa los tipos correctos**

---

## Distribución del Tiempo Sugerido

| Sección | Tiempo | Actividad |
|---------|--------|----------|
| 1. Información y Datos | 20 min | Lectura + ejemplos |
| 2. Clasificación de Tipos | 25 min | Estudio de tablas |
| 3. Campos y Registros | 20 min | Actividad práctica |
| 4. Variables | 20 min | Conceptual + ejemplos |
| 5. Nombres y Declaraciones | 20 min | Práctica de errores |
| 6. Pseudocódigo | 25 min | Ejemplos guiados |
| 7. Práctica Dirigida | 30 min | Ejercicios 1-4 |
| 8. Quiz Final | 20 min | Evaluación individual |
| **Total** | **180 min** | |

---

*Material elaborado para uso educativo — Fundamentos de Programación*
*Adaptado para estudiantes de 10º grado (15-16 años)*
*Clase 02 — Tipos de Datos, Variables y Pseudocódigo*