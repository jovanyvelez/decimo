# 🖥️ Sistemas Numéricos: El Lenguaje Secreto de las Computadoras

> **Nivel:** Secundaria (15–16 años)  
> **Duración total:** 4 horas (2 sesiones de descanso de 15 min c/u)  
> **Autor:** Material didáctico de aula  
> **Temas:** Sistema Binario · Sistema Octal · Conversiones · Sistemas Digitales

---

## 📋 Tabla de Contenidos

1. [¿Por qué las computadoras no hablan como nosotros?](#1-por-qué-las-computadoras-no-hablan-como-nosotros)
2. [El Sistema Decimal — Nuestro punto de partida](#2-el-sistema-decimal--nuestro-punto-de-partida)
3. [El Sistema Binario — El idioma de las máquinas](#3-el-sistema-binario--el-idioma-de-las-máquinas)
   - [Conversión: Decimal → Binario](#31-conversión-decimal--binario)
   - [Conversión: Binario → Decimal](#32-conversión-binario--decimal)
   - [Ejercicios paso a paso](#33-ejercicios-paso-a-paso-binario)
4. [Tabla Maestra de Conversiones](#4-tabla-maestra-de-conversiones)
5. [⏸️ DESCANSO 1 — 15 minutos](#️-descanso-1--15-minutos)
6. [El Sistema Octal — El atajo inteligente](#6-el-sistema-octal--el-atajo-inteligente)
   - [Conversión: Decimal → Octal](#61-conversión-decimal--octal)
   - [Conversión: Octal → Decimal](#62-conversión-octal--decimal)
   - [Conversión: Binario ↔ Octal](#63-conversión-binario--octal-el-truco-mágico)
   - [Ejercicios paso a paso](#64-ejercicios-paso-a-paso-octal)
7. [⏸️ DESCANSO 2 — 15 minutos](#️-descanso-2--15-minutos)
8. [Práctica Individual con Seguimiento](#8-práctica-individual-con-seguimiento)
9. [🎮 Juego de Roles — La Computadora Humana](#9--juego-de-roles--la-computadora-humana)
10. [Resumen y Cierre](#10-resumen-y-cierre)

---

## Guía de Tiempos para el Docente

| Bloque | Actividad | Duración |
|--------|-----------|----------|
| 🟢 Bloque 1 | Introducción + Sistema Decimal | 20 min |
| 🟢 Bloque 2 | Sistema Binario (teoría + conversiones) | 45 min |
| 🟢 Bloque 3 | Ejercicios binarios + Tabla maestra | 35 min |
| 🟢 Bloque 4 | Practica guiada binario | 20 min |
| ⏸️ | **DESCANSO 1** | **15 min** |
| 🔵 Bloque 5 | Sistema Octal (teoría + conversiones) | 40 min |
| 🔵 Bloque 6 | Ejercicios octal + conversión binario↔octal | 30 min |
| ⏸️ | **DESCANSO 2** | **15 min** |
| 🔴 Bloque 7 | Práctica individual con seguimiento | 20 min |
| 🔴 Bloque 8 | Juego de roles "Computadora Humana" | 30 min |
| 🔴 Bloque 9 | Resumen y cierre | 10 min |
| **TOTAL** | | **4 h 10 min aprox.** |

---

# BLOQUE 1 — Introducción *(20 min)*

## 1. ¿Por qué las computadoras no hablan como nosotros?

Imagina que tienes que comunicarte con alguien que **solo puede decir dos palabras: "sí" o "no"**. Suena limitado, ¿verdad? Pero con suficientes preguntas de sí/no puedes transmitir cualquier información del mundo.

Eso es exactamente lo que hacen las computadoras.

### ¿Qué hay dentro de un chip?

Dentro de cualquier procesador existen millones de pequeños interruptores llamados **transistores**. Cada transistor solo tiene dos estados:

```
⚡ Hay electricidad  →  Estado: 1  (encendido / TRUE)
💤 No hay electricidad →  Estado: 0  (apagado / FALSE)
```

> **¡Dato curioso!** El chip del iPhone 15 tiene **19,000 millones** de transistores en un espacio del tamaño de tu uña. Cada uno de esos transistores solo conoce el 0 y el 1.

### Los sistemas numéricos que veremos hoy

| Sistema | Base | Símbolos que usa | ¿Dónde se usa? |
|---------|------|-----------------|----------------|
| Decimal | 10 | 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 | Vida diaria |
| **Binario** | **2** | **0, 1** | **Circuitos digitales, CPU** |
| **Octal** | **8** | **0, 1, 2, 3, 4, 5, 6, 7** | **Permisos Unix, programación** |
| Hexadecimal | 16 | 0–9, A–F | Colores web, memoria RAM |

---

# BLOQUE 2 — El Sistema Decimal *(parte del bloque 1)*

## 2. El Sistema Decimal — Nuestro punto de partida

Antes de aprender un nuevo idioma, hay que entender bien el propio. El sistema decimal funciona con **potencias de 10**.

### ¿Qué significa el número 3,472?

```
  3  ,  4  ,  7  ,  2
  ↑     ↑     ↑     ↑
 Mil  Cien  Diez  Unidad
 10³   10²   10¹   10⁰
1000   100    10     1
```

**Comprobación:**
```
(3 × 1000) + (4 × 100) + (7 × 10) + (2 × 1)
= 3000 + 400 + 70 + 2
= 3,472  ✅
```

> 💡 **Concepto clave:** En cualquier sistema numérico, **la posición de cada dígito le da su valor**. Esto se llama **sistema posicional**.

---

# BLOQUE 3 — Sistema Binario *(45 min)*

## 3. El Sistema Binario — El idioma de las máquinas

El sistema binario funciona exactamente igual que el decimal, **pero con potencias de 2** en lugar de potencias de 10.

### Las potencias de 2 que debes memorizar

| Potencia | Valor |
|----------|-------|
| 2⁰ | 1 |
| 2¹ | 2 |
| 2² | 4 |
| 2³ | 8 |
| 2⁴ | 16 |
| 2⁵ | 32 |
| 2⁶ | 64 |
| 2⁷ | 128 |
| 2⁸ | 256 |

> 🎯 **Truco para recordarlas:** 1, 2, 4, 8, 16, 32, 64, 128… Cada número es el **doble del anterior**.

### Vocabulario esencial

| Término | Significado |
|---------|-------------|
| **Bit** | Un solo dígito binario (0 o 1). La unidad mínima de información. |
| **Nibble** | Grupo de 4 bits |
| **Byte** | Grupo de 8 bits — puede representar 256 valores distintos (0 a 255) |
| **Kilobyte (KB)** | 1,024 bytes |
| **Megabyte (MB)** | 1,024 KB |

---

## 3.1 Conversión: Decimal → Binario

### Método de las divisiones sucesivas

**Regla de oro:** Divide repetidamente entre 2 y anota los **residuos de abajo hacia arriba**.

---

### 🔍 Ejemplo 1 — Convertir 13 a binario

**Paso 1:** Divide entre 2 y anota el residuo.

```
13 ÷ 2 = 6   residuo → 1   ← último en entrar, primero en salir
 6 ÷ 2 = 3   residuo → 0
 3 ÷ 2 = 1   residuo → 1
 1 ÷ 2 = 0   residuo → 1   ← primero en entrar, último en salir
```

**Paso 2:** Lee los residuos de **abajo hacia arriba** (como si leyeras una escalera de subida):

```
Residuos leídos de ↑ arriba hacia abajo: 1 → 1 → 0 → 1
```

**Resultado:** 13₁₀ = **1101₂**

**Verificación:**
```
1×2³ + 1×2² + 0×2¹ + 1×2⁰
= 8   +   4  +   0  +   1
= 13  ✅
```

---

### 🔍 Ejemplo 2 — Convertir 25 a binario

```
25 ÷ 2 = 12  residuo → 1
12 ÷ 2 = 6   residuo → 0
 6 ÷ 2 = 3   residuo → 0
 3 ÷ 2 = 1   residuo → 1
 1 ÷ 2 = 0   residuo → 1
              ↑ leer de aquí
```

Leyendo de abajo hacia arriba: **1 1 0 0 1**

**Resultado:** 25₁₀ = **11001₂**

**Verificación:**
```
1×16 + 1×8 + 0×4 + 0×2 + 1×1 = 16 + 8 + 0 + 0 + 1 = 25  ✅
```

---

### 🔍 Ejemplo 3 — Convertir 100 a binario *(ejercicio de nivel medio)*

```
100 ÷ 2 = 50   residuo → 0
 50 ÷ 2 = 25   residuo → 0
 25 ÷ 2 = 12   residuo → 1
 12 ÷ 2 = 6    residuo → 0
  6 ÷ 2 = 3    residuo → 0
  3 ÷ 2 = 1    residuo → 1
  1 ÷ 2 = 0    residuo → 1
```

Leyendo de abajo hacia arriba: **1 1 0 0 1 0 0**

**Resultado:** 100₁₀ = **1100100₂**

**Verificación:**
```
1×64 + 1×32 + 0×16 + 0×8 + 1×4 + 0×2 + 0×1
= 64  +  32  +   0  +  0  +  4  +  0  +  0
= 100  ✅
```

---

## 3.2 Conversión: Binario → Decimal

### Método de las potencias de posición

**Regla de oro:** Multiplica cada dígito binario por su potencia de 2 según su posición, y suma todo.

```
Posición:   ...  4    3    2    1    0
Potencia:   ...  16   8    4    2    1
```

> ⚠️ **Importante:** La posición siempre se cuenta de **derecha a izquierda**, comenzando en 0.

---

### 🔍 Ejemplo 4 — Convertir 10110₂ a decimal

**Paso 1:** Coloca los dígitos con su posición:

```
Dígito:    1    0    1    1    0
Posición:  4    3    2    1    0
Potencia:  16   8    4    2    1
```

**Paso 2:** Multiplica dígito × potencia:

```
1 × 16 = 16
0 ×  8 =  0
1 ×  4 =  4
1 ×  2 =  2
0 ×  1 =  0
```

**Paso 3:** Suma todo:

```
16 + 0 + 4 + 2 + 0 = 22
```

**Resultado:** 10110₂ = **22₁₀** ✅

---

### 🔍 Ejemplo 5 — Convertir 11111111₂ a decimal *(¡el byte máximo!)*

```
Dígito:    1     1     1     1     1     1     1     1
Posición:  7     6     5     4     3     2     1     0
Potencia:  128   64    32    16    8     4     2     1
```

```
128 + 64 + 32 + 16 + 8 + 4 + 2 + 1 = 255
```

**Resultado:** 11111111₂ = **255₁₀**

> 💡 **¿Por qué 255?** Porque un byte tiene 8 bits y puede representar valores del 0 al 255. Por eso los colores RGB van de 0 a 255 en programas de diseño.

---

## 3.3 Ejercicios Paso a Paso — Binario

### 📝 Serie A — Decimal a Binario *(resuelta para guiar al estudiante)*

**Ejercicio A1:** Convertir **7** a binario.

```
7 ÷ 2 = 3   residuo → 1
3 ÷ 2 = 1   residuo → 1
1 ÷ 2 = 0   residuo → 1
```
**Respuesta:** 7₁₀ = **111₂**

---

**Ejercicio A2:** Convertir **18** a binario.

```
18 ÷ 2 = 9   residuo → 0
 9 ÷ 2 = 4   residuo → 1
 4 ÷ 2 = 2   residuo → 0
 2 ÷ 2 = 1   residuo → 0
 1 ÷ 2 = 0   residuo → 1
```
**Respuesta:** 18₁₀ = **10010₂**

---

**Ejercicio A3:** Convertir **45** a binario.

```
45 ÷ 2 = 22  residuo → 1
22 ÷ 2 = 11  residuo → 0
11 ÷ 2 = 5   residuo → 1
 5 ÷ 2 = 2   residuo → 1
 2 ÷ 2 = 1   residuo → 0
 1 ÷ 2 = 0   residuo → 1
```
**Respuesta:** 45₁₀ = **101101₂**

---

### 📝 Serie B — Binario a Decimal *(resuelta)*

**Ejercicio B1:** Convertir **1010₂** a decimal.

```
1×8 + 0×4 + 1×2 + 0×1 = 8 + 0 + 2 + 0 = 10
```
**Respuesta:** 1010₂ = **10₁₀**

---

**Ejercicio B2:** Convertir **110011₂** a decimal.

```
1×32 + 1×16 + 0×8 + 0×4 + 1×2 + 1×1
= 32 + 16 + 0 + 0 + 2 + 1 = 51
```
**Respuesta:** 110011₂ = **51₁₀**

---

**Ejercicio B3:** Convertir **1001010₂** a decimal.

```
Posición: 6    5    4    3    2    1    0
Dígito:   1    0    0    1    0    1    0
Potencia: 64   32   16   8    4    2    1

1×64 + 0×32 + 0×16 + 1×8 + 0×4 + 1×2 + 0×1
= 64 + 0 + 0 + 8 + 0 + 2 + 0 = 74
```
**Respuesta:** 1001010₂ = **74₁₀**

---

# BLOQUE 4 — Tabla Maestra de Conversiones

## 4. Tabla Maestra de Conversiones

> 📌 **Para el docente:** Esta tabla es el recurso central del aula. Se recomienda imprimirla en tamaño grande o proyectarla durante toda la clase.

| Decimal | Binario | Octal |
|---------|---------|-------|
| 0 | 0000 | 0 |
| 1 | 0001 | 1 |
| 2 | 0010 | 2 |
| 3 | 0011 | 3 |
| 4 | 0100 | 4 |
| 5 | 0101 | 5 |
| 6 | 0110 | 6 |
| 7 | 0111 | 7 |
| 8 | 1000 | 10 |
| 9 | 1001 | 11 |
| 10 | 1010 | 12 |
| 11 | 1011 | 13 |
| 12 | 1100 | 14 |
| 13 | 1101 | 15 |
| 14 | 1110 | 16 |
| 15 | 1111 | 17 |
| 16 | 10000 | 20 |
| 20 | 10100 | 24 |
| 24 | 11000 | 30 |
| 32 | 100000 | 40 |
| 64 | 1000000 | 100 |
| 128 | 10000000 | 200 |
| 255 | 11111111 | 377 |

> 🔎 **Actividad rápida (5 min):** Pide a los estudiantes que encuentren el patrón en los valores de la columna octal cuando el decimal salta de 7 a 8.

---

---

# ⏸️ DESCANSO 1 — 15 minutos

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║   🕐 DESCANSO — 15 MINUTOS                          ║
║                                                      ║
║   Han pasado 2 horas de trabajo intenso.             ║
║   ¡Es hora de recargar energías!                     ║
║                                                      ║
║   Sugerencias:                                       ║
║   • Estira los brazos y el cuello                    ║
║   • Toma agua                                        ║
║   • Aléjate de la pantalla o el cuaderno             ║
║                                                      ║
║   🔔 Regresamos en 15 minutos                       ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

> 📌 **Para el docente — Actividad de reconexión (3 min al regresar):**  
> Pide a un voluntario que convierta el número **20** a binario usando el método de divisiones, de memoria. El resto del grupo verifica. Esto activa la memoria antes de continuar.

---

---

# BLOQUE 5 — Sistema Octal *(40 min)*

## 6. El Sistema Octal — El atajo inteligente

### ¿Qué es y para qué sirve?

El sistema octal usa **8 como base** y únicamente emplea los dígitos del **0 al 7**. Fue muy popular en los primeros años de la informática porque permite representar números binarios largos de forma más compacta.

**Regla:** El dígito 8 y el 9 **no existen** en octal.

### ¿Dónde se usa hoy en día?

- **Permisos de archivos en Linux/Unix:** Cuando ves `chmod 755` o `chmod 644`, esos números son octales.
- **Sistemas embebidos** y microcontroladores.
- **Representación intermedia** entre binario y hexadecimal.

```bash
# Ejemplo real en Linux
chmod 755 archivo.sh
# 7 = rwx (leer, escribir, ejecutar) para el propietario
# 5 = r-x (leer y ejecutar) para el grupo
# 5 = r-x (leer y ejecutar) para otros
```

### Las potencias de 8

| Potencia | Valor |
|----------|-------|
| 8⁰ | 1 |
| 8¹ | 8 |
| 8² | 64 |
| 8³ | 512 |
| 8⁴ | 4,096 |

---

## 6.1 Conversión: Decimal → Octal

### Método de las divisiones sucesivas (igual que en binario, ¡pero dividiendo entre 8!)

---

### 🔍 Ejemplo 6 — Convertir 58 a octal

```
58 ÷ 8 = 7   residuo → 2
 7 ÷ 8 = 0   residuo → 7
              ↑ leer de aquí
```

Leyendo de abajo hacia arriba: **7 2**

**Resultado:** 58₁₀ = **72₈**

**Verificación:**
```
7×8¹ + 2×8⁰ = 56 + 2 = 58  ✅
```

---

### 🔍 Ejemplo 7 — Convertir 200 a octal

```
200 ÷ 8 = 25  residuo → 0
 25 ÷ 8 = 3   residuo → 1
  3 ÷ 8 = 0   residuo → 3
```

Leyendo de abajo hacia arriba: **3 1 0**

**Resultado:** 200₁₀ = **310₈**

**Verificación:**
```
3×64 + 1×8 + 0×1 = 192 + 8 + 0 = 200  ✅
```

---

### 🔍 Ejemplo 8 — Convertir 500 a octal

```
500 ÷ 8 = 62  residuo → 4
 62 ÷ 8 = 7   residuo → 6
  7 ÷ 8 = 0   residuo → 7
```

Leyendo de abajo hacia arriba: **7 6 4**

**Resultado:** 500₁₀ = **764₈**

**Verificación:**
```
7×512 + 6×64 + 4×8 + ... espera, revisemos posiciones:
7×64 + 6×8 + 4×1 = 448 + 48 + 4 = 500  ✅
```

---

## 6.2 Conversión: Octal → Decimal

### Método de las potencias de posición *(igual que en binario)*

---

### 🔍 Ejemplo 9 — Convertir 135₈ a decimal

```
Dígito:    1     3     5
Posición:  2     1     0
Potencia:  64    8     1
```

```
1×64 + 3×8 + 5×1 = 64 + 24 + 5 = 93
```

**Resultado:** 135₈ = **93₁₀** ✅

---

### 🔍 Ejemplo 10 — Convertir 4072₈ a decimal

```
Dígito:    4      0      7      2
Posición:  3      2      1      0
Potencia:  512    64     8      1
```

```
4×512 + 0×64 + 7×8 + 2×1
= 2048 + 0 + 56 + 2
= 2106
```

**Resultado:** 4072₈ = **2106₁₀** ✅

---

## 6.3 Conversión: Binario ↔ Octal — ¡El Truco Mágico!

Esta es la razón por la que el octal fue tan popular: **convertir entre binario y octal es extremadamente fácil**.

### El secreto: grupos de 3 bits

Cada dígito octal equivale exactamente a **3 bits** (porque 2³ = 8):

| Octal | Binario de 3 bits |
|-------|-------------------|
| 0 | 000 |
| 1 | 001 |
| 2 | 010 |
| 3 | 011 |
| 4 | 100 |
| 5 | 101 |
| 6 | 110 |
| 7 | 111 |

> 🧠 **Memoriza esta mini-tabla.** Es la clave para hacer conversiones en segundos.

---

### De Binario → Octal: agrupa de 3 en 3 desde la derecha

### 🔍 Ejemplo 11 — Convertir 110101₂ a octal

**Paso 1:** Agrupa en bloques de 3 bits desde la derecha:

```
110  101
```

**Paso 2:** Convierte cada grupo usando la mini-tabla:

```
110 → 6
101 → 5
```

**Resultado:** 110101₂ = **65₈** ✅

---

### 🔍 Ejemplo 12 — Convertir 10011110₂ a octal

**Paso 1:** Agrupa de derecha a izquierda (completa con ceros a la izquierda si es necesario):

```
010  011  110
 ↑ (se añade 0 al inicio para completar el grupo)
```

**Paso 2:** Convierte cada grupo:

```
010 → 2
011 → 3
110 → 6
```

**Resultado:** 10011110₂ = **236₈** ✅

**Verificación cruzada:**
```
10011110₂ = 128+16+8+4+2 = 158₁₀
236₈ = 2×64 + 3×8 + 6×1 = 128+24+6 = 158₁₀  ✅
```

---

### De Octal → Binario: cada dígito se convierte en 3 bits exactos

### 🔍 Ejemplo 13 — Convertir 537₈ a binario

**Paso 1:** Convierte cada dígito octal a su equivalente de 3 bits:

```
5 → 101
3 → 011
7 → 111
```

**Paso 2:** Concatena:

```
101 011 111
```

**Resultado:** 537₈ = **101011111₂** ✅

---

## 6.4 Ejercicios Paso a Paso — Octal

### 📝 Serie C — Decimal a Octal

**Ejercicio C1:** Convertir **33** a octal.

```
33 ÷ 8 = 4   residuo → 1
 4 ÷ 8 = 0   residuo → 4
```
**Respuesta:** 33₁₀ = **41₈**

---

**Ejercicio C2:** Convertir **150** a octal.

```
150 ÷ 8 = 18  residuo → 6
 18 ÷ 8 = 2   residuo → 2
  2 ÷ 8 = 0   residuo → 2
```
**Respuesta:** 150₁₀ = **226₈**

---

**Ejercicio C3:** Convertir **999** a octal.

```
999 ÷ 8 = 124  residuo → 7
124 ÷ 8 = 15   residuo → 4
 15 ÷ 8 = 1    residuo → 7
  1 ÷ 8 = 0    residuo → 1
```
**Respuesta:** 999₁₀ = **1747₈**

---

### 📝 Serie D — Binario ↔ Octal *(Truco de los grupos de 3)*

**Ejercicio D1:** Convertir **111000₂** a octal.

```
111  000
 7    0
```
**Respuesta:** 111000₂ = **70₈**

---

**Ejercicio D2:** Convertir **1010101₂** a octal.

```
001  010  101
(se agrega 0 al inicio)
 1    2    5
```
**Respuesta:** 1010101₂ = **125₈**

---

**Ejercicio D3:** Convertir **62₈** a binario.

```
6 → 110
2 → 010
```
**Respuesta:** 62₈ = **110010₂**

---

---

# ⏸️ DESCANSO 2 — 15 minutos

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║   🕐 DESCANSO — 15 MINUTOS                          ║
║                                                      ║
║   ¡Excelente trabajo! Han dominado dos sistemas      ║
║   numéricos. Ahora viene la parte más divertida:     ║
║   ¡van a convertirse en computadoras humanas! 🤖     ║
║                                                      ║
║   Mientras descansas, piensa:                        ║
║   ¿Cuántos bits necesitas para representar           ║
║   el número de tu salón de clases?                   ║
║                                                      ║
║   🔔 Regresamos en 15 minutos listos para jugar     ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

> 📌 **Para el docente — Actividad de reconexión:**  
> Al regresar, pide a dos estudiantes que conviertan el número 37 a binario usando el método del truco de grupos de 3 (primero a octal, luego a binario). Genera debate si los resultados difieren.

---

---

# BLOQUE 7 — Práctica Individual con Seguimiento *(20 min)*

## 8. Práctica Individual con Seguimiento

> 📌 **Para el docente:** Esta sección está diseñada para trabajo individual. Camina por el salón, observa los procesos y no solo los resultados. El error en el método es más informativo que el error en la respuesta final. Usa la **Rúbrica de Seguimiento** al final de esta sección.

---

### 🧪 Taller Individual — Hoja de Trabajo

**Instrucciones:** Resuelve cada ejercicio mostrando **todos los pasos**. No basta con la respuesta final.

---

#### Nivel 1 — Calentamiento

| # | Ejercicio | Tipo | Respuesta |
|---|-----------|------|-----------|
| 1 | Convertir **9₁₀** a binario | Dec → Bin | _______ |
| 2 | Convertir **1111₂** a decimal | Bin → Dec | _______ |
| 3 | Convertir **15₁₀** a octal | Dec → Oct | _______ |
| 4 | Convertir **17₈** a decimal | Oct → Dec | _______ |

---

#### Nivel 2 — En marcha

| # | Ejercicio | Tipo | Respuesta |
|---|-----------|------|-----------|
| 5 | Convertir **53₁₀** a binario | Dec → Bin | _______ |
| 6 | Convertir **101010₂** a decimal | Bin → Dec | _______ |
| 7 | Convertir **100₁₀** a octal | Dec → Oct | _______ |
| 8 | Convertir **111₂** a octal (truco de grupos) | Bin → Oct | _______ |

---

#### Nivel 3 — Desafío

| # | Ejercicio | Tipo | Respuesta |
|---|-----------|------|-----------|
| 9 | Convertir **255₁₀** a binario Y a octal | Dec → Bin y Oct | _______ |
| 10 | ¿Cuál es mayor: **11001₂** o **30₈**? Justifica. | Comparación | _______ |
| 11 | Un archivo de Linux tiene permiso **101 111 101₂**. ¿Cuál es su código octal? | Aplicación | _______ |
| 12 | Convertir **1011010110₂** a octal usando el truco de grupos | Bin → Oct | _______ |

---

### ✅ Respuestas del Taller Individual

> *(Para el docente — no mostrar hasta que los estudiantes terminen)*

| # | Respuesta Correcta | Proceso clave a verificar |
|---|--------------------|--------------------------|
| 1 | 1001₂ | 4 divisiones entre 2 |
| 2 | 15₁₀ | 8+4+2+1 |
| 3 | 17₈ | 1 división con residuos 7 y 1 |
| 4 | 15₁₀ | 1×8 + 7×1 |
| 5 | 110101₂ | 6 divisiones |
| 6 | 42₁₀ | 32+0+8+0+2+0 |
| 7 | 144₈ | 3 divisiones entre 8 |
| 8 | 7₈ | grupo: 111 → 7 |
| 9 | 11111111₂ / 377₈ | Ambas conversiones correctas |
| 10 | Son iguales: ambos = 25₁₀ | Conversión de ambos a decimal |
| 11 | 575₈ | 101→5, 111→7, 101→5 |
| 12 | 1326₈ | Grupos: 001 011 010 110 |

---

### 📊 Rúbrica de Seguimiento Docente

| Criterio | Excelente (4) | Bueno (3) | En Proceso (2) | Necesita Apoyo (1) |
|----------|---------------|-----------|----------------|--------------------|
| Método de división | Usa divisiones correctamente y sin errores | Pequeños errores aritméticos | Confunde la dirección de lectura | No recuerda el método |
| Lectura de residuos | Lee siempre de abajo hacia arriba | 1 error de dirección | Confunde regularmente | Dirección incorrecta siempre |
| Verificación | Verifica sus respuestas espontáneamente | Verifica si se le pide | Verifica con ayuda | No verifica |
| Truco Bin↔Oct | Aplica grupos de 3 sin ayuda | Necesita la mini-tabla | Confunde el tamaño del grupo | No comprende el truco |

---

# BLOQUE 8 — Juego de Roles *(30 min)*

## 9. 🎮 Juego de Roles — La Computadora Humana

> 🎯 **Objetivo:** Simular el funcionamiento de una CPU humana donde cada estudiante es un componente del proceso de conversión numérica.

---

### 📖 Contexto del Juego

> *"El año es 1960. Los ingenieros de IBM necesitan una computadora urgente, pero los transistores no llegan a tiempo. Han decidido usar... ¡estudiantes! Cada uno de ustedes es una parte del procesador. La misión: convertir números y no cometer errores o el cohete espacial se pierde."* 🚀

---

### 🎭 Los Roles

#### Configuración para grupos de 5–6 estudiantes:

---

**🟥 ROL 1: El Generador de Entrada**
- **Misión:** Escribir en una tarjeta el número decimal que la "computadora" debe procesar.
- **Restricción:** Solo puede escribir números entre 0 y 127.
- **Materiales:** Tarjetas de cartulina, marcador.

---

**🟦 ROL 2: El Divisor** *(x2 personas si el grupo es grande)*
- **Misión:** Recibir el número, aplicar el método de divisiones sucesivas.
- **Entrega:** Una hoja con todas las divisiones y los residuos anotados.
- **Frase del rol:** *"Procesando... división completada."*

---

**🟩 ROL 3: El Lector de Bits**
- **Misión:** Tomar la hoja del Divisor, leer los residuos de abajo hacia arriba y escribir el número binario en una tarjeta grande.
- **Entrega:** La tarjeta con el número binario.
- **Frase del rol:** *"Bits leídos. Transmitiendo señal binaria."*

---

**🟨 ROL 4: El Agrupador Octal**
- **Misión:** Tomar el número binario, agruparlo en bloques de 3 desde la derecha y convertirlo a octal.
- **Entrega:** La tarjeta con el número octal.
- **Frase del rol:** *"Comprimiendo datos a octal. Compresión exitosa."*

---

**🟪 ROL 5: El Verificador**
- **Misión:** Verificar que la cadena completa sea correcta usando la Tabla Maestra. Si hay error, activa la "alarma de error" (dice *"¡ERROR DE SISTEMA!"* y el proceso se reinicia).
- **Entrega:** Confirmación oral y escrita del resultado.
- **Frase del rol:** *"Verificación completa. Sistema operativo."* ✅

---

### 🕹️ Mecánica del Juego

#### Ronda 1 — Entrenamiento (5 min)
- El docente guía todo el proceso con el número **42**.
- Cada rol practica su función en voz alta.
- El Verificador confirma: 42₁₀ = 101010₂ = 52₈.

#### Ronda 2 — Primera Misión (8 min)
- El Generador crea un número.
- Cada rol ejecuta su función.
- El Verificador da el veredicto.
- **Condición de victoria:** Cero errores en la cadena.

#### Ronda 3 — Misión Inversa (8 min)
- El Generador ahora escribe un número **octal** (entre 10₈ y 177₈).
- El proceso se invierte: Octal → Binario → Decimal.
- Los roles se adaptan al proceso inverso.

#### Ronda 4 — Torneo (7 min)
- Dos grupos compiten en paralelo con el mismo número.
- Gana el grupo que llegue al resultado correcto primero.
- El Verificador de cada grupo confirma antes de declarar ganador.

---

### 🏆 Sistema de Puntuación

| Logro | Puntos |
|-------|--------|
| Completar la cadena sin errores | 10 pts |
| Verificador detecta un error real | 5 pts |
| Completar más rápido que el grupo rival | 3 pts extra |
| Corregir el error y recomenzar exitosamente | 5 pts |
| Todos los miembros pueden explicar su rol | 10 pts |

---

### 📝 Reflexión Post-Juego (5 min)

Al terminar el juego, el docente guía una reflexión rápida:

1. **¿Qué rol fue más difícil?** ¿Por qué?
2. **¿Qué pasó cuando el Verificador encontró un error?** ¿Cómo se sintió el equipo?
3. **Conexión real:** *"En una CPU real, si un bit llega incorrecto, todo el cálculo falla. ¿Cómo creen que las computadoras reales manejan los errores?"* (Pista: bits de paridad, checksums).
4. **¿Cuál fue el número más difícil de procesar?** ¿Por qué?

---

---

# BLOQUE 9 — Resumen y Cierre *(10 min)*

## 10. Resumen y Cierre

### Lo que aprendiste hoy

```
┌─────────────────────────────────────────────────────────┐
│                  MAPA DE LO APRENDIDO                   │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  SISTEMA DECIMAL          SISTEMA BINARIO               │
│  Base: 10                 Base: 2                       │
│  Dígitos: 0-9             Dígitos: 0, 1                 │
│  Uso: vida diaria         Uso: circuitos, CPU           │
│                                                         │
│  Conversión Dec→Bin:      Conversión Bin→Dec:           │
│  Dividir entre 2          Multiplicar por potencias     │
│  Leer residuos ↑          de 2 y sumar                  │
│                                                         │
│  SISTEMA OCTAL            TRUCO BINARIO ↔ OCTAL        │
│  Base: 8                  Grupos de 3 bits              │
│  Dígitos: 0-7             1 dígito octal = 3 bits       │
│  Uso: permisos Unix       Rápido y sin divisiones       │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

### Las 5 reglas de oro para recordar siempre

1. **Regla del 0 y el 1:** Todo en una computadora es binario; el resto de sistemas son solo formas más cómodas de leerlo.
2. **Regla de las divisiones:** Para convertir decimal a cualquier base, divide entre esa base y lee residuos de abajo hacia arriba.
3. **Regla de las potencias:** Para convertir a decimal desde cualquier base, multiplica cada dígito por su potencia de posición y suma.
4. **Regla de los grupos de 3:** Para pasar entre binario y octal, agrupa de 3 en 3 desde la derecha.
5. **Regla de la verificación:** Siempre verifica tu respuesta convirtiendo de vuelta al número original.

---

### Conexión con la vida real

| ¿Dónde lo ves? | Sistema que usa |
|----------------|----------------|
| Colores en CSS (#FF5733) | Hexadecimal (próxima clase) |
| Permisos en Linux (chmod 755) | Octal |
| Almacenamiento: 1 GB = 1024 MB | Binario (potencias de 2) |
| Dirección IP: 192.168.1.1 | Decimal (pero internamente binario) |
| Código ASCII de la letra 'A' | Decimal 65 = Binario 01000001 |

---

### Tarea para la próxima sesión

> *(Opcional — a criterio del docente)*

1. Convierte los dígitos de tu número de celular a binario (uno por uno).
2. Investiga: ¿Qué es el sistema hexadecimal y en qué se parece al octal?
3. Desafío: ¿Cuántos bits se necesitan para representar tu edad? ¿Y para representar el año actual?

---

### Autoevaluación del estudiante

Antes de salir, responde honestamente:

| Pregunta | 😕 Aún no | 🤔 Más o menos | 😊 Sí lo entiendo |
|----------|-----------|----------------|-------------------|
| ¿Puedo convertir de decimal a binario? | ☐ | ☐ | ☐ |
| ¿Puedo convertir de binario a decimal? | ☐ | ☐ | ☐ |
| ¿Puedo convertir de decimal a octal? | ☐ | ☐ | ☐ |
| ¿Entiendo el truco de grupos de 3? | ☐ | ☐ | ☐ |
| ¿Puedo explicarle esto a alguien más? | ☐ | ☐ | ☐ |

---

## Glosario

| Término | Definición |
|---------|-----------|
| **Base** | La cantidad de símbolos distintos que usa un sistema numérico |
| **Bit** | Dígito binario; la unidad mínima de información digital (0 o 1) |
| **Byte** | Grupo de 8 bits; puede representar 256 valores distintos |
| **Transistor** | Componente electrónico que funciona como interruptor; la base del hardware digital |
| **Sistema posicional** | Sistema donde el valor de un dígito depende de su posición dentro del número |
| **Residuo** | Lo que sobra después de una división entera |
| **Nibble** | Grupo de 4 bits; la mitad de un byte |
| **Potencia** | Resultado de multiplicar un número por sí mismo varias veces (ej. 2³ = 8) |
| **Octal** | Sistema de base 8; usa dígitos del 0 al 7 |
| **Binario** | Sistema de base 2; solo usa 0 y 1 |
| **Decimal** | Sistema de base 10; el que usamos en la vida cotidiana |

---

## Referencias y Recursos Adicionales

- 📖 **Libro:** Mano, M. M. (2003). *Diseño Digital*. Pearson Educación.
- 🌐 **Herramienta online:** [RapidTables — Number Conversion](https://www.rapidtables.com/convert/number/)
- 🎮 **Práctica interactiva:** [CS Unplugged — Binary Numbers](https://csunplugged.org/en/topics/binary-numbers/)
- 📺 **Video:** Busca en YouTube: *"Sistema binario para principiantes"* o *"How computers work: Binary"* (CrashCourse)

---

> **Nota para el docente:** Este material está diseñado bajo el enfoque de aprendizaje activo y gamificación. Se recomienda adaptar el ritmo según el grupo. El juego de roles puede extenderse si el grupo muestra alto engagement, reduciendo el tiempo de resumen. Los ejercicios del Nivel 3 en la práctica individual son opcionales para estudiantes avanzados.

---

*Material educativo de libre uso. Creado para aprendizaje de sistemas digitales — Nivel secundaria.*

