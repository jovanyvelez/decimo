# 🖥️ Representación de Datos en la Computadora

> **Nivel:** Educación Media — 15 a 16 años  
> **Duración total:** 4 horas de clase + 2 descansos de 15 min  
> **Modalidad:** Teórico-práctica con talleres y retos

---

## 📋 Tabla de Contenido

1. [¿Cómo piensa una computadora?](#1-cómo-piensa-una-computadora)
2. [El Bit: la unidad mínima de información](#2-el-bit-la-unidad-mínima-de-información)
3. [Bytes y Palabras: agrupando bits](#3-bytes-y-palabras-agrupando-bits)
4. [Sistema Binario: contando con 0s y 1s](#4-sistema-binario-contando-con-0s-y-1s)
5. [Representación Sin Signo](#5-representación-sin-signo)
6. [🔴 DESCANSO 1 — 15 minutos](#-descanso-1--15-minutos)
7. [Representación Con Signo](#6-representación-con-signo)
8. [Desbordamiento: cuando los números se salen de control](#7-desbordamiento-cuando-los-números-se-salen-de-control)
9. [Codificación de Caracteres: del número a la letra](#8-codificación-de-caracteres-del-número-a-la-letra)
10. [🔴 DESCANSO 2 — 15 minutos](#-descanso-2--15-minutos)
11. [¿Cómo impacta esto la lógica de los programas?](#9-cómo-impacta-esto-la-lógica-de-los-programas)
12. [🧪 Taller Evaluativo](#-taller-evaluativo-de-codificación-simple-de-caracteres)
13. [Glosario](#glosario)

---

## Cronograma de la Sesión

| Bloque | Actividad | Duración |
|--------|-----------|----------|
| 🟢 Bloque 1 | Secciones 1–5: Bits, Bytes, Palabras y Representación Sin Signo | 120 min |
| 🔴 Descanso 1 | Pausa activa | 15 min |
| 🟡 Bloque 2 | Secciones 6–9: Con Signo, Desbordamiento, Caracteres e Impacto | 75 min |
| 🔴 Descanso 2 | Pausa activa | 15 min |
| 🔵 Bloque 3 | Taller Evaluativo | 45 min |

---

# 🟢 BLOQUE 1 — 120 minutos

---

## 1. ¿Cómo piensa una computadora?

Imagina que le preguntas a tu amigo: "¿Hay luz en el cuarto?". Tu amigo solo puede responderte **sí** o **no**. Eso es básicamente cómo piensa una computadora: con solo dos respuestas posibles.

Internamente, una computadora es un circuito electrónico enorme lleno de diminutos interruptores llamados **transistores**. Cada interruptor solo puede estar en uno de dos estados:

- **Encendido** → representamos esto como `1`
- **Apagado** → representamos esto como `0`

Todo lo que hace una computadora —reproducir música, mostrar fotos, ejecutar un videojuego, enviar un mensaje— ocurre porque millones de estos interruptores se encienden y apagan a velocidades increíbles.

> 💡 **Dato curioso:** Un procesador moderno puede contener más de **50 mil millones de transistores** en un chip del tamaño de una uña.

### ¿Por qué solo dos estados y no más?

Podríamos diseñar computadoras que usen 10 estados (como nuestros dedos), pero usar solo dos estados tiene ventajas enormes:

- **Confiabilidad:** Es muy fácil distinguir "hay corriente" de "no hay corriente". Cualquier valor intermedio se interpreta sin ambigüedad.
- **Ruido:** En la electrónica real, siempre hay pequeñas variaciones de voltaje. Con dos estados, pequeñas fluctuaciones no causan errores.
- **Simplicidad:** Las matemáticas con solo `0` y `1` son muy elegantes y poderosas (Álgebra de Boole).

---

## 2. El Bit: la unidad mínima de información

Un **bit** (del inglés *binary digit*, dígito binario) es la unidad más pequeña de información que existe en una computadora.

Un solo bit solo puede representar **dos posibilidades**:

```
bit = 0   →  apagado, falso, no, vacío
bit = 1   →  encendido, verdadero, sí, lleno
```

### ¿Cuánto podemos representar con bits?

Con un solo bit: **2 posibilidades** (`0` o `1`)  
Con 2 bits: **4 posibilidades** (`00`, `01`, `10`, `11`)  
Con 3 bits: **8 posibilidades**  
Con `n` bits: **2ⁿ posibilidades**

| Bits (n) | Posibilidades (2ⁿ) | Ejemplo de uso |
|----------|-------------------|----------------|
| 1 | 2 | Verdadero/Falso |
| 2 | 4 | 4 colores |
| 4 | 16 | Un dígito hexadecimal |
| 8 | 256 | Un carácter ASCII básico |
| 16 | 65,536 | Sonido de 16 bits (CD) |
| 24 | 16,777,216 | Colores en una pantalla |
| 32 | 4,294,967,296 | Enteros de 32 bits |
| 64 | ~1.8 × 10¹⁹ | Enteros de 64 bits |

### ✏️ Actividad rápida 1

> ¿Cuántos bits necesitas para representar los 7 días de la semana sin que ningún día quede sin representación? Justifica tu respuesta.

<details>
<summary>💡 Pista (haz clic para ver)</summary>

Recuerda: necesitas encontrar el menor `n` tal que `2ⁿ ≥ 7`.  
Prueba con n=2: 2²=4 (insuficiente). Con n=3: 2³=8 (¡suficiente!).

</details>

---

## 3. Bytes y Palabras: agrupando bits

Un solo bit nos da muy poca información. Por eso los bits se agrupan.

### El Byte

La agrupación más común es el **byte**: un grupo de **8 bits**.

```
Un byte: [  1  |  0  |  1  |  1  |  0  |  0  |  1  |  0  ]
           bit7  bit6  bit5  bit4  bit3  bit2  bit1  bit0
```

Con 8 bits podemos representar **2⁸ = 256** valores diferentes (del 0 al 255).

> 💡 **¿Por qué 8?** Históricamente, 8 bits resultó ser un buen balance entre eficiencia y capacidad. Los primeros microprocesadores trabajaban con 8 bits, y la convención quedó establecida.

### Múltiplos del byte

Las computadoras modernas manejan cantidades enormes de información. Por eso usamos prefijos:

| Unidad | Símbolo | Equivalencia aproximada |
|--------|---------|------------------------|
| Kilobyte | KB | 1,024 bytes ≈ 10³ bytes |
| Megabyte | MB | 1,024 KB ≈ 10⁶ bytes |
| Gigabyte | GB | 1,024 MB ≈ 10⁹ bytes |
| Terabyte | TB | 1,024 GB ≈ 10¹² bytes |
| Petabyte | PB | 1,024 TB ≈ 10¹⁵ bytes |

> 🎮 **Contexto real:** Un videojuego moderno de alta calidad puede ocupar entre 50 y 100 GB. Un emoji en WhatsApp ocupa unos pocos bytes. Un minuto de video en HD ocupa aproximadamente 100 MB.

### La Palabra (Word)

En arquitectura de computadoras, una **palabra** (*word*) es el tamaño natural de datos que el procesador puede manejar en una sola operación. Su tamaño depende de la arquitectura:

| Arquitectura | Tamaño de palabra | Bits |
|--------------|-------------------|------|
| 8 bits (retro) | 1 byte | 8 bits |
| 16 bits (ej: Intel 8086) | 2 bytes | 16 bits |
| 32 bits (ej: Pentium) | 4 bytes | 32 bits |
| 64 bits (computadoras actuales) | 8 bytes | 64 bits |

Piensa en la "palabra" como el tamaño del "cucharón" con el que el procesador toma información: un cucharón más grande permite trabajar con números más grandes y mover más datos de una vez.

### ✏️ Actividad rápida 2

> Una canción en formato MP3 tiene 4.5 MB. Si quisieras almacenar 100 canciones similares, ¿cuántos GB necesitarías aproximadamente? Muestra tus cálculos.

---

## 4. Sistema Binario: contando con 0s y 1s

Para entender cómo los bits representan números, necesitamos entender el **sistema binario** (base 2).

### Primero, recordemos el sistema decimal (base 10)

Cuando escribimos el número `3,742`, cada posición tiene un valor:

```
  3  ,  7  ,  4  ,  2
  ↑     ↑     ↑     ↑
 10³   10²   10¹   10⁰
1000   100    10     1

3×1000 + 7×100 + 4×10 + 2×1 = 3,742
```

Usamos base 10 porque tenemos 10 dígitos: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9`.

### Ahora, el sistema binario (base 2)

En binario solo hay 2 dígitos: `0` y `1`. Cada posición tiene un valor que es una potencia de 2:

```
  1  |  0  |  1  |  1  |  0  |  1  |  0  |  0
  ↑     ↑     ↑     ↑     ↑     ↑     ↑     ↑
 2⁷   2⁶   2⁵   2⁴   2³   2²   2¹   2⁰
 128   64    32    16    8     4     2     1
```

Para convertir `10110100₂` a decimal:

```
1×128 + 0×64 + 1×32 + 1×16 + 0×8 + 1×4 + 0×2 + 0×1
= 128 + 0 + 32 + 16 + 0 + 4 + 0 + 0
= 180
```

### Tabla de los primeros 16 números

| Decimal | Binario (4 bits) | Hexadecimal |
|---------|-----------------|-------------|
| 0 | 0000 | 0 |
| 1 | 0001 | 1 |
| 2 | 0010 | 2 |
| 3 | 0011 | 3 |
| 4 | 0100 | 4 |
| 5 | 0101 | 5 |
| 6 | 0110 | 6 |
| 7 | 0111 | 7 |
| 8 | 1000 | 8 |
| 9 | 1001 | 9 |
| 10 | 1010 | A |
| 11 | 1011 | B |
| 12 | 1100 | C |
| 13 | 1101 | D |
| 14 | 1110 | E |
| 15 | 1111 | F |

### El Sistema Hexadecimal: un atajo útil

Como los números binarios se vuelven muy largos, los programadores frecuentemente usan la **base 16 (hexadecimal)**. Cada dígito hexadecimal equivale exactamente a **4 bits**:

```
Binario:      1011  0100
              ↓       ↓
Hexadecimal:   B       4
→ 0xB4  (en programación, el prefijo 0x indica hexadecimal)
```

> 🎨 **Ejemplo real:** Los colores en pantalla se expresan en hexadecimal.  
> El rojo puro es `#FF0000` → R=255 (FF), G=0 (00), B=0 (00)  
> El blanco es `#FFFFFF`, el negro es `#000000`.

### Convirtiendo decimal a binario

El método más sencillo es la **división sucesiva por 2**:

**Ejemplo:** Convertir `45` a binario.

```
45 ÷ 2 = 22, residuo 1   ← bit menos significativo
22 ÷ 2 = 11, residuo 0
11 ÷ 2 =  5, residuo 1
 5 ÷ 2 =  2, residuo 1
 2 ÷ 2 =  1, residuo 0
 1 ÷ 2 =  0, residuo 1   ← bit más significativo

Leyendo los residuos de abajo hacia arriba: 101101₂
```

Verificación: `1×32 + 0×16 + 1×8 + 1×4 + 0×2 + 1×1 = 32+8+4+1 = 45` ✔️

### ✏️ Actividad práctica 3 — Conversiones

Convierte los siguientes números (muestra el proceso):

| # | Número | De | A |
|---|--------|-----|---|
| a | `42` | Decimal | Binario |
| b | `11001010₂` | Binario | Decimal |
| c | `255` | Decimal | Binario y Hexadecimal |
| d | `0x1A` | Hexadecimal | Decimal y Binario |

---

## 5. Representación Sin Signo

Cuando usamos todos los bits para representar **solo números positivos** (incluyendo el cero), decimos que estamos usando **representación sin signo** (*unsigned*).

### Rango de valores

Con `n` bits sin signo podemos representar números desde `0` hasta `2ⁿ - 1`:

| Bits | Mínimo | Máximo | Tipo en C/C++ |
|------|--------|--------|---------------|
| 8 | 0 | 255 | `uint8_t` |
| 16 | 0 | 65,535 | `uint16_t` |
| 32 | 0 | 4,294,967,295 | `uint32_t` |
| 64 | 0 | 18,446,744,073,709,551,615 | `uint64_t` |

### ¿Cuándo se usa?

La representación sin signo es ideal cuando sabemos que el valor **nunca será negativo**:

- Tamaño de un archivo (no puede ser negativo)
- Edad de una persona (en la mayoría de contextos)
- Contadores de bucles positivos
- Direcciones de memoria
- Valores de colores RGB (0–255)
- Números de puerto de red (0–65535)

### Suma en binario sin signo

Las reglas son iguales que en decimal, pero solo con 0 y 1:

```
  0 + 0 = 0
  0 + 1 = 1
  1 + 0 = 1
  1 + 1 = 10  (es decir, 0 con acarreo de 1)
```

**Ejemplo:** `0b00110101` (53) + `0b00011010` (26) = `0b01001111` (79)

```
   0 0 1 1 0 1 0 1   = 53
+  0 0 0 1 1 0 1 0   = 26
─────────────────
   0 1 0 0 1 1 1 1   = 79
```

### ✏️ Actividad práctica 4

Realiza las siguientes sumas en binario (8 bits sin signo). Luego verifica el resultado convirtiendo a decimal:

```
a)  00101010 + 00010101 = ?
b)  01100000 + 00011111 = ?
c)  11110000 + 00001111 = ?
```

> ¿Qué pasaría si intentaras sumar `11111111 + 00000001` en 8 bits? ¿Qué resultado obtienes y qué problema observas?

---

# 🔴 DESCANSO 1 — 15 minutos

> 🧘 **Pausa activa sugerida:**
> - Estira los brazos y el cuello.
> - Cierra los ojos 1 minuto y respira profundo.
> - Camina un poco y toma agua.
> - Reto mental: intenta "leer" el número `0b10101010` de camino al baño 😄

---

# 🟡 BLOQUE 2 — 75 minutos

---

## 6. Representación Con Signo

En la vida real los números negativos existen. Las temperaturas bajo cero, las deudas, los errores de posición... ¿Cómo representamos el signo negativo cuando solo tenemos `0` y `1`?

### Intento 1: Bit de signo (Magnitud y Signo)

La idea más intuitiva: usar el **bit más significativo (MSB)** para indicar el signo.

```
0 → positivo
1 → negativo
```

Con 8 bits: `0 1001100` = +76 y `1 1001100` = -76

**Problema:** Este enfoque tiene dos representaciones del cero: `00000000` (+0) y `10000000` (-0). Eso complica los circuitos de suma.

### La solución moderna: Complemento a Dos (Two's Complement)

El método estándar en todos los procesadores modernos es el **complemento a dos**. Parece extraño al principio, pero es brillante.

#### Cómo obtener el complemento a dos de un número negativo:

1. Escribe el número positivo en binario.
2. **Invierte todos los bits** (cambia 0 por 1 y viceversa). A esto se le llama complemento a uno.
3. **Suma 1** al resultado.

**Ejemplo:** ¿Cómo representamos `-45` en 8 bits?

```
Paso 1: Positivo  →   00101101  (45 en binario)
Paso 2: Invertir  →   11010010  (complemento a uno)
Paso 3: Sumar 1   →   11010011  (complemento a dos = -45)
```

Entonces `-45` se representa como `11010011`.

#### Verificación: ¿Cómo saber si es negativo?

Si el **bit más significativo (el de la izquierda) es 1**, el número es negativo.

#### Rango con complemento a dos

| Bits | Mínimo | Máximo | Tipo en C/C++ |
|------|--------|--------|---------------|
| 8 | -128 | +127 | `int8_t` |
| 16 | -32,768 | +32,767 | `int16_t` |
| 32 | -2,147,483,648 | +2,147,483,647 | `int32_t` |
| 64 | -9,223,372,036,854,775,808 | +9,223,372,036,854,775,807 | `int64_t` |

> 🤔 **¿Por qué no es simétrico?** Hay un número negativo más que positivos. Por ejemplo, en 8 bits hay -128 pero no +128. Esto se debe a que el cero ocupa uno de los valores positivos.

#### La magia del complemento a dos: la suma funciona igual

La gran ventaja es que podemos sumar números positivos y negativos con **el mismo circuito**:

```
  45 en 8 bits:  00101101
+ (-45) en 8 bits: 11010011
─────────────────────────────
                 100000000  ← el 1 del bit 8 "se cae" (desbordamiento)
                  00000000  = 0 ✔️
```

### Cómo convertir un número negativo en complemento a dos a decimal

**Ejemplo:** Dado `11010011`, ¿qué número decimal es?

Como el MSB es `1`, sabemos que es negativo. Para encontrar su valor:

1. Invertir todos los bits: `00101100`
2. Sumar 1: `00101101`
3. Convertir a decimal: `32+8+4+1 = 45`
4. Agregar el signo: **-45**

### ✏️ Actividad práctica 5 — Con signo

| # | Enunciado | Respuesta |
|---|-----------|-----------|
| a | Representa `-35` en binario de 8 bits (complemento a dos) | ? |
| b | ¿Qué número decimal es `11111111` en complemento a dos de 8 bits? | ? |
| c | ¿Qué número decimal es `10000000` en complemento a dos de 8 bits? | ? |
| d | Suma `(-30) + 20` usando complemento a dos de 8 bits | ? |

---

## 7. Desbordamiento: cuando los números se salen de control

El **desbordamiento** (*overflow*) ocurre cuando el resultado de una operación es más grande (o más pequeño) de lo que puede almacenar la variable.

### Ejemplo clásico

En una variable de 8 bits sin signo, el máximo es 255. ¿Qué pasa si sumamos 1?

```
  11111111  (255)
+ 00000001  (1)
──────────
 100000000  → El 1 se pierde, queda 00000000 = 0
```

**¡255 + 1 = 0!** Esto no es un error matemático, es una consecuencia de la representación finita.

### Desbordamiento con signo

Con 8 bits con signo, el máximo es 127:

```
  01111111  (127)
+ 00000001  (1)
──────────
  10000000  = -128 en complemento a dos
```

**¡127 + 1 = -128!** Esto es un bug clásico en programación.

### Casos reales famosos de overflow

- **El año 2000 (Y2K):** Los programas guardaban el año con solo 2 dígitos. `99 + 1 = 00` causó pánico mundial.
- **Ariane 5 (1996):** Un cohete espacial europeo explotó segundos después del lanzamiento. La causa: un número de 64 bits se intentó guardar en una variable de 16 bits.
- **Juego GTA San Andreas:** Al llegar a cierto nivel de "quería", un valor llegaba a 32,767 y al sumar 1 se convertía en -32,768, haciendo que la policía "olvidara" al jugador.

> ⚠️ **Lección para programadores:** Siempre considera el rango de tus variables. Un overflow silencioso puede causar desde un bug gracioso hasta un desastre catastrófico.

### ✏️ Reflexión rápida

> En un sistema de votaciones, ¿qué tipo de dato usarías para guardar el número de votos de una elección presidencial en un país de 50 millones de habitantes? ¿Por qué?

---

## 8. Codificación de Caracteres: del número a la letra

Ya sabemos que la computadora solo entiende números. Entonces, ¿cómo almacena texto?

La respuesta: **asignando un número a cada carácter**. Esta tabla de correspondencias se llama **codificación de caracteres** (*character encoding*).

### ASCII: el principio de todo

En 1963, el **Código Estándar Americano para el Intercambio de Información** (ASCII, por sus siglas en inglés) estableció una tabla de 128 caracteres usando 7 bits (después extendido a 8 bits).

#### Tabla ASCII básica (selección)

| Decimal | Hexadecimal | Binario | Carácter | Descripción |
|---------|-------------|---------|----------|-------------|
| 0 | 0x00 | 00000000 | NUL | Carácter nulo |
| 9 | 0x09 | 00001001 | TAB | Tabulación |
| 10 | 0x0A | 00001010 | LF | Nueva línea |
| 13 | 0x0D | 00001101 | CR | Retorno de carro |
| 32 | 0x20 | 00100000 | (espacio) | Espacio |
| 48 | 0x30 | 00110000 | `0` | Dígito cero |
| 49 | 0x31 | 00110001 | `1` | Dígito uno |
| 57 | 0x39 | 00111001 | `9` | Dígito nueve |
| 65 | 0x41 | 01000001 | `A` | Mayúscula A |
| 66 | 0x42 | 01000010 | `B` | Mayúscula B |
| 90 | 0x5A | 01011010 | `Z` | Mayúscula Z |
| 97 | 0x61 | 01100001 | `a` | Minúscula a |
| 98 | 0x62 | 01100010 | `b` | Minúscula b |
| 122 | 0x7A | 01111010 | `z` | Minúscula z |

#### Patrones útiles de ASCII

> **Truco 1:** Las letras mayúsculas van del 65 (`A`) al 90 (`Z`).  
> **Truco 2:** Las letras minúsculas van del 97 (`a`) al 122 (`z`).  
> **Truco 3:** La diferencia entre una mayúscula y su minúscula es siempre **32**.  
> Ej: `A` = 65, `a` = 97. `97 - 65 = 32`.  
> En binario: `A` = `01000001`, `a` = `01100001`. ¡Solo cambia el bit 5!

> **Truco 4:** Los dígitos van del 48 (`'0'`) al 57 (`'9'`).  
> Para convertir el carácter `'5'` al número `5`, basta restar 48:  
> `'5'` = 53, `53 - 48 = 5`.

### El problema de ASCII: ¿y el resto del mundo?

ASCII fue diseñado para el inglés. Solo tiene 128 caracteres (26 letras × 2 casos + números + puntuación + caracteres de control). No incluye:

- Tildes: á, é, í, ó, ú (español)
- Eñe: ñ (español)
- Caracteres chinos, árabes, hindi, japonés...
- Emojis 😅

### ISO-8859-1 (Latin-1): una solución parcial

En los años 80, se extendió ASCII a 8 bits completos (256 valores). Los primeros 128 son iguales a ASCII, y los siguientes 128 incluyen caracteres europeos como `á`, `é`, `ñ`, `ü`, etc.

El problema: distintos países crearon sus propias extensiones de 256 caracteres. Un texto escrito en una computadora de Europa Occidental podía verse como caracteres extraños en una computadora de Europa del Este.

### Unicode y UTF-8: la solución global

**Unicode** es un estándar que asigna un número único (llamado *code point*) a **cada carácter de cada idioma del mundo**, incluyendo emojis. Actualmente define más de **149,000 caracteres**.

**UTF-8** es la forma más popular de almacenar Unicode. Es inteligente: usa **entre 1 y 4 bytes por carácter**:
- Los caracteres ASCII originales usan 1 byte (¡compatible hacia atrás!)
- Letras europeas con acentos usan 2 bytes
- Caracteres asiáticos usan 3 bytes
- Emojis y caracteres especiales usan 4 bytes

| Carácter | Unicode | UTF-8 (bytes) | Bytes en hex |
|----------|---------|---------------|--------------|
| `A` | U+0041 | 1 byte | `41` |
| `ñ` | U+00F1 | 2 bytes | `C3 B1` |
| `€` | U+20AC | 3 bytes | `E2 82 AC` |
| `😀` | U+1F600 | 4 bytes | `F0 9F 98 80` |

> 🌍 **Dato:** Hoy en día, más del 98% de las páginas web usan UTF-8 como codificación.

### ✏️ Actividad práctica 6 — Codificación ASCII

Usando la tabla ASCII:

**a)** Decodifica el siguiente mensaje (decimal a texto):

```
72  101  108  108  111  44  32  77  117  110  100  111  33
```

**b)** Codifica tu nombre completo en ASCII decimal.

**c)** ¿Qué cadena de texto forman estos bytes en hexadecimal?

```
0x48 0x6F 0x6C 0x61
```

**d)** Si `'A'` es 65, ¿cómo calcularías el código ASCII de `'M'` sin consultar la tabla?

---

# 🔴 DESCANSO 2 — 15 minutos

> 🧘 **Pausa activa sugerida:**
> - Estira los dedos y mueve las muñecas (¡van a programar pronto!).
> - Menciona en tu mente 3 cosas que aprendiste hoy.
> - Reto: ¿Qué dice `72 111 108 97`? (respuesta en ASCII) 😄

---

# 🔵 BLOQUE 3 — 45 minutos

---

## 9. ¿Cómo impacta esto la lógica de los programas?

Todo lo que hemos aprendido no es solo teoría. La representación de datos tiene consecuencias directas en cómo escribimos y depuramos código.

### 9.1 El tipo de dato importa

Cuando declaras una variable en cualquier lenguaje de programación, estás reservando un espacio en memoria con un número específico de bits. Usar el tipo equivocado puede causar problemas.

```python
# Python (maneja enteros de forma flexible, pero...)
edad = -5          # Python no se queja, pero una edad negativa no tiene sentido
votos = 4300000000 # En C/C++ con int de 32 bits esto causaría overflow

# En C/C++ el tipo define el límite:
# int8_t  edad = -5;      // OK, rango: -128 a 127
# uint8_t votos = 300;    // OK para votos pequeños
# uint32_t votos = 4300000000; // ERROR: máximo es 4,294,967,295
```

### 9.2 Comparar caracteres vs. comparar números

```python
# En Python
print('A' < 'B')    # True (porque 65 < 66)
print('Z' < 'a')    # True (porque 90 < 97, ¡mayúsculas van primero!)
print('9' < 'A')    # True (porque 57 < 65)

# Esto explica por qué al ordenar ["Zapato", "árbol", "Canasta"]
# "árbol" podría quedar al FINAL si se usa ordenamiento ASCII puro
# porque 'á' (225) > 'Z' (90) > 'C' (67)
```

### 9.3 El encoding puede romper tu programa

```python
# Si tu archivo tiene codificación Latin-1 pero lo lees como UTF-8:
with open("texto.txt", encoding="utf-8") as f:
    contenido = f.read()
# UnicodeDecodeError: 'utf-8' codec can't decode byte 0xf1 in position 3

# 0xF1 es 'ñ' en Latin-1, pero no es un byte válido en UTF-8
```

> 🔥 **Bug clásico:** ¿Alguna vez viste texto como `â€™` o `Ã±` en una página web? Eso es un error de encoding: el texto fue guardado en un formato (ej: UTF-8) y leído con otro (ej: Latin-1).

### 9.4 División entera vs. división real

```python
# En muchos lenguajes, dividir dos enteros da un entero
# Python 3:
print(7 / 2)   # 3.5  (división real)
print(7 // 2)  # 3    (división entera, descarta decimales)

# En C/C++:
# int resultado = 7 / 2;  →  resultado = 3 (¡no 3.5!)
```

Esta diferencia viene de que los enteros y los números de punto flotante se almacenan con esquemas de bits completamente distintos.

### 9.5 El operador módulo y los ciclos

```python
# El operador % (módulo) devuelve el residuo de la división
# Es útil para "wraparound" (dar vuelta al inicio)

posicion = (posicion_actual + 1) % total_elementos
# Si total = 5 y posicion_actual = 4: (4+1) % 5 = 0
# ¡Vuelve automáticamente al inicio! Como un reloj de 5 horas.
```

### 9.6 Operaciones bit a bit (Bitwise)

Los programadores a veces manipulan bits directamente. Esto es útil para eficiencia, flags de configuración, y encriptación básica.

| Operación | Símbolo | Ejemplo | Resultado |
|-----------|---------|---------|-----------|
| AND | `&` | `0b1010 & 0b1100` | `0b1000` |
| OR | `\|` | `0b1010 \| 0b1100` | `0b1110` |
| XOR | `^` | `0b1010 ^ 0b1100` | `0b0110` |
| NOT | `~` | `~0b00001111` | `0b11110000` |
| Shift izq. | `<<` | `0b0001 << 3` | `0b1000` (=8) |
| Shift der. | `>>` | `0b1000 >> 2` | `0b0010` (=2) |

**¿Para qué sirve esto?**

```python
# Verificar si un número es par o impar (mirando el último bit)
numero = 42
if numero & 1 == 0:
    print("par")   # El último bit de un par siempre es 0

# Multiplicar por 2 con shift izquierdo (más rápido que *)
x = 5          # 00000101
x_doble = x << 1  # 00001010 = 10

# Convertir mayúscula a minúscula con OR
# 'A' = 01000001, 32 = 00100000
# 'A' | 32 = 01100001 = 'a' ✔️
```

---

## 🧪 Taller Evaluativo de Codificación Simple de Caracteres

> ⏱️ **Tiempo:** 45 minutos  
> 📝 **Material permitido:** Esta guía, calculadora básica  
> 🏆 **Puntaje:** 100 puntos

---

### 📌 Parte 1 — Bases y Conversiones (25 puntos)

**1.1** (5 pts) Convierte los siguientes números. Muestra el procedimiento completo:

| # | Número dado | Convertir a... |
|---|-------------|----------------|
| a | `47` decimal | binario de 8 bits |
| b | `11001101₂` | decimal |
| c | `200` decimal | hexadecimal |
| d | `0xFF` | decimal y binario de 8 bits |

**1.2** (5 pts) Un byte tiene el valor `0b10110111`.

- a) ¿Cuál es su valor en decimal sin signo?
- b) ¿Cuál es su valor en decimal **con signo** (complemento a dos)?
- c) ¿Qué carácter ASCII representa este valor (si es un carácter imprimible)?

**1.3** (5 pts) Realiza las siguientes sumas binarias de 8 bits sin signo y escribe el resultado en decimal:

```
a)  01010101 + 00101010 = ?
b)  11000000 + 01000000 = ?
```
Para el inciso b), ¿hay desbordamiento? ¿Por qué?

**1.4** (5 pts) Representa los siguientes números en complemento a dos con 8 bits:

```
a) -1
b) -64
c) -128
```

**1.5** (5 pts) Completa la tabla:

| Binario (8 bits) | Decimal sin signo | Decimal con signo |
|-----------------|-------------------|-------------------|
| `00000001` | ? | ? |
| `01111111` | ? | ? |
| `10000000` | ? | ? |
| `11111111` | ? | ? |
| `10000001` | ? | ? |

---

### 📌 Parte 2 — Codificación ASCII (35 puntos)

**2.1** (10 pts) Decodifica los siguientes mensajes ASCII (decimal → texto):

**Mensaje A:**
```
66  105  101  110  118  101  110  105  100  111  115
```

**Mensaje B:**
```
80  114  111  103  114  97  109  97  114  32  101  115  32  99  114  101  97  114
```

**2.2** (10 pts) Codifica los siguientes textos en ASCII decimal:

- a) Tu nombre (al menos 4 caracteres)
- b) La palabra: `Hola2025`
- c) La frase: `Si!` (incluye mayúscula, minúscula y signo)

**2.3** (5 pts) Responde razonando con base en la tabla ASCII:

- a) ¿El carácter `'z'` es mayor o menor que el carácter `'A'` en ASCII? ¿Por qué?
- b) ¿Qué valor ASCII tiene `'F'`? (Calcula sin mirar la tabla, usando el valor de `'A'`)
- c) ¿Cómo convertirías el carácter `'7'` al número entero 7 usando aritmética?

