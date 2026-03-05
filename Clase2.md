# 📚 Teoría de Conjuntos
### Guía Completa para Estudiantes · Matemáticas Discretas

> **Nivel:** Bachillerato (16 años aprox.)
> **Duración:** 4 horas de clase + 30 minutos de descanso
> **Modalidad:** Presencial / Virtual
> **Autor:** Material educativo de libre uso

---

## 🗓️ Agenda de la Clase

| Bloque | Tiempo | Contenido |
|--------|--------|-----------|
| 🟢 Bloque 1 | 0:00 – 1:00 h | ¿Qué es un conjunto? Representaciones y elementos |
| 🔵 Bloque 2 | 1:00 – 2:00 h | Tipos de conjuntos y relaciones entre conjuntos |
| ☕ Descanso | 2:00 – 2:30 h | Pausa activa |
| 🟠 Bloque 3 | 2:30 – 3:30 h | Operaciones con conjuntos y Diagramas de Venn |
| 🔴 Bloque 4 | 3:30 – 4:30 h | Aplicación en algoritmos + Taller gráfico + Retroalimentación |

---

# 🟢 BLOQUE 1 — ¿Qué es un Conjunto?

## 1.1 Definición Intuitiva

Imagina que llegas a casa después del colegio y tu mamá te pide que **organices tu cuarto**. Empiezas a agrupar cosas:

- 👟 Un grupo con todos tus zapatos
- 📱 Un grupo con todos tus dispositivos electrónicos
- 📚 Un grupo con todos tus libros

¡Acabas de crear **conjuntos** sin darte cuenta! Un conjunto es simplemente **una colección de objetos bien definidos**, a los que llamamos **elementos** o **miembros**.

> 🎓 **Definición formal:**
> Un **conjunto** es una colección bien definida de objetos distintos, llamados **elementos**, que comparten alguna característica o propiedad en común.

La palabra clave aquí es **"bien definido"**: para cualquier objeto del universo, debe ser posible determinar de forma clara y sin ambigüedad si pertenece o no al conjunto.

---

## 1.2 Ejemplos Cotidianos

| Conjunto | ¿Qué agrupa? | Ejemplos de elementos |
|----------|-------------|----------------------|
| 🎮 Los videojuegos de tu colección | Juegos que posees | FIFA 24, Minecraft, GTA V |
| 🌎 Los países de Sudamérica | Países del continente | Colombia, Brasil, Argentina |
| 🎵 Las canciones de tu playlist favorita | Canciones guardadas | "Tití me preguntó", "Blinding Lights" |
| 🔢 Los números pares menores que 10 | Números con propiedad matemática | 2, 4, 6, 8 |
| 🏫 Los estudiantes de este salón | Personas en clase | Tú, tus compañeros |

---

## 1.3 ¿Cómo se Representa un Conjunto?

### ✏️ Notación: Letras Mayúsculas

Los conjuntos se nombran con **letras mayúsculas**: A, B, C, D... y sus elementos van entre **llaves `{ }`**.

```
A = {manzana, pera, uva, sandía}

B = {1, 2, 3, 4, 5}

C = {Colombia, México, Perú, Chile}
```

---

### 📋 Tres formas de representar un conjunto

#### 🔹 Forma 1 — Extensión (por lista)
Se escriben **todos los elementos** del conjunto entre llaves, separados por comas.

```
Vocales del alfabeto español:
V = {a, e, i, o, u}

Meses del año que empiezan con "J":
M = {enero, junio, julio}

Números del 1 al 5:
N = {1, 2, 3, 4, 5}
```

> ✅ Úsala cuando el conjunto tiene **pocos elementos** o cuando es práctico listarlos todos.

---

#### 🔹 Forma 2 — Comprensión (por descripción o regla)
Se describe la **propiedad** que deben cumplir los elementos. Se usa la notación `{ x | propiedad de x }` que se lee "el conjunto de todos los x tal que...".

```
N = { x | x es un número natural menor que 6 }
→ Leemos: "El conjunto de todos los x tal que x es un número natural menor que 6"
→ Resultado: N = {1, 2, 3, 4, 5}

P = { x | x es un país de América del Sur }
→ Leemos: "El conjunto de todos los x tal que x es un país de América del Sur"
```

> ✅ Úsala cuando el conjunto tiene **muchos elementos** o una **regla clara**.

---

#### 🔹 Forma 3 — Diagrama (representación visual)
Se dibuja una **región cerrada** (óvalo o círculo) y se escriben los elementos dentro.

```
┌─────────────────────┐
│   A = Frutas rojas  │
│                     │
│  🍎 manzana         │
│  🍓 fresa           │
│  🍒 cereza          │
│  🌹 frambuesa       │
│                     │
└─────────────────────┘
```

