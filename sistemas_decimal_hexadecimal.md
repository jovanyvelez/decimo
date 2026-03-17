# 🎨 Sistemas Numérico: Decimal y Hexadecimal

> **Nivel:** Secundaria (15–16 años)
> **Duración total:** 4 horas (2 sesiones de descanso de 15 min c/u)
> **Prerequisito recomendado:** Conocimiento básico de sistema binario y octal
> **Temas:** Sistema Decimal · Sistema Hexadecimal · Conversiones cruzadas · Aplicaciones reales

---

## Tabla de Contenidos

1. [¿Por qué necesitamos el hexadecimal?](#1-por-qué-necesitamos-el-hexadecimal)
2. [Repaso del Sistema Decimal](#2-repaso-del-sistema-decimal)
3. [El Sistema Hexadecimal](#3-el-sistema-hexadecimal)
4. [Tabla Maestra de Conversiones](#4-tabla-maestra-de-conversiones)
5. [Conversiones: Decimal → Hexadecimal](#5-conversiones-decimal--hexadecimal)
6. [Conversiones: Hexadecimal → Decimal](#6-conversiones-hexadecimal--decimal)
7. [DESCANSO 1 — 15 minutos](#descanso-1--15-minutos)
8. [Conversiones Cruzadas con Binario](#8-conversiones-cruzadas-con-binario)
9. [Interpretación de Valores en Distintos Formatos](#9-interpretación-de-valores-en-distintos-formatos)
10. [DESCANSO 2 — 15 minutos](#descanso-2--15-minutos)
11. [Taller Práctico](#11-taller-práctico)
12. [Resumen y Cierre](#12-resumen-y-cierre)
13. [Glosario](#glosario)

---

## Guía de Tiempos para el Docente

| Bloque | Actividad | Duración |
|--------|-----------|----------|
| Bloque 1 | Introducción + Repaso Decimal | 20 min |
| Bloque 2 | Sistema Hexadecimal — teoría y tabla | 30 min |
| Bloque 3 | Conversión Decimal → Hex (ejemplos) | 30 min |
| Bloque 4 | Conversión Hex → Decimal (ejemplos) | 25 min |
| Bloque 5 | Ejercicios guiados + verificación cruzada | 15 min |
| **DESCANSO 1** | | **15 min** |
| Bloque 6 | Conversiones cruzadas con Binario (Hex ↔ Bin) | 35 min |
| Bloque 7 | Interpretación de valores en distintos formatos | 30 min |
| **DESCANSO 2** | | **15 min** |
| Bloque 8 | Taller práctico (individual + parejas) | 45 min |
| Bloque 9 | Socialización y corrección del taller | 15 min |
| Bloque 10 | Resumen y cierre | 10 min |
| **TOTAL** | | **4 h 15 min aprox.** |

> **Nota para el docente:** El Descanso 2 se ubica estratégicamente entre la parte teórica de interpretación y el taller práctico, justo cuando los estudiantes han asimilado todo el contenido conceptual y necesitan un corte antes del bloque más intenso de trabajo individual.

---

# BLOQUE 1 — Introducción (20 min)

## 1. ¿Por qué necesitamos el hexadecimal?

Imagina que eres programador y tienes que representar el color rojo exacto de la camiseta del equipo de fútbol de tu colegio. En el mundo digital, ese rojo no es simplemente "rojo": es una combinación de tres valores numéricos entre 0 y 255 que indican cuánta luz roja, verde y azul debe mezclar tu pantalla.

El problema: **el número 255 en binario se escribe `11111111`**. Ahora imagina tener que escribir tres de esos números para cada color, en cada pixel de una imagen de 4K. Serían miles de millones de unos y ceros. Imposible de leer para un humano.

La solución que inventaron los ingenieros de los años 60: **el sistema hexadecimal**. Con él, ese `11111111` binario se convierte simplemente en `FF`. Dos caracteres en lugar de ocho.

### El hexadecimal está en todas partes

| Donde lo ves | Ejemplo real |
|-------------|-------------|
| Colores en páginas web | `#FF5733` (naranja vibrante) |
| Direcciones de memoria RAM | `0x7FFF5FBD` |
| Direcciones MAC de red | `A4:C3:F0:85:AC:2D` |
| Códigos de error en Windows | `0x0000007E` |
| Huellas digitales de archivos (hash) | `5d41402abc4b2a76b9719d911017c592` |
| Editores hexadecimales | `48 65 6C 6C 6F` = "Hello" |

> **Reto de apertura (5 min):** ¿Alguien sabe qué color es `#1A237E`? ¿Y `#FFFFFF`? ¿Y `#000000`?
> Respuestas: azul oscuro / blanco / negro.

---

# BLOQUE 2 — El Sistema Hexadecimal (30 min)

## 2. Repaso del Sistema Decimal

Antes de entrar al hexadecimal, recordemos la estructura del sistema decimal con un ejemplo que usaremos como puente.

El número **2,748** en decimal:

```
Dígito:     2       7       4       8
Posición:   3       2       1       0
Potencia:  10³     10²     10¹     10⁰
Valor:    1000     100      10       1

(2×1000) + (7×100) + (4×10) + (8×1) = 2,748
```

**La clave:** en cualquier sistema posicional, cada posición vale (base)^posición. Esto no cambia nunca, solo cambia la base.

---

## 3. El Sistema Hexadecimal

El sistema hexadecimal usa **16 como base**. Aquí viene el primer reto: con los dígitos del 0 al 9 solo tenemos 10 símbolos, pero necesitamos 16. La solución fue incorporar las primeras seis letras del abecedario.

### La tabla de símbolos hexadecimales

| Valor decimal | Símbolo hexadecimal | Nombre |
|:---:|:---:|:---|
| 0 | 0 | Cero |
| 1 | 1 | Uno |
| 2 | 2 | Dos |
| 3 | 3 | Tres |
| 4 | 4 | Cuatro |
| 5 | 5 | Cinco |
| 6 | 6 | Seis |
| 7 | 7 | Siete |
| 8 | 8 | Ocho |
| 9 | 9 | Nueve |
| 10 | **A** | "Diez" |
| 11 | **B** | "Once" |
| 12 | **C** | "Doce" |
| 13 | **D** | "Trece" |
| 14 | **E** | "Catorce" |
| 15 | **F** | "Quince" |

> **¡Atención!** Las letras A, B, C, D, E y F son dígitos, no letras. `1F` en hexadecimal NO es "uno F": es un número de dos dígitos cuyo segundo dígito vale 15.

### Las potencias de 16

| Potencia | Valor | Nota |
|----------|-------|------|
| 16⁰ | 1 | Unidades |
| 16¹ | 16 | "Dieciseisenas" |
| 16² | 256 | (= 2 bytes = 1 palabra) |
| 16³ | 4,096 | |
| 16⁴ | 65,536 | (= 64 KB) |
| 16⁵ | 1,048,576 | (= 1 MB) |

> **Truco para recordar:** 16⁰=1, 16¹=16, 16²=256 son los más usados. Nota que 256 = 2⁸ = el número de valores que cabe en un byte. No es coincidencia: por eso el hex y los bytes son inseparables.

### ¿Cómo se escribe un número hexadecimal?

Para evitar confusiones, los números hexadecimales se escriben de dos formas:
- Con subíndice 16: `3B₁₆`
- Con prefijo `0x` (en programación): `0x3B`
- Con sufijo `h` (en ensamblador): `3Bh`

En esta guía usaremos la notación `₁₆` para mayor claridad.

---

## 4. Tabla Maestra de Conversiones

> Para el docente: Esta tabla es el recurso de referencia durante toda la sesión. Proyectarla o imprimirla en formato grande es altamente recomendado.

| Decimal | Hexadecimal | Binario | Octal |
|:---:|:---:|:---:|:---:|
| 0 | 0 | 0000 | 0 |
| 1 | 1 | 0001 | 1 |
| 2 | 2 | 0010 | 2 |
| 3 | 3 | 0011 | 3 |
| 4 | 4 | 0100 | 4 |
| 5 | 5 | 0101 | 5 |
| 6 | 6 | 0110 | 6 |
| 7 | 7 | 0111 | 7 |
| 8 | 8 | 1000 | 10 |
| 9 | 9 | 1001 | 11 |
| 10 | **A** | 1010 | 12 |
| 11 | **B** | 1011 | 13 |
| 12 | **C** | 1100 | 14 |
| 13 | **D** | 1101 | 15 |
| 14 | **E** | 1110 | 16 |
| 15 | **F** | 1111 | 17 |
| 16 | 10 | 0001 0000 | 20 |
| 17 | 11 | 0001 0001 | 21 |
| 31 | 1F | 0001 1111 | 37 |
| 32 | 20 | 0010 0000 | 40 |
| 48 | 30 | 0011 0000 | 60 |
| 63 | 3F | 0011 1111 | 77 |
| 64 | 40 | 0100 0000 | 100 |
| 100 | 64 | 0110 0100 | 144 |
| 127 | 7F | 0111 1111 | 177 |
| 128 | 80 | 1000 0000 | 200 |
| 160 | A0 | 1010 0000 | 240 |
| 192 | C0 | 1100 0000 | 300 |
| 200 | C8 | 1100 1000 | 310 |
| 255 | **FF** | 1111 1111 | 377 |

> **Observaciones importantes para discutir en clase:**
> - ¿Por qué el 16 decimal se escribe "10" en hex? (Porque 16 = 1×16¹ + 0×16⁰)
> - ¿Por qué el 255 decimal es "FF" en hex? (F=15; 15×16 + 15×1 = 240 + 15 = 255)
> - ¿Por qué los programadores aman el 255? (Es el máximo de un byte de 8 bits)

---

# BLOQUE 3 — Conversión Decimal → Hexadecimal (30 min)

## 5. Conversiones: Decimal → Hexadecimal

### El método: divisiones sucesivas entre 16

**Regla de oro:** igual que con binario (dividir entre 2) y con octal (dividir entre 8), pero ahora dividimos entre **16**. Los residuos se leen de abajo hacia arriba, y si el residuo es 10 o más, se escribe su letra equivalente.

---

### Ejemplo 1 — Convertir 75 a hexadecimal

**Paso 1:** Divide entre 16 y anota cociente y residuo.

```
75 ÷ 16 = 4    residuo → 11  →  B   (11 en decimal = B en hex)
 4 ÷ 16 = 0    residuo →  4  →  4
               ↑ leer de aquí
```

**Paso 2:** Leer los residuos de abajo hacia arriba: **4B**

**Resultado:** 75₁₀ = **4B₁₆**

**Verificación:**
```
4×16¹ + B×16⁰
= 4×16 + 11×1
= 64   + 11
= 75  ✓
```

---

### Ejemplo 2 — Convertir 200 a hexadecimal

```
200 ÷ 16 = 12   residuo → 8   →   8
 12 ÷ 16 =  0   residuo → 12  →   C
               ↑ leer de aquí
```

**Resultado:** 200₁₀ = **C8₁₆**

**Verificación:**
```
C×16¹ + 8×16⁰
= 12×16 + 8×1
= 192   + 8
= 200  ✓
```

---

### Ejemplo 3 — Convertir 3,500 a hexadecimal (número grande)

```
3500 ÷ 16 = 218   residuo → 12  →  C
 218 ÷ 16 =  13   residuo → 10  →  A
  13 ÷ 16 =   0   residuo → 13  →  D
                  ↑ leer de aquí
```

**Resultado:** 3500₁₀ = **DAC₁₆**

**Verificación:**
```
D×16² + A×16¹ + C×16⁰
= 13×256 + 10×16 + 12×1
= 3328   + 160   + 12
= 3500  ✓
```

---

### Ejemplo 4 — Convertir 65,535 a hexadecimal (máximo de 2 bytes)

```
65535 ÷ 16 = 4095   residuo → 15  →  F
 4095 ÷ 16 =  255   residuo → 15  →  F
  255 ÷ 16 =   15   residuo → 15  →  F
   15 ÷ 16 =    0   residuo → 15  →  F
                    ↑ leer de aquí
```

**Resultado:** 65535₁₀ = **FFFF₁₆**

> **Dato clave:** FFFF es el número hexadecimal de 4 dígitos más grande. Equivale a 65,535 en decimal, que es el máximo valor que puede almacenar un número entero sin signo de 16 bits (2 bytes). Por eso en programación el tipo de dato `unsigned short` va de 0 a 65,535.

---

### Ejemplo 5 — Convertir 255 a hexadecimal (el byte más importante)

```
255 ÷ 16 = 15   residuo → 15  →  F
 15 ÷ 16 =  0   residuo → 15  →  F
               ↑ leer de aquí
```

**Resultado:** 255₁₀ = **FF₁₆**

> Este es el resultado más importante de memorizar. En diseño gráfico y web, cuando el rojo de un color RGB está al máximo (255), se escribe `FF`. El blanco puro es `#FFFFFF` porque los tres canales (rojo, verde, azul) están al máximo.

---

### Ejercicios de práctica guiada — Decimal a Hexadecimal

> Para el docente: resuelva estos ejercicios en el tablero, invitando a los estudiantes a decir cada paso en voz alta.

**Ejercicio G1:** Convertir **29** a hex.

```
29 ÷ 16 = 1   residuo → 13  →  D
 1 ÷ 16 = 0   residuo →  1  →  1
```
**Respuesta:** 29₁₀ = **1D₁₆**  — Verificación: 1×16 + 13 = 16 + 13 = 29 ✓

---

**Ejercicio G2:** Convertir **256** a hex.

```
256 ÷ 16 = 16   residuo → 0  →  0
 16 ÷ 16 =  1   residuo → 0  →  0
  1 ÷ 16 =  0   residuo → 1  →  1
```
**Respuesta:** 256₁₀ = **100₁₆**  — Verificación: 1×256 + 0 + 0 = 256 ✓

> **¿Por qué 256 es "100" en hex?** Porque 256 = 16², exactamente igual a como 100 en decimal es 10². El "1" ocupa la posición de 16².

---

# BLOQUE 4 — Conversión Hexadecimal → Decimal (25 min)

## 6. Conversiones: Hexadecimal → Decimal

### El método: potencias de posición

**Regla de oro:** multiplica cada dígito hexadecimal por 16 elevado a su posición (de derecha a izquierda desde 0), recordando que A=10, B=11, C=12, D=13, E=14, F=15. Luego suma todo.

---

### Ejemplo 6 — Convertir 2F₁₆ a decimal

```
Dígito:     2       F
Posición:   1       0
Potencia:  16¹     16⁰
              16      1
```

```
2×16 + F×1
= 2×16 + 15×1
= 32   + 15
= 47
```

**Resultado:** 2F₁₆ = **47₁₀** ✓

---

### Ejemplo 7 — Convertir A3₁₆ a decimal

```
A×16¹ + 3×16⁰
= 10×16 + 3×1
= 160   + 3
= 163
```

**Resultado:** A3₁₆ = **163₁₀** ✓

---

### Ejemplo 8 — Convertir 1B4₁₆ a decimal (3 dígitos)

```
Dígito:     1       B       4
Posición:   2       1       0
Potencia:  16²     16¹     16⁰
            256      16       1
```

```
1×256 + B×16 + 4×1
= 1×256 + 11×16 + 4×1
= 256   + 176   + 4
= 436
```

**Resultado:** 1B4₁₆ = **436₁₀** ✓

---

### Ejemplo 9 — Convertir FF00₁₆ a decimal (color con transparencia)

```
F×16³ + F×16² + 0×16¹ + 0×16⁰
= 15×4096 + 15×256 + 0 + 0
= 61440   + 3840
= 65280
```

**Resultado:** FF00₁₆ = **65280₁₀** ✓

> **Contexto real:** En algunos sistemas de color con transparencia (ARGB), los primeros dos dígitos hex representan la opacidad. `FF00` podría ser rojo al 100% de opacidad sin componente verde ni azul, dependiendo del formato.

---

### Ejemplo 10 — Convertir DEAD₁₆ a decimal (una dirección clásica)

```
D×16³ + E×16² + A×16¹ + D×16⁰
= 13×4096 + 14×256 + 10×16 + 13×1
= 53248   + 3584   + 160   + 13
= 57005
```

**Resultado:** DEAD₁₆ = **57005₁₀** ✓

> **Nota curiosa:** Los programadores usan "DEAD", "BEEF", "CAFE", "BABE" como marcadores en memoria porque son palabras reales en inglés. Son fáciles de identificar en un volcado de memoria hexadecimal cuando algo falla.

---

### Ejercicios de práctica guiada — Hexadecimal a Decimal

**Ejercicio G3:** Convertir **3C₁₆** a decimal.

```
3×16 + C×1 = 3×16 + 12×1 = 48 + 12 = 60
```
**Respuesta:** 3C₁₆ = **60₁₀** ✓

---

**Ejercicio G4:** Convertir **B0₁₆** a decimal.

```
B×16 + 0×1 = 11×16 + 0 = 176 + 0 = 176
```
**Respuesta:** B0₁₆ = **176₁₀** ✓

---

**Ejercicio G5:** Convertir **7FF₁₆** a decimal.

```
7×256 + F×16 + F×1
= 7×256 + 15×16 + 15×1
= 1792  + 240   + 15
= 2047
```
**Respuesta:** 7FF₁₆ = **2047₁₀** ✓

---

# DESCANSO 1 — 15 minutos

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║   DESCANSO — 15 MINUTOS                              ║
║                                                      ║
║   Han pasado 2 horas de trabajo intenso.             ║
║   Momento de recargar energías.                      ║
║                                                      ║
║   Sugerencias:                                       ║
║   - Estira cuello, muñecas y espalda                 ║
║   - Toma agua o come algo ligero                     ║
║   - Aléjate del cuaderno por completo                ║
║                                                      ║
║   Regresamos en 15 minutos                           ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

> **Para el docente — Actividad de reconexión (5 min al regresar):**
>
> Antes de continuar, escribe en el tablero el código de color `#FF6B35` y pregunta:
> - ¿Cuánto vale el canal rojo? (FF = 255)
> - ¿Cuánto vale el canal verde? (6B = ?)
> - ¿Cuánto vale el canal azul? (35 = ?)
>
> Que los estudiantes resuelvan en parejas la conversión de 6B y 35 como activación.
> Respuestas: 6B₁₆ = 107₁₀ · 35₁₆ = 53₁₀

---

# BLOQUE 6 — Conversiones Cruzadas con Binario (35 min)

## 8. Conversiones Cruzadas con Binario

Esta es la razón más poderosa por la que el hexadecimal existe: **convertir entre binario y hexadecimal es casi inmediato**, sin necesidad de divisiones.

### El secreto: grupos de 4 bits

Cada dígito hexadecimal equivale exactamente a **4 bits** (porque 2⁴ = 16):

| Hex | Binario 4 bits | Hex | Binario 4 bits |
|:---:|:---:|:---:|:---:|
| 0 | 0000 | 8 | 1000 |
| 1 | 0001 | 9 | 1001 |
| 2 | 0010 | A | 1010 |
| 3 | 0011 | B | 1011 |
| 4 | 0100 | C | 1100 |
| 5 | 0101 | D | 1101 |
| 6 | 0110 | E | 1110 |
| 7 | 0111 | F | 1111 |

> **Memoriza esta tabla.** Es la clave de toda la informática práctica: 1 dígito hex = 4 bits exactos = 1 nibble.

---

### De Binario → Hexadecimal: agrupa de 4 en 4 desde la derecha

### Ejemplo 11 — Convertir 11010110₂ a hex

**Paso 1:** Agrupa en bloques de 4 bits desde la derecha:

```
1101  0110
```

**Paso 2:** Convierte cada grupo con la mini-tabla:

```
1101 → D
0110 → 6
```

**Resultado:** 11010110₂ = **D6₁₆** ✓

**Verificación cruzada:**
```
11010110₂ = 128+64+0+16+0+4+2+0 = 214₁₀
D6₁₆ = 13×16 + 6×1 = 208 + 6 = 214₁₀  ✓
```

---

### Ejemplo 12 — Convertir 101111000011₂ a hex (12 bits)

**Paso 1:** Agrupa de 4 en 4 desde la derecha:

```
1011  1100  0011
```

**Paso 2:** Convierte cada grupo:

```
1011 → B
1100 → C
0011 → 3
```

**Resultado:** 101111000011₂ = **BC3₁₆** ✓

**Verificación:**
```
B×256 + C×16 + 3×1
= 11×256 + 12×16 + 3
= 2816  + 192   + 3
= 3011₁₀

Y en binario: 2048+512+256+128+64+0+0+0+0+0+1+0+0+0+1+1 = 3011₁₀ ✓
```

---

### De Hexadecimal → Binario: cada dígito se expande a 4 bits exactos

### Ejemplo 13 — Convertir 5A₁₆ a binario

**Paso 1:** Convierte cada dígito hex a su grupo de 4 bits:

```
5 → 0101
A → 1010
```

**Paso 2:** Concatena:

```
0101 1010
```

**Resultado:** 5A₁₆ = **01011010₂**

> Nota: el cero a la izquierda se mantiene para completar el grupo de 4 bits.

---

### Ejemplo 14 — Convertir FF₁₆ a binario

```
F → 1111
F → 1111
```

**Resultado:** FF₁₆ = **11111111₂**

> Este es el byte completo con todos los bits en 1. Es el número más conocido de la informática: 255 en decimal, FF en hex, 11111111 en binario, 377 en octal. Cuatro formas de escribir el mismo valor.

---

### Ejemplo 15 — Convertir 0xCAFE a binario (clásico de programación)

```
C → 1100
A → 1010
F → 1111
E → 1110
```

**Resultado:** CAFE₁₆ = **1100 1010 1111 1110₂**

**Verificación:**
```
12×4096 + 10×256 + 15×16 + 14×1
= 49152  + 2560  + 240   + 14
= 51966₁₀
```

---

### Ejercicios de práctica — Conversión cruzada Bin ↔ Hex

**Ejercicio C1:** Convertir **10101010₂** a hex.

```
1010  1010
 A     A
→ AA₁₆
```
Verificación: 10×16 + 10 = 160 + 10 = 170₁₀ · En binario: 128+32+8+2 = 170₁₀ ✓

---

**Ejercicio C2:** Convertir **3F₁₆** a binario.

```
3 → 0011
F → 1111
→ 00111111₂
```
Verificación: 32+16+8+4+2+1 = 63₁₀ · 3×16+15 = 63₁₀ ✓

---

**Ejercicio C3:** Convertir **11001110 01011010₂** (16 bits) a hex.

```
1100  1110  0101  1010
 C     E     5     A
→ CE5A₁₆
```

---

# BLOQUE 7 — Interpretación de Valores en Distintos Formatos (30 min)

## 9. Interpretación de Valores en Distintos Formatos

Esta sección responde una pregunta fundamental: dado un valor numérico, **¿qué significa en contexto?** Un mismo número puede representar un color, una dirección de memoria, un carácter de texto o una instrucción de máquina, dependiendo de dónde aparezca.

---

### 9.1 Los Colores RGB y el Hexadecimal

Un color en pantalla se define con tres componentes: Rojo (R), Verde (G) y Azul (B), cada uno entre 0 y 255. En formato hexadecimal, cada componente ocupa exactamente 2 dígitos hex (un byte).

```
Color = #RRGGBB
         ||||||
         ||++++-- Azul: 00 a FF (0 a 255)
         ++------ Verde: 00 a FF
 Rojo: 00 a FF --+
```

**Ejemplos descodificados:**

| Código Hex | Rojo | Verde | Azul | Color |
|:---:|:---:|:---:|:---:|:---:|
| #FF0000 | 255 | 0 | 0 | Rojo puro |
| #00FF00 | 0 | 255 | 0 | Verde puro |
| #0000FF | 0 | 0 | 255 | Azul puro |
| #FFFFFF | 255 | 255 | 255 | Blanco |
| #000000 | 0 | 0 | 0 | Negro |
| #FF6B35 | 255 | 107 | 53 | Naranja |
| #1A237E | 26 | 35 | 126 | Azul índigo oscuro |
| #2ECC71 | 46 | 204 | 113 | Verde esmeralda |

> **Actividad (5 min):** Cada estudiante elige el color de su camiseta favorita y busca (o estima) su código hex. Luego lo descompone en sus tres componentes RGB decimales.

---

### Cómo descifrar cualquier código de color

**Ejercicio resuelto:** ¿Qué color es `#A020F0`?

```
A0₁₆ = 10×16 + 0×1 = 160  → Rojo:  160
20₁₆ =  2×16 + 0×1 =  32  → Verde:  32
F0₁₆ = 15×16 + 0×1 = 240  → Azul:  240
```

Mucho azul, bastante rojo, poco verde → **Púrpura / Violeta** ✓

---

### 9.2 Los Códigos ASCII — Cómo el texto se convierte en números

El estándar ASCII asigna un número a cada carácter del teclado. Las computadoras almacenan el texto como secuencias de esos números, y el hexadecimal es la forma más compacta de verlos.

| Carácter | Decimal | Hexadecimal | Binario |
|:---:|:---:|:---:|:---:|
| 'A' | 65 | 41 | 0100 0001 |
| 'B' | 66 | 42 | 0100 0010 |
| 'Z' | 90 | 5A | 0101 1010 |
| 'a' | 97 | 61 | 0110 0001 |
| 'z' | 122 | 7A | 0111 1010 |
| '0' | 48 | 30 | 0011 0000 |
| '9' | 57 | 39 | 0011 1001 |
| espacio | 32 | 20 | 0010 0000 |
| '!' | 33 | 21 | 0010 0001 |

> **Patrón a descubrir:** ¿Notas que entre 'A' (65) y 'a' (97) hay exactamente 32 de diferencia? Eso es porque en binario, pasar de mayúscula a minúscula solo cambia un bit (el bit 5). Los diseñadores del ASCII lo hicieron así deliberadamente.

---

### Descifrar un mensaje en hexadecimal — Actividad grupal (10 min)

Los siguientes valores hexadecimales representan un mensaje en código ASCII. Conviértelos a decimal y busca el carácter correspondiente.

**Mensaje cifrado:**
```
48  6F  6C  61  20  4D  75  6E  64  6F
```

**Proceso de decodificación:**

| Hex | Decimal | Carácter |
|:---:|:---:|:---:|
| 48 | 4×16 + 8 = 72 | H |
| 6F | 6×16 + 15 = 111 | o |
| 6C | 6×16 + 12 = 108 | l |
| 61 | 6×16 + 1 = 97 | a |
| 20 | 2×16 + 0 = 32 | (espacio) |
| 4D | 4×16 + 13 = 77 | M |
| 75 | 7×16 + 5 = 117 | u |
| 6E | 6×16 + 14 = 110 | n |
| 64 | 6×16 + 4 = 100 | d |
| 6F | 6×16 + 15 = 111 | o |

**Mensaje:** `Hola Mundo`

---

### 9.3 Direcciones de Memoria y Errores del Sistema

Las direcciones de memoria RAM se escriben en hexadecimal porque son compactas y se alinean perfectamente con la arquitectura binaria del hardware.

**Lectura de un volcado de memoria (Memory Dump):**

```
Dirección  | Contenido Hex          | Interpretación ASCII
-----------+------------------------+---------------------
0x00400000 | 48 65 6C 6C 6F 20 57  | Hello W
0x00400007 | 6F 72 6C 64 00 00 00  | orld...
```

- Las direcciones (`0x00400000`) indican la posición en memoria.
- Los valores son bytes en hexadecimal.
- La columna ASCII muestra cómo se ven si se interpretan como texto.
- Los `00` son bytes vacíos (valor cero).

**Códigos de error de Windows (Stop Codes):**

| Código hex | Significado |
|:---:|:---|
| `0x0000007E` | Error de sistema — excepción no manejada |
| `0x000000D1` | Problema con driver de hardware |
| `0x000000A5` | Error en BIOS o ACPI |
| `0xC0000005` | Acceso a memoria no permitida |

Todos esos números enormes son simplemente hexadecimales que se pueden convertir a decimal o binario con el método que ya aprendiste.

---

### 9.4 Comparación completa: el mismo valor en cuatro sistemas

El siguiente cuadro muestra el valor **255** (el byte máximo) visto desde cada sistema:

| Sistema | Representación | Interpretación |
|:---:|:---:|:---|
| Decimal | 255 | Doscientos cincuenta y cinco |
| Binario | 11111111 | Ocho bits, todos en 1 |
| Octal | 377 | Tres dígitos octales |
| Hexadecimal | FF | Dos dígitos hex, máximo valor de un byte |
| Color (R) | #FF0000 | Rojo al máximo, sin verde ni azul |
| ASCII | — | No es un carácter ASCII estándar |
| En 2 bytes | 0x00FF | Byte alto = 0, Byte bajo = 255 |

> **Reflexión:** ¿Cuál es la forma más útil? Depende del contexto. Un diseñador prefiere hex. Un electricista prefiere binario. Un usuario normal prefiere decimal. Un ingeniero de sistemas usa los cuatro.

---

# DESCANSO 2 — 15 minutos

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║   DESCANSO — 15 MINUTOS                              ║
║                                                      ║
║   Excelente trabajo. Han dominado el sistema         ║
║   hexadecimal y sus conversiones cruzadas.           ║
║                                                      ║
║   Ahora viene el taller práctico donde               ║
║   aplicarán todo lo aprendido.                       ║
║                                                      ║
║   Pregunta para reflexionar en el descanso:          ║
║   ¿De qué color es #FF00FF?                          ║
║   (respuesta al regresar)                            ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

> **Para el docente — Al regresar:**
> Responder la pregunta del descanso: `#FF00FF` = Rojo 255, Verde 0, Azul 255 = **Magenta / Fucsia**.
> Luego anunciar las instrucciones del taller. Organizar los grupos si el taller incluye trabajo en parejas.

---

# BLOQUE 8 — Taller Práctico (45 min)

## 11. Taller Práctico

> **Para el docente:** Este taller tiene tres partes. La Parte A es individual (15 min), la Parte B es en parejas con verificación cruzada (15 min), y la Parte C es un desafío de aplicación real en grupos de 3 (15 min). Monitorear el proceso, no solo el resultado.

---

### PARTE A — Trabajo Individual (15 min)

> **Instrucciones:** Resuelve cada ejercicio mostrando todos los pasos del proceso. La respuesta sin procedimiento no se cuenta.

---

#### Sección 1 — Decimal a Hexadecimal

**A1.** Convertir **45₁₀** a hexadecimal.

*Espacio de trabajo:*
```
_____ ÷ 16 = _____  residuo → _____  →  ___
_____ ÷ 16 = _____  residuo → _____  →  ___

Resultado: ___________

Verificación: ___ × ___ + ___ × ___ = ___________
```

**A2.** Convertir **173₁₀** a hexadecimal.

*Espacio de trabajo:*
```
_____ ÷ 16 = _____  residuo → _____  →  ___
_____ ÷ 16 = _____  residuo → _____  →  ___

Resultado: ___________

Verificación: ___ × ___ + ___ × ___ = ___________
```

**A3.** Convertir **1000₁₀** a hexadecimal.

*Espacio de trabajo:*
```
_______ ÷ 16 = _______  residuo → _____  →  ___
_______ ÷ 16 = _______  residuo → _____  →  ___
_______ ÷ 16 = _______  residuo → _____  →  ___

Resultado: ___________

Verificación: ___ × ___ + ___ × ___ + ___ × ___ = ___________
```

---

#### Sección 2 — Hexadecimal a Decimal

**A4.** Convertir **7A₁₆** a decimal.

*Espacio de trabajo:*
```
___ × 16¹  +  ___ × 16⁰
= ___ × 16 + ___ × 1
= _______  + _______
= ___________
```

**A5.** Convertir **2BC₁₆** a decimal.

*Espacio de trabajo:*
```
___ × 16²  +  ___ × 16¹  +  ___ × 16⁰
= ___ × 256 + ___ × 16  + ___ × 1
= _______   + _______   + _______
= ___________
```

**A6.** Convertir **F0F₁₆** a decimal.

*Espacio de trabajo:*
```
___ × 256  +  ___ × 16  +  ___ × 1
= _______   + _______   + _______
= ___________
```

---

#### Sección 3 — Conversión cruzada Binario ↔ Hexadecimal

**A7.** Convertir **11110000₂** a hexadecimal (usando grupos de 4).

*Espacio de trabajo:*
```
____  ____
 __    __

Resultado: ___________
```

**A8.** Convertir **B9₁₆** a binario (expandir cada dígito a 4 bits).

*Espacio de trabajo:*
```
B →  ____
9 →  ____

Resultado: ___________
```

---

#### Sección 4 — Interpretación de formato

**A9.** El código de color de un logotipo es **#4CAF50**. Descompón sus tres componentes RGB en decimal.

*Espacio de trabajo:*
```
Rojo:   4C₁₆ = ___ × 16 + ___ = ___
Verde:  AF₁₆ = ___ × 16 + ___ = ___
Azul:   50₁₆ = ___ × 16 + ___ = ___
```

¿De qué color aproximado es? ___________

**A10.** El siguiente volcado hexadecimal es un fragmento de texto. Decodifícalo:

```
43  6F  6C  6F  6D  62  69  61
```

| Hex | Decimal | Carácter |
|:---:|:---:|:---:|
| 43 | | |
| 6F | | |
| 6C | | |
| 6F | | |
| 6D | | |
| 62 | | |
| 69 | | |
| 61 | | |

**Texto:** ___________

---

### PARTE B — Verificación en Parejas (15 min)

> **Instrucciones:** Intercambia tu hoja con un compañero. Verifica sus respuestas usando el método de conversión inversa. Si encuentras un error, indícalo con una marca y explica cuál fue el paso incorrecto (no solo el resultado).

**Protocolo de verificación:**

Para verificar una conversión Decimal → Hex: convierte el resultado hex de vuelta a decimal.
Para verificar una conversión Hex → Decimal: convierte el resultado decimal de vuelta a hex.
Para verificar Bin ↔ Hex: aplica el método inverso de grupos de 4.

**Registro de verificación:**

| Ejercicio | Mi resultado | Resultado del compañero | ¿Coincide? | Observación |
|:---:|:---:|:---:|:---:|:---|
| A1 | | | | |
| A2 | | | | |
| A3 | | | | |
| A4 | | | | |
| A5 | | | | |
| A6 | | | | |
| A7 | | | | |
| A8 | | | | |
| A9 R/G/B | | | | |
| A10 texto | | | | |

---

### PARTE C — Desafío de Aplicación Real (15 min)

> **Instrucciones:** En grupos de 3. Cada desafío conecta las conversiones con una situación real. Uno del grupo resuelve, otro verifica, el tercero explica el resultado en palabras.

---

**Desafío 1 — El Paleta de Colores del Colegio**

Tu colegio quiere crear su página web y necesita definir los colores institucionales. El equipo de diseño dice que el color azul del escudo es RGB(0, 71, 171).

a) Convierte cada componente a hexadecimal para escribir el código de color web.
b) Escribe el código completo en formato `#RRGGBB`.
c) ¿Cómo se vería ese azul en binario (los tres bytes uno tras otro)?

*Respuesta esperada:*
```
R: 0   → 00₁₆  → 0000 0000₂
G: 71  → 47₁₆  → 0100 0111₂
B: 171 → AB₁₆  → 1010 1011₂

Código web: #0047AB
Binario completo: 00000000 01000111 10101011
```

---

**Desafío 2 — El Mensaje Secreto**

Un hackeador dejó este mensaje en el sistema de tu colegio. Decodifícalo:

```
53  69  73  74  65  6D  61  73  20  4E  75  6D  E9  72  69  63  6F  73
```

> Nota: El byte `E9` corresponde al carácter 'é' (e con acento agudo) en la codificación Latin-1.

*Ayuda:* Los primeros 8 bytes son: S-i-s-t-e-m-a-s

**Mensaje completo:** ___________

*Respuesta:* `Sistemas Numéricos`

---

**Desafío 3 — El Error del Sistema**

Una computadora muestra el código de error `0xC0FFEE` en pantalla.

a) ¿Cuánto vale en decimal?
b) ¿Cuántos bytes ocupa?
c) Escríbelo en binario completo (sin omitir ceros).
d) ¿Es un número que puede almacenarse en 2 bytes (16 bits)? ¿Por qué?

*Respuesta esperada:*
```
a) C0FFEE₁₆ = 12×65536 + 0×4096 + 15×256 + 15×16 + 14×1
            = 786432 + 0 + 3840 + 240 + 14
            = 12648430₁₀

b) Ocupa 3 bytes (6 dígitos hex = 3 bytes de 8 bits)

c) 1100 0000  1111 1111  1110 1110

d) No, porque su valor (12648430) supera el máximo
   de 2 bytes (65535). Necesita al menos 3 bytes.
```

---

### Respuestas Oficiales del Taller — Parte A

> **Solo para el docente. No mostrar hasta que todos terminen.**

| Ejercicio | Respuesta correcta | Proceso clave a monitorear |
|:---:|:---:|:---|
| A1 | 2D₁₆ | 45÷16=2 R13(D), 2÷16=0 R2 |
| A2 | AD₁₆ | 173÷16=10 R13(D), 10÷16=0 R10(A) |
| A3 | 3E8₁₆ | 1000÷16=62 R8, 62÷16=3 R14(E), 3÷16=0 R3 |
| A4 | 122₁₀ | 7×16 + 10×1 = 112+10 |
| A5 | 700₁₀ | 2×256 + 11×16 + 12 = 512+176+12 |
| A6 | 3855₁₀ | 15×256 + 0×16 + 15 = 3840+0+15 |
| A7 | F0₁₆ | 1111→F, 0000→0 |
| A8 | 10111001₂ | B→1011, 9→1001 |
| A9 | R:76, G:175, B:80 (verde oliva/esmeralda) | 4C=76, AF=175, 50=80 |
| A10 | Colombia | 43=C,6F=o,6C=l,6F=o,6D=m,62=b,69=i,61=a |

---

# BLOQUE 9 — Socialización y Corrección (15 min)

> **Para el docente:** Selecciona 4–5 ejercicios representativos del taller para resolver en el tablero. Prioriza los que generaron más dudas durante el monitoreo. Invita a un estudiante diferente a resolver cada ejercicio, y pide al resto que señale el error o confirme el proceso.

**Preguntas clave para la discusión post-taller:**

1. ¿Qué diferencia hay entre cometer un error en el residuo y cometer un error en la conversión del residuo a letra hex?
2. ¿Por qué conviene siempre verificar convirtiendo en sentido inverso?
3. En el desafío del color (#0047AB), ¿qué pasaría si el verde fuera 74 en lugar de 47? ¿Sería un color muy diferente?
4. ¿Por qué creen que los programadores usan `0x` antes de los números hex en el código?

---

# BLOQUE 10 — Resumen y Cierre (10 min)

## 12. Resumen y Cierre

### Mapa de lo aprendido hoy

```
SISTEMA DECIMAL          SISTEMA HEXADECIMAL
Base: 10                 Base: 16
Dígitos: 0–9             Dígitos: 0–9, A–F
Uso: vida cotidiana      Uso: colores, memoria, errores

Conversión Dec→Hex:      Conversión Hex→Dec:
Dividir entre 16         Multiplicar por potencias de 16
Leer residuos ↑          y sumar
(convertir 10+ a letra)

TRUCO BINARIO ↔ HEX      APLICACIONES REALES
Grupos de 4 bits         Colores: #RRGGBB
1 dígito hex = 4 bits    Texto: ASCII en hex
= 1 nibble               Memoria: 0xDIRECCIÓN
                         Errores: 0xCÓDIGO
```

---

### Las 5 Reglas de Oro para Recordar

1. **Regla de los 16 símbolos:** El hex tiene 16 dígitos — los diez normales (0–9) y seis letras (A=10, B=11, C=12, D=13, E=14, F=15).

2. **Regla de las divisiones:** Para decimal → hex, divide repetidamente entre 16. Los residuos de 10 a 15 se escriben como A, B, C, D, E, F. Se leen de abajo hacia arriba.

3. **Regla de las potencias:** Para hex → decimal, multiplica cada dígito hex por 16 elevado a su posición (derecha a izquierda desde 0) y suma.

4. **Regla de los 4 bits:** Para binario ↔ hex, agrupa de 4 en 4 desde la derecha. 1 dígito hex = 4 bits exactos. Nunca más, nunca menos.

5. **Regla de la verificación:** Siempre comprueba convirtiendo en sentido contrario. Si `AB₁₆ = 171₁₀`, entonces `171₁₀` debe dar `AB₁₆` al convertirlo de regreso.

---

### Comparación final de todos los sistemas

| Sistema | Base | Dígitos | Bits por dígito | Ejemplo (255) |
|:---:|:---:|:---:|:---:|:---:|
| Binario | 2 | 0, 1 | 1 | 11111111 |
| Octal | 8 | 0–7 | 3 | 377 |
| Decimal | 10 | 0–9 | ~3.32 | 255 |
| Hexadecimal | 16 | 0–F | 4 | FF |

> El hexadecimal gana en compacidad para representar datos binarios: 2 dígitos hex = 1 byte exacto. Por eso domina la programación de sistemas.

---

### Conexión con la próxima clase

| Tema | Concepto relacionado |
|:---|:---|
| Representación de enteros negativos | Complemento a 2 en binario y hex |
| Redes de computadoras | Direcciones IPv4 e IPv6 en hex |
| Criptografía básica | Hashes MD5/SHA en hexadecimal |
| Programación en C/Python | Operaciones bit a bit con hex |

---

### Autoevaluación del Estudiante

Responde marcando con una X tu nivel de comprensión:

| Habilidad | No lo domino | En proceso | Lo domino |
|:---|:---:|:---:|:---:|
| Identificar los 16 dígitos hexadecimales (incluidas letras) | | | |
| Convertir de decimal a hexadecimal usando divisiones | | | |
| Convertir de hexadecimal a decimal usando potencias | | | |
| Convertir entre binario y hex usando grupos de 4 | | | |
| Interpretar un código de color RGB en hexadecimal | | | |
| Decodificar texto en formato ASCII hexadecimal | | | |
| Verificar una conversión usando el método inverso | | | |

---

### Tarea para la Próxima Sesión

> Opcional — a criterio del docente.

1. Busca el código hexadecimal de los colores de la bandera de tu país. Conviértelos a RGB decimal.
2. Encuentra en tu computador o celular una configuración avanzada que muestre valores en hexadecimal (puede ser en ajustes de color, información de red, o consola del navegador).
3. Desafío: el color `#7F7F7F` — ¿qué nombre le darías? ¿Por qué todos sus componentes son iguales?
4. Investiga: ¿Qué es el sistema hexadecimal de 32 bits y para qué se usa en las direcciones IPv6?

---

## Glosario

| Término | Definición |
|:---|:---|
| **Hexadecimal** | Sistema numérico de base 16. Usa los dígitos 0–9 y las letras A–F. |
| **Nibble** | Grupo de 4 bits. Equivale exactamente a un dígito hexadecimal. |
| **Byte** | Grupo de 8 bits. Equivale exactamente a 2 dígitos hexadecimales. |
| **ASCII** | Estándar que asigna un número a cada carácter del teclado. |
| **RGB** | Modelo de color basado en tres componentes: Rojo, Verde y Azul, cada uno de 0 a 255. |
| **Volcado de memoria** | Representación de la memoria RAM en formato hexadecimal, byte por byte. |
| **Prefijo 0x** | Notación usada en programación para indicar que un número está en hexadecimal. |
| **Stop Code** | Código de error del sistema operativo, típicamente representado en hexadecimal. |
| **Complemento** | Operación matemática que permite representar números negativos en binario y hexadecimal. |
| **Hash** | Valor hexadecimal generado por una función matemática a partir de datos. Se usa en seguridad. |
| **Dirección MAC** | Identificador único de una tarjeta de red, expresado en 6 bytes hexadecimales. |
| **Conversión cruzada** | Proceso de convertir un valor entre dos o más sistemas numéricos para verificar su equivalencia. |

---

## Referencias y Recursos Adicionales

- **Herramienta online de colores:** [coolors.co](https://coolors.co) — permite ver códigos hex y RGB de millones de colores.
- **Conversor numérico:** [rapidtables.com/convert/number](https://www.rapidtables.com/convert/number/) — convierte entre todos los sistemas en tiempo real.
- **Tabla ASCII completa:** [asciitable.com](https://www.asciitable.com) — todos los caracteres con su valor decimal, hex y binario.
- **Editor hexadecimal online:** [hexed.it](https://hexed.it) — permite abrir archivos y ver su contenido en hexadecimal.
- **Actividad complementaria:** buscar en YouTube "How computers use hexadecimal — Computerphile" para una explicación audiovisual excelente.
- **Libro de referencia:** Mano, M. M. (2003). *Diseño Digital*. Pearson. Capítulos 1 y 2.

---

*Material educativo de libre uso — Sistemas Digitales · Módulo 2: Decimal y Hexadecimal · Nivel secundaria (15–16 años) · Publicable en GitHub Pages.*