**2.4** (10 pts) **Cifrado César básico con ASCII**

El cifrado César desplaza cada letra del alfabeto un número fijo de posiciones. Por ejemplo, con desplazamiento 3: `A → D`, `B → E`, `Z → C`.

El truco: suma el desplazamiento al código ASCII y aplica módulo para dar la vuelta al alfabeto.

Para mayúsculas: `código_cifrado = ((código - 65 + desplazamiento) % 26) + 65`

- a) Cifra la palabra `HOLA` con desplazamiento 3. Muestra los códigos ASCII intermedios.
- b) Descifra el siguiente mensaje cifrado con desplazamiento 13:

```
86  82  74  86  78  73  66
```
*(Pista: descifrar es cifrar con desplazamiento `26 - 13 = 13` nuevamente)*

---

### 📌 Parte 3 — Análisis y Reflexión (25 puntos)

**3.1** (10 pts) **El bug del overflow**

Un programador está desarrollando un sistema de puntuación para un videojuego. Usa una variable de tipo `uint8_t` (8 bits sin signo) para guardar la puntuación. El máximo actual de puntos que un jugador puede lograr es 300.

- a) ¿Es `uint8_t` el tipo correcto? ¿Por qué?
- b) ¿Qué ocurriría si el jugador alcanza exactamente 256 puntos?
- c) Escribe en binario qué valor quedaría guardado si se llega a 300 puntos con ese tipo.
- d) ¿Qué tipo de dato recomendarías? Justifica con el rango.