> ✅ Úsala para **visualizar** conjuntos y sus relaciones (¡muy útil en Venn!).

---

## 1.4 La Pertenencia: El Símbolo ∈ y ∉

Para indicar si un elemento **pertenece** o **no pertenece** a un conjunto usamos:

| Símbolo | Significado | Ejemplo |
|---------|-------------|---------|
| `∈` | **Pertenece a** | Si A = {1, 2, 3}, entonces **2 ∈ A** ✅ |
| `∉` | **No pertenece a** | Si A = {1, 2, 3}, entonces **7 ∉ A** ❌ |

**Ejemplos cotidianos:**

```
Sea J = {juegos de mesa} = {ajedrez, monopolio, parqués, parchís}

✅ ajedrez ∈ J         → El ajedrez SÍ pertenece a J
✅ parqués ∈ J         → El parqués SÍ pertenece a J
❌ fútbol ∉ J          → El fútbol NO pertenece a J
❌ videojuegos ∉ J     → Los videojuegos NO pertenecen a J
```

---

## 1.5 Cardinalidad: ¿Cuántos elementos tiene un conjunto?

La **cardinalidad** es simplemente la **cantidad de elementos** de un conjunto. Se escribe `|A|` o `n(A)`.

```
A = {🍕, 🍔, 🌮, 🍜, 🥗}    →   |A| = 5

B = {2, 4, 6, 8, 10, 12}      →   |B| = 6

C = {Colombia}                 →   |C| = 1

D = { }   (vacío)              →   |D| = 0
```

---

### 🧩 ACTIVIDAD 1.1 — Calentamiento (10 minutos)
> **Instrucción para el docente:** Cada estudiante trabaja individualmente. Compartir respuestas en voz alta.

**Escribe en notación de extensión los siguientes conjuntos:**

1. El conjunto de las asignaturas que ves este año en el colegio.
2. El conjunto de los planetas del sistema solar.
3. El conjunto de los números pares entre 10 y 20.
4. El conjunto de tus 5 canciones favoritas en este momento.

**Determina si las siguientes afirmaciones son Verdaderas (V) o Falsas (F):**

Dado: `A = {lunes, martes, miércoles, jueves, viernes}`

- [ ] `sábado ∈ A`
- [ ] `lunes ∈ A`
- [ ] `domingo ∉ A`
- [ ] `|A| = 7`
- [ ] `viernes ∈ A`

> 💡 **Respuestas:** F, V, V, F, V

---

# 🔵 BLOQUE 2 — Tipos de Conjuntos y Relaciones

## 2.1 Tipos Especiales de Conjuntos

### 🔸 Conjunto Vacío (∅ o { })
Un conjunto que **no tiene ningún elemento**. Es como una caja completamente vacía.

```
∅ = { }

Ejemplos de conjuntos vacíos:
• El conjunto de los meses del año con 32 días → { }
• El conjunto de los números que son pares e impares al mismo tiempo → { }
• El conjunto de los elefantes que saben volar → { }
```

> ⚠️ **Cuidado:** `{∅}` NO es un conjunto vacío, ¡tiene un elemento que es el vacío mismo!

---

### 🔸 Conjunto Unitario
Tiene exactamente **un solo elemento**.

```
U = {el Sol}           → El conjunto que contiene solo al Sol
P = {0}                → El conjunto que contiene solo al cero
```

---

### 🔸 Conjunto Universal (U o Ω)
Es el conjunto que **contiene todos los elementos** posibles dentro de un contexto dado. Es el "universo" de referencia.

```
Si hablamos de animales domésticos:
U = {perro, gato, conejo, hámster, pez, loro, tortuga, ...}

Si hablamos de dígitos:
U = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}
```

---

### 🔸 Conjunto Finito e Infinito

| Tipo | Descripción | Ejemplo |
|------|-------------|---------|
| **Finito** | Tiene un número contable de elementos | `{1, 2, 3, 4, 5}` |
| **Infinito** | Sus elementos no se agotan | `{1, 2, 3, 4, 5, ...}` (números naturales) |

---

## 2.2 Relaciones Entre Conjuntos

### 🔹 Igualdad de Conjuntos
Dos conjuntos son **iguales** si tienen exactamente los mismos elementos (sin importar el orden ni las repeticiones).

```
A = {1, 2, 3}
B = {3, 1, 2}
→ A = B ✅  (mismo contenido, distinto orden → iguales)

C = {a, b, b, c}
D = {a, b, c}
→ C = D ✅  (las repeticiones no cuentan)
```

---