**3.2** (10 pts) **Encoding y texto internacional**

Un estudiante en Colombia escribe un programa que guarda nombres en un archivo de texto con codificación **Latin-1**. Luego, su compañero en Japón intenta abrir el archivo con su programa que usa **UTF-8**.

- a) ¿Qué problema podrían encontrar con nombres como "Sofía Muñoz"?
- b) ¿Qué caracteres específicamente causarían el problema? ¿Por qué?
- c) ¿Cómo se podría prevenir este problema desde el diseño del sistema?

**3.3** (5 pts) **Pregunta de reflexión abierta**

En tus propias palabras (mínimo 5 líneas), reflexiona sobre la siguiente pregunta:

> _"Dado que todo en una computadora es en última instancia una secuencia de 0s y 1s, ¿cómo es posible que la misma secuencia de bits pueda ser interpretada como un número, una letra, un color o una instrucción de programa? ¿Qué determina la interpretación?"_

---

### 📌 Parte 4 — Reto Extra ⭐ (15 puntos adicionales)

> *Esta parte es opcional y vale puntos extra. Solo inténtala si terminaste las partes anteriores.*

**4.1** (5 pts) Diseña tu propio sistema de codificación de 4 bits para los emojis más usados en tu clase. Define qué 16 emojis incluirías y justifica tu elección.

**4.2** (5 pts) En Python (o pseudocódigo), escribe una función que reciba un texto en mayúsculas y lo cifre usando el Cifrado César con desplazamiento `k`. ¿Cómo modificarías la función para manejar también minúsculas?

**4.3** (5 pts) Investiga brevemente: ¿qué es el **BOM (Byte Order Mark)** en archivos de texto y por qué puede causar problemas en programas que procesan archivos UTF-8? Explica con tus palabras.

---

## Glosario

| Término | Definición |
|---------|------------|
| **Bit** | Unidad mínima de información; puede ser 0 o 1 |
| **Byte** | Grupo de 8 bits; puede representar 256 valores |
| **Palabra (Word)** | Tamaño natural de datos del procesador (16, 32 o 64 bits) |
| **Binario** | Sistema numérico en base 2 (solo 0 y 1) |
| **Hexadecimal** | Sistema numérico en base 16; usa dígitos 0-9 y letras A-F |
| **Sin signo (Unsigned)** | Representación que solo incluye números no negativos |
| **Con signo (Signed)** | Representación que incluye positivos, negativos y cero |
| **Complemento a dos** | Método estándar para representar negativos en binario |
| **Desbordamiento (Overflow)** | Error al exceder el rango máximo (o mínimo) de una variable |
| **ASCII** | Tabla de 128 caracteres estándar (1963), base de la codificación de texto |
| **Unicode** | Estándar global que asigna un código único a cada carácter del mundo |
| **UTF-8** | Codificación de longitud variable compatible con ASCII, estándar en la web |
| **MSB** | Bit más significativo; el de mayor peso (posición izquierda) |
| **LSB** | Bit menos significativo; el de menor peso (posición derecha) |
| **Encoding** | Esquema que mapea caracteres a secuencias de bytes |
| **Bitwise** | Operaciones que actúan sobre bits individuales de un número |
| **Transistor** | Interruptor microscópico; la unidad física que representa un bit |
| **Módulo (%)** | Operación que devuelve el residuo de una división entera |