### 🔹 Subconjunto (⊆)
A es **subconjunto** de B si **todos los elementos de A también están en B**.

```
A ⊆ B  →  "A está contenido en B"

Ejemplo:
A = {perro, gato}
B = {perro, gato, pez, loro, conejo}
→ A ⊆ B ✅  (todo lo de A está en B)

Visualización:
┌──────────────────────────────────┐
│  B                               │
│   ┌────────────┐                 │
│   │  A         │  pez            │
│   │  perro     │  loro           │
│   │  gato      │  conejo         │
│   └────────────┘                 │
└──────────────────────────────────┘
```

> 🧠 **Regla importante:** El conjunto vacío `∅` es subconjunto de **cualquier** conjunto.

---

### 🔹 Subconjunto Propio (⊂)
A es **subconjunto propio** de B si `A ⊆ B` pero `A ≠ B` (hay al menos un elemento en B que no está en A).

```
A = {2, 4}     B = {2, 4, 6, 8}
A ⊂ B ✅  →  A está "dentro" de B y B tiene elementos adicionales
```

---

## 2.3 El Complemento: Lo que "no está"

El **complemento** de un conjunto A (escrito A' o Aᶜ) contiene **todos los elementos del conjunto universal que NO están en A**.

```
U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {2, 4, 6, 8, 10}  (números pares)

A' = {1, 3, 5, 7, 9}  (números impares → lo que no estaba en A)

┌─────────────────────────────────────────┐
│  U (universo)                           │
│  ┌──────────────────┐                   │
│  │   A              │  1   3   5        │
│  │   2  4  6  8  10 │  7   9            │
│  └──────────────────┘       ← A'        │
└─────────────────────────────────────────┘
```

---

### 🧩 ACTIVIDAD 2.1 — Clasificación de Conjuntos (15 minutos)
> **Instrucción:** Trabajo en parejas. Cada pareja tiene 5 minutos para resolver y luego se comparte en clase.

**Clasifica cada conjunto como: Vacío / Unitario / Finito / Infinito**

1. `A = {x | x es un triángulo con 4 lados}` → ___________
2. `B = {x | x es el número natural entre 3 y 4}` → ___________
3. `C = {x | x es un múltiplo de 5}` → ___________
4. `D = {Colombia}` → ___________
5. `E = {1, 3, 5, 7, 9, 11, 13}` → ___________

**Dado:**
```
U = {a, b, c, d, e, f, g, h}
A = {a, b, c, d}
B = {c, d, e, f}
```

Responde:
- ¿Es `A ⊆ U`? ___
- ¿Es `B ⊆ A`? ___
- ¿Cuál es `A'`? ___
- ¿Cuál es `B'`? ___

> 💡 **Respuestas:** Vacío, Vacío, Infinito, Unitario, Finito | Sí, No, {e,f,g,h}, {a,b,g,h}

---

# ☕ DESCANSO — 30 minutos

> 🎯 **Sugerencia para el docente:** Antes del descanso, proponer este mini-reto mental:
>
> *"Piensa en 3 conjuntos de tu vida cotidiana que se relacionen entre sí. Por ejemplo: las aplicaciones de tu celular que usan internet, las aplicaciones que usas para estudiar y las aplicaciones que usas para entretenerte. ¿Hay apps que estén en más de uno?"*
>
> Los estudiantes compartirán sus respuestas al inicio del Bloque 3. 🔥

---

# 🟠 BLOQUE 3 — Operaciones con Conjuntos y Diagramas de Venn

## 3.1 ¿Qué son los Diagramas de Venn?

Los **Diagramas de Venn** son representaciones visuales que muestran **cómo se relacionan dos o más conjuntos**. Fueron creados por el matemático inglés **John Venn** en 1880.

```
      ┌─────────────────────────────────────────────┐
      │  U (Universo)                               │
      │                                             │
      │    ╔═══════════╗   ╔═══════════╗            │
      │    ║     A     ║   ║     B     ║            │
      │    ║           ║   ║           ║            │
      │    ║  solo A   ║   ║  solo B   ║            │
      │    ║           ╠═══╣           ║            │
      │    ║           ║A∩B║           ║            │
      │    ╚═══════════╩═══╩═══════════╝            │
      │                                             │
      └─────────────────────────────────────────────┘
```

---

## 3.2 Operaciones Fundamentales

### ➕ Unión (A ∪ B)
La unión contiene **todos los elementos de A, de B, o de ambos**.

> 🧠 Regla mnemotécnica: **Unión = Uno más el otro = TODO**

```
A = {🍕 pizza, 🍔 hamburguesa, 🌮 taco}
B = {🍔 hamburguesa, 🥗 ensalada, 🍜 ramen}

A ∪ B = {pizza, hamburguesa, taco, ensalada, ramen}
       (hamburguesa aparece en ambos, pero se escribe UNA sola vez)

Diagrama de Venn:
      ╔═══════════╦═══════════╗
      ║     A     ║     B     ║
      ║  pizza    ║  ensalada ║
      ║  taco     ║  ramen    ║
      ║       hamburguesa     ║
      ╚═══════════╩═══════════╝
      ↑_______________________↑
              A ∪ B
              (todo lo sombreado)
```

**Fórmula:** `|A ∪ B| = |A| + |B| - |A ∩ B|`

---

### ✖️ Intersección (A ∩ B)
La intersección contiene **solo los elementos que están en A Y en B al mismo tiempo**.

> 🧠 Regla mnemotécnica: **Intersección = lo que está en el medio = LO COMÚN**

```
A = {2, 4, 6, 8, 10}      (múltiplos de 2 hasta 10)
B = {3, 6, 9, 12} ∩ A     (múltiplos de 3)

A ∩ B = {6}
       (solo el 6 está en ambos)

Diagrama de Venn:
      ╔═══════════╦═══╦═══════════╗
      ║     A     ║   ║     B     ║
      ║  2  4     ║ 6 ║  3  9 12 ║
      ║  8  10    ║   ║           ║
      ╚═══════════╩═══╩═══════════╝
                  ↑
               A ∩ B
```

---

### ➖ Diferencia (A − B)
La diferencia A − B contiene **los elementos que están en A pero NO están en B**.

> 🧠 Regla mnemotécnica: **Diferencia = A "quita" lo que tiene de B = Solo A puro**

```
A = {perro, gato, pez, loro}
B = {gato, loro, tortuga}

A − B = {perro, pez}
       (quitamos de A lo que también está en B)

B − A = {tortuga}
       (quitamos de B lo que también está en A)

⚠️ OJO: A − B ≠ B − A  (la diferencia NO es conmutativa)

Diagrama de Venn:
      ╔═══════════╦═══════════╦═══════════╗
      ║  A − B    ║   A ∩ B   ║   B − A   ║
      ║  perro    ║   gato    ║  tortuga  ║
      ║  pez      ║   loro    ║           ║
      ╚═══════════╩═══════════╩═══════════╝
      ↑_________↑              ↑_________↑
        solo A                   solo B
```

---

### 🔄 Resumen Visual de Operaciones

```
UNIÓN A ∪ B          INTERSECCIÓN A ∩ B     DIFERENCIA A − B
╔══════╦══════╗       ╔══════╦══════╗         ╔══════╦══════╗
║██████║██████║       ║      ║      ║         ║██████║      ║
║██████║██████║       ║      ║██████║         ║██████║      ║
╚══════╩══════╝       ╚══════╩══════╝         ╚══════╩══════╝
  Todo sombreado      Solo el centro          Solo lado A

COMPLEMENTO A'
╔══════════════════╗
║██████╔════╗██████║
║██████║ A  ║██████║
║██████╚════╝██████║
╚══════════════════╝
  Todo excepto A
```

---

## 3.3 Leyes y Propiedades

| Propiedad | Unión | Intersección |
|-----------|-------|--------------|
| **Conmutativa** | `A ∪ B = B ∪ A` | `A ∩ B = B ∩ A` |
| **Asociativa** | `(A ∪ B) ∪ C = A ∪ (B ∪ C)` | `(A ∩ B) ∩ C = A ∩ (B ∩ C)` |
| **Identidad** | `A ∪ ∅ = A` | `A ∩ U = A` |
| **Complemento** | `A ∪ A' = U` | `A ∩ A' = ∅` |

---

## 3.4 Ejemplo Integrador: Tres Conjuntos

**Situación:** En un grupo de 30 estudiantes, se investigó cuáles practican deportes:

```
F = {estudiantes que juegan fútbol}
B = {estudiantes que juegan baloncesto}
V = {estudiantes que juegan voleibol}
```

**Datos:**
- Solo fútbol: 8
- Solo baloncesto: 6
- Solo voleibol: 4
- Fútbol y baloncesto (no voleibol): 3
- Fútbol y voleibol (no baloncesto): 2
- Baloncesto y voleibol (no fútbol): 2
- Los tres deportes: 1

```
┌─────────────────────────────────────────────────┐
│  U = 30 estudiantes                             │
│  ┌─────────────┐    ┌─────────────┐             │
│  │      F      │    │      B      │             │
│  │     (8)     │    │     (6)     │             │
│  │         (3) │    │ (2)         │             │
│  │      ┌──────┼────┼──────┐      │             │
│  │      │  (2) │(1) │      │      │             │
│  └──────┼──────┘    └──────┼──────┘             │
│         │      V           │                    │
│         │     (4)          │                    │
│         └──────────────────┘                    │
│  Ningún deporte: 30 - (8+6+4+3+2+2+1) = 4      │
└─────────────────────────────────────────────────┘
```

**Preguntas:**
- ¿Cuántos juegan fútbol? → `8 + 3 + 2 + 1 = 14`
- ¿Cuántos juegan exactamente 2 deportes? → `3 + 2 + 2 = 7`
- ¿Cuántos no practican ningún deporte? → `30 - 26 = 4`

---

### 🧩 ACTIVIDAD 3.1 — Taller Gráfico de Conjuntos (25 minutos)
> **Instrucción:** Grupos de 3-4 personas. Cada grupo dibuja en papel o en herramienta digital.

#### 🎨 Parte A — Construye tu Diagrama (15 min)

Dado el siguiente contexto:

*En tu colegio, un grupo de 40 estudiantes fue encuestado sobre sus apps favoritas:*

```
R = {usan redes sociales} = {Instagram, TikTok, Twitter/X, Facebook}
M = {usan apps de música} = {Spotify, YouTube Music, Apple Music}
J = {usan apps de juegos} = {Roblox, Minecraft, Free Fire, Among Us}

Datos adicionales:
• 20 usan solo redes sociales
• 10 usan solo música
• 5 usan solo juegos
• 3 usan redes sociales Y música
• 2 usan redes sociales Y juegos
• 1 usa música Y juegos
• 0 usan las tres categorías
```

**Tu tarea:**
1. 📐 Dibuja el Diagrama de Venn con los tres conjuntos R, M y J
2. 🔢 Ubica correctamente los números en cada región
3. 📊 Calcula cuántos estudiantes no usan ninguna de estas apps

#### 🔍 Parte B — Análisis (10 min)

Con base en tu diagrama, responde:
1. ¿Cuántos estudiantes usan al menos una app? ¿Y cuántos no usan ninguna?
2. Calcula: `R ∪ M ∪ J` (total de elementos)
3. Calcula: `R ∩ M` (los que usan redes sociales Y música)
4. ¿Quiénes pertenecen a `M − R`? (música pero no redes)
5. ¿Qué representa el complemento `(R ∪ M ∪ J)'`?

> 💡 **Solución guiada:**
> Total usando apps = 20+10+5+3+2+1+0 = 41... ¡Eso supera los 40!
> Discute con tu grupo: ¿Qué error hay en los datos? ¿Cómo lo corregirías? (Actividad de pensamiento crítico)

---

# 🔴 BLOQUE 4 — Conjuntos en Algoritmos + Taller Final

## 4.1 ¿Por qué los Conjuntos son Importantes en Computación?

Imagina que eres el creador de una app. Necesitas organizar información de miles de usuarios. ¿Cómo lo harías? ¡Los conjuntos son la respuesta!

> 🖥️ **Los conjuntos son la base matemática de:**
> - Bases de datos (SQL usa operaciones de conjuntos)
> - Buscadores como Google
> - Sistemas de recomendación (Netflix, Spotify)
> - Redes sociales (amigos en común)
> - Motores de búsqueda y filtros

---

## 4.2 Conjuntos en la Vida de un Programador

### 🔍 Ejemplo 1: Filtros de Búsqueda

Cuando buscas algo en una tienda online y aplicas filtros:

```
U = {todos los productos de la tienda}
A = {productos con precio < $50.000}
B = {productos de color azul}
C = {productos con envío gratis}

Si aplicas TODOS los filtros:  A ∩ B ∩ C
Si aplicas CUALQUIER filtro:   A ∪ B ∪ C
Si excluyes envío gratis:      (A ∩ B) − C
```

---

### 🔍 Ejemplo 2: Amigos en Común (Redes Sociales)

```python
# En programación, esto se ve así:
amigos_de_juan  = {"María", "Pedro", "Luisa", "Carlos", "Ana"}
amigos_de_sofia = {"Pedro", "Luis",  "Ana",   "Diego",  "María"}

# Amigos en común (Intersección):
en_comun = amigos_de_juan & amigos_de_sofia
# Resultado: {"María", "Pedro", "Ana"}

# Todos sus amigos (Unión):
todos = amigos_de_juan | amigos_de_sofia
# Resultado: {"María", "Pedro", "Luisa", "Carlos", "Ana", "Luis", "Diego"}

# Amigos solo de Juan (Diferencia):
solo_juan = amigos_de_juan - amigos_de_sofia
# Resultado: {"Luisa", "Carlos"}
```

> 💡 ¡Python tiene un tipo de dato llamado `set` que implementa exactamente la teoría de conjuntos!

---

### 🔍 Ejemplo 3: Consultas en Bases de Datos (SQL)

```sql
-- Unión: todos los clientes de Colombia O de México
SELECT nombre FROM clientes WHERE pais = 'Colombia'
UNION
SELECT nombre FROM clientes WHERE pais = 'México';

-- Intersección: clientes que compraron en enero Y en febrero
SELECT cliente_id FROM ventas WHERE mes = 'enero'
INTERSECT
SELECT cliente_id FROM ventas WHERE mes = 'febrero';

-- Diferencia: clientes que compraron en enero pero NO en febrero
SELECT cliente_id FROM ventas WHERE mes = 'enero'
EXCEPT
SELECT cliente_id FROM ventas WHERE mes = 'febrero';
```

---

### 🔍 Ejemplo 4: Algoritmo de Recomendación

```
Perfil de usuario A: le gustan {acción, comedia, ciencia ficción}
Perfil de usuario B: le gustan {drama, comedia, romance}

Géneros en común: {acción, comedia, ciencia ficción} ∩ {drama, comedia, romance}
                = {comedia}

El sistema recomienda: "A otros usuarios como tú también les gusta la comedia.
Te recomendamos estas películas de ese género..."
```

---

## 4.3 Tabla: Matemáticas vs. Programación

| Concepto Matemático | Símbolo | Python | SQL |
|--------------------|---------|--------|-----|
| Conjunto | `A = {1,2,3}` | `A = {1,2,3}` | Tabla/columna |
| Unión | `A ∪ B` | `A \| B` | `UNION` |
| Intersección | `A ∩ B` | `A & B` | `INTERSECT` |
| Diferencia | `A − B` | `A - B` | `EXCEPT` |
| Pertenencia | `x ∈ A` | `x in A` | `WHERE x IN (...)` |
| Subconjunto | `A ⊆ B` | `A.issubset(B)` | `EXISTS` |
| Complemento | `A'` | `U - A` | `NOT IN` |

---

## 4.4 🏆 TALLER FINAL — Aplicación Integral (40 minutos)

> **Instrucción:** Trabajo en grupos de 4-5 personas. Cada grupo presenta sus respuestas al final.
> **Materiales:** Papel grande / tablero / herramienta digital de diagramas.

---

### 🎯 Problema Central: "La Red Social del Colegio"

*El colegio quiere crear una app interna. Se encuestaron 50 estudiantes sobre sus hábitos digitales:*

**Datos de la encuesta:**

| Categoría | Conjunto | Descripción |
|-----------|----------|-------------|
| T | TikTok | Usan TikTok diariamente |
| I | Instagram | Usan Instagram diariamente |
| Y | YouTube | Usan YouTube diariamente |

**Resultados:**
- Usan **solo TikTok**: 12 estudiantes
- Usan **solo Instagram**: 8 estudiantes
- Usan **solo YouTube**: 10 estudiantes
- Usan **TikTok e Instagram** (no YouTube): 5 estudiantes
- Usan **TikTok y YouTube** (no Instagram): 4 estudiantes
- Usan **Instagram y YouTube** (no TikTok): 3 estudiantes
- Usan **las tres plataformas**: 2 estudiantes
- **No usan ninguna**: el resto

---

#### 📝 Parte 1 — Diagrama de Venn (10 min)
1. Dibuja el Diagrama de Venn con los tres conjuntos T, I, Y
2. Coloca los valores numéricos en cada región correctamente
3. Calcula cuántos estudiantes no usan ninguna plataforma

---

#### 🔢 Parte 2 — Operaciones (15 min)

Calcula y describe en palabras qué representa cada operación:

| Operación | Resultado numérico | ¿Qué significa en contexto? |
|-----------|-------------------|-----------------------------|
| `\|T\|` | ___ | ___ |
| `\|I\|` | ___ | ___ |
| `T ∪ I` | ___ | ___ |
| `T ∩ I` | ___ | ___ |
| `T − Y` | ___ | ___ |
| `(T ∪ I ∪ Y)'` | ___ | ___ |
| `T ∩ I ∩ Y` | ___ | ___ |

---

#### 💻 Parte 3 — Pensamiento Algorítmico (10 min)

*La app del colegio necesita enviar notificaciones. Responde:*

1. **Notificación A:** "¡Nuevo reto de baile!" → ¿A qué conjunto enviarías esto?
2. **Notificación B:** "¡Tendencias musicales del mes!" → ¿Qué operación usarías para llegar a usuarios de TikTok O YouTube?
3. **Notificación C:** "Descuento en cámara profesional" → ¿A qué conjunto enviarías esto? (usuarios que usan Instagram Y YouTube, creativos visuales)
4. **Notificación D:** "App de estudio sin distracciones" → ¿Cómo identificas a los que NO usan ninguna red?

---

#### 🎤 Parte 4 — Presentación y Debate (5 min por grupo)

Cada grupo presenta:
1. Su Diagrama de Venn (máx. 1 minuto)
2. La operación que más les costó entender y cómo la resolvieron
3. **Pregunta estrella:** ¿En qué otra situación de su vida cotidiana aplicarían esta operación?

---

## 4.5 Retroalimentación Guiada

### 🔄 Ronda de Preguntas Generadoras
> **Instrucción docente:** Estas preguntas generan reflexión y participación activa. Lanzar una por una y esperar respuestas antes de revelar la correcta.

---

**🟡 Nivel Básico — "¿Entendí lo esencial?"**

> ❓ *"Si A = {días de la semana que empiezan con 'M'}, ¿cuál es la cardinalidad de A?"*

<details>
<summary>📖 Ver respuesta</summary>

`A = {lunes, martes, miércoles}` → `|A| = 3`

</details>

---

> ❓ *"¿Puede el conjunto vacío ser subconjunto de A = {1, 2, 3}?"*

<details>
<summary>📖 Ver respuesta</summary>

**Sí.** El conjunto vacío ∅ es subconjunto de **cualquier** conjunto. Por definición, ningún elemento de ∅ viola la condición de estar en A (porque ∅ no tiene elementos que violarla).

</details>

---

**🟠 Nivel Intermedio — "¿Lo sé aplicar?"**

> ❓ *"En una clase de 30 estudiantes: 18 hablan inglés, 12 hablan francés, y 5 hablan ambos. ¿Cuántos hablan al menos uno de los dos idiomas?"*

<details>
<summary>📖 Ver respuesta</summary>

Usamos la fórmula de la unión:

`|A ∪ B| = |A| + |B| - |A ∩ B|`
`|A ∪ B| = 18 + 12 - 5 = 25 estudiantes`

Los 5 restantes no hablan ninguno de los dos idiomas.

</details>

---

> ❓ *"Si A ⊆ B y B ⊆ A al mismo tiempo, ¿qué podemos concluir?"*

<details>
<summary>📖 Ver respuesta</summary>

Que `A = B`. Si todo elemento de A está en B, y todo elemento de B está en A, entonces ambos conjuntos tienen exactamente los mismos elementos.

</details>

---

**🔴 Nivel Avanzado — "¿Puedo ir más allá?"**

> ❓ *"Tienes una lista de canciones sin repetir. La divides en las que son de reggaeton (R) y las que son en inglés (I). Hay canciones de reggaeton en inglés. Diseña una consulta (en lenguaje cotidiano) para encontrar: las canciones en inglés que NO son de reggaeton."*

<details>
<summary>📖 Ver respuesta</summary>

Eso corresponde a la **diferencia** `I − R`:

*"Dame todas las canciones en inglés, pero excluye las que también sean de reggaeton."*

En Python: `I - R`
En SQL: `SELECT cancion FROM lista WHERE idioma = 'inglés' EXCEPT SELECT cancion FROM lista WHERE genero = 'reggaeton'`

</details>

---

> ❓ *"¿Por qué es importante que un conjunto esté 'bien definido'? Da un ejemplo de un 'pseudo-conjunto' que no esté bien definido."*

<details>
<summary>📖 Ver respuesta</summary>

Un conjunto debe ser "bien definido" porque necesitamos poder determinar con certeza si cualquier elemento pertenece o no a él.

**Ejemplo de pseudo-conjunto mal definido:**
`X = {los estudiantes altos del salón}`

¿Qué es "alto"? ¿Alto para quién? ¿Más de 1.70m? ¿Más de 1.80m? La ambigüedad hace que diferentes personas incluyan o excluyan distintos elementos. **Esto NO es un conjunto válido.**

Un conjunto válido sería: `X = {estudiantes con estatura mayor a 1.75 metros}` → ahora sí es claro y medible.

</details>

---

## 4.6 Mapa Mental de la Clase

```
                    TEORÍA DE CONJUNTOS
                           │
          ┌────────────────┼────────────────┐
          │                │                │
   CONCEPTOS BASE    OPERACIONES      APLICACIONES
          │                │                │
    ┌─────┴─────┐    ┌─────┴─────┐    ┌─────┴─────┐
    │           │    │           │    │           │
 Definición  Notac. Unión(∪)  Intersec. Algoritmos
 Elemento    Exten. Diferencia Complement Bases datos
 Cardinal.   Compr. A-B       A'        Python sets
 Pertenencia Diagr. A∪B       A∩B       SQL queries
    │
  Tipos
    │
 ┌──┴──┐
Vacío  Finito
Unit.  Infinito
Univ.  Subconjunto
```

---

# 📋 Resumen de Conceptos Clave

| Concepto | Símbolo | Definición rápida | Ejemplo |
|----------|---------|------------------|---------|
| Conjunto | `A = { }` | Colección bien definida de elementos | `A = {1, 2, 3}` |
| Pertenencia | `∈` / `∉` | Indica si algo es o no elemento | `2 ∈ A` |
| Cardinalidad | `\|A\|` | Número de elementos | `\|{a,b,c}\| = 3` |
| Conjunto vacío | `∅` | Sin elementos | `∅ = { }` |
| Conjunto universal | `U` | Todos los elementos del contexto | `U = {0...9}` |
| Subconjunto | `⊆` | Todos los de A están en B | `{1,2} ⊆ {1,2,3}` |
| Unión | `∪` | Todo A más todo B | `{1,2}∪{2,3}={1,2,3}` |
| Intersección | `∩` | Solo lo común | `{1,2}∩{2,3}={2}` |
| Diferencia | `−` | A sin lo de B | `{1,2}−{2,3}={1}` |
| Complemento | `A'` | Lo que no está en A | Si U={1,2,3}, A={1}, A'={2,3} |

---

# 📚 Recursos para Profundizar

### Herramientas Online Gratuitas

| Herramienta | Enlace | Para qué sirve |
|-------------|--------|----------------|
| **GeoGebra** | [geogebra.org](https://www.geogebra.org) | Crear diagramas de Venn interactivos |
| **Canva** | [canva.com](https://www.canva.com) | Diseñar diagramas visuales |
| **Creately** | [creately.com](https://creately.com) | Diagramas de Venn colaborativos |
| **Symbolab** | [symbolab.com](https://www.symbolab.com) | Resolver problemas de conjuntos paso a paso |
| **Python (Replit)** | [replit.com](https://replit.com) | Practicar conjuntos en código real |

### Para Seguir Aprendiendo

- 📖 **Khan Academy Español** → Teoría de conjuntos básica (gratuito)
- 🎬 **YouTube: "ProfesorGiuseppe"** → Videos en español sobre conjuntos
- 📗 **"Matemáticas Discretas" - Rosen** → Referencia académica completa
- 💻 **Codecademy** → Sets en Python (aplicación práctica)

---

# ✅ Autoevaluación Final

> Antes de salir, marca honestamente cuánto dominas cada concepto:

| Concepto | 😕 Confundido | 🤔 Más o menos | 😊 Lo entiendo | 🚀 Puedo explicarlo |
|----------|:---:|:---:|:---:|:---:|
| Qué es un conjunto y sus elementos | ☐ | ☐ | ☐ | ☐ |
| Representación por extensión | ☐ | ☐ | ☐ | ☐ |
| Representación por comprensión | ☐ | ☐ | ☐ | ☐ |
| Símbolos ∈, ∉, ⊆, ∅ | ☐ | ☐ | ☐ | ☐ |
| Cardinalidad | ☐ | ☐ | ☐ | ☐ |
| Unión (A ∪ B) | ☐ | ☐ | ☐ | ☐ |
| Intersección (A ∩ B) | ☐ | ☐ | ☐ | ☐ |
| Diferencia (A − B) | ☐ | ☐ | ☐ | ☐ |
| Complemento (A') | ☐ | ☐ | ☐ | ☐ |
| Diagramas de Venn | ☐ | ☐ | ☐ | ☐ |
| Aplicación en algoritmos/código | ☐ | ☐ | ☐ | ☐ |

---

# 🏅 Reto Bonus — Para los que Quieran Más

**¿Puedes demostrar la Ley de De Morgan?**

La Ley de De Morgan establece:

```
1. (A ∪ B)' = A' ∩ B'
2. (A ∩ B)' = A' ∪ B'
```

**Desafío:** Usando el siguiente universo y conjuntos, verifica AMBAS leyes:

```
U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}
```

> Pista: Calcula cada lado de la ecuación por separado y verifica que sean iguales. Si lo logras, ¡tienes un nivel universitario de teoría de conjuntos! 🎓

---

*📄 Material creado para uso educativo libre — Teoría de Conjuntos · Bachillerato*
*🔗 Compatible con GitHub Markdown · Última actualización: 2026*

---
> *"Las matemáticas son el lenguaje en el que Dios escribió el universo."*
> — Galileo Galilei