---

## 📚 Referencias y Recursos para Profundizar

- [ASCII Table](https://www.asciitable.com/) — Tabla ASCII completa e interactiva
- [Unicode Explorer](https://unicode-explorer.com/) — Busca cualquier carácter Unicode
- [Ben Eater — How Computers Work](https://www.youtube.com/@BenEater) — Videos explicativos de electrónica y computación
- [CS50x (Harvard)](https://cs50.harvard.edu/x/) — Curso introductorio gratuito de informática (en inglés con subtítulos)
- [Computerphile](https://www.youtube.com/@Computerphile) — Canal de YouTube con conceptos de ciencias de la computación

---

## ✅ Rúbrica del Taller

| Criterio | Excelente (100%) | Bueno (75%) | Suficiente (50%) | Insuficiente (<50%) |
|----------|-----------------|-------------|-----------------|---------------------|
| **Conversiones numéricas** | Procedimiento correcto y resultado exacto | Procedimiento correcto, pequeño error de cálculo | Procedimiento parcial | Sin procedimiento o resultado incorrecto |
| **Codificación ASCII** | Todos los caracteres correctos | 1–2 errores menores | Errores en más del 30% | No reconoce la relación número-carácter |
| **Análisis de overflow** | Identifica el problema, el tipo correcto y los efectos | Identifica el problema pero el tipo propuesto no es óptimo | Identifica parcialmente | No relaciona bits con rangos |
| **Reflexión** | Argumentación sólida, usa vocabulario técnico correcto | Argumentación parcial | Ideas correctas sin desarrollo | Respuesta muy corta o incorrecta |

---

*Material elaborado para educación media. Se permite su uso y adaptación con fines educativos no comerciales.*  
*Versión 1.0 — Publicado en GitHub*
