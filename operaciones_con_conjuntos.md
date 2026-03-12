# 🔢 Operaciones con Conjuntos: Del Álgebra al Código

> **Nivel:** Grado 10° · **Edad:** 15–16 años  
> **Duración total:** 4 horas (2 sesiones con descansos)  
> **Modalidad:** Presencial / Híbrida  
> **Autores:** _(escribe aquí el nombre del docente)_

---

## 📋 Tabla de Contenidos

1. [¿Qué vamos a aprender hoy?](#1--qué-vamos-a-aprender-hoy)
2. [Repaso rápido: ¿Qué es un conjunto?](#2--repaso-rápido-qué-es-un-conjunto)
3. [Unión de Conjuntos (A ∪ B)](#3--unión-de-conjuntos-a--b)
4. [Intersección de Conjuntos (A ∩ B)](#4--intersección-de-conjuntos-a--b)
5. [Diferencia de Conjuntos (A − B)](#5--diferencia-de-conjuntos-a--b)
6. [Complemento de un Conjunto (Aᶜ)](#6--complemento-de-un-conjunto-aᶜ)
7. [⏸️ DESCANSO 1](#️-descanso-1--15-minutos)
8. [Conjuntos en Programación](#8--conjuntos-y-lógica-en-programación)
9. [Trabajo Colaborativo en Equipos](#9--trabajo-colaborativo-en-equipos)
10. [⏸️ DESCANSO 2](#️-descanso-2--15-minutos)
11. [Ejercicios de Aplicación](#11--ejercicios-de-aplicación-individual)
12. [Reto Final: El Gran Desafío](#12--reto-final-el-gran-desafío)
13. [Resumen y Cierre](#13--resumen-y-cierre)

---

## ⏱️ Planificación de la Sesión

| Bloque | Contenido | Duración | Acumulado |
|--------|-----------|----------|-----------|
| 1 | Introducción y repaso | 20 min | 20 min |
| 2 | Unión e Intersección | 35 min | 55 min |
| 3 | Diferencia y Complemento | 35 min | 90 min |
| 4 | Ejercicios escritos individuales | 30 min | 120 min |
| ☕ | **DESCANSO 1** | 15 min | 135 min |
| 5 | Conjuntos en Programación | 30 min | 165 min |
| 6 | Trabajo colaborativo en equipos | 45 min | 210 min |
| ☕ | **DESCANSO 2** | 15 min | 225 min |
| 7 | Ejercicios de aplicación + reto final | 30 min | 255 min |
| 8 | Socialización y cierre | 15 min | 270 min* |

> *El margen adicional (~30 min) está previsto para preguntas, socialización de equipos y evaluación formativa.

---

## 1. 🎯 ¿Qué vamos a aprender hoy?

> **⏱️ Tiempo estimado: 10 minutos**

Imagina que tienes dos listas de reproducción en Spotify:

- 🎵 **Lista A:** las canciones que escuchas cuando estudias
- 🎵 **Lista B:** las canciones que escuchas cuando entrenas

¿Qué pasa si quieres crear una nueva lista con **todas** esas canciones? ¿O solo las que comparten ambas listas? ¿O quieres eliminar las que ya escuchaste?

Eso es exactamente lo que hacen las **operaciones con conjuntos**.

### Objetivos de Aprendizaje

Al finalizar esta sesión podrás:

- ✅ Identificar y representar conjuntos usando notación simbólica y diagramas de Venn
- ✅ Aplicar las operaciones de **unión, intersección, diferencia y complemento**
- ✅ Relacionar estas operaciones con **condiciones lógicas en programación**
- ✅ Resolver problemas en equipo usando el pensamiento matemático

### 🧠 Activador de Conocimiento Previo

Antes de comenzar, responde en tu cuaderno:

1. ¿Qué es un conjunto? Da un ejemplo de la vida real.
2. ¿Conoces alguna app o programa que filtre información? ¿Cómo crees que lo hace?
3. En programación, ¿qué significa la condición `AND` y `OR`?

> 💬 **Comparte tu respuesta** con el compañero de al lado durante 2 minutos.

---

## 2. 📚 Repaso Rápido: ¿Qué es un Conjunto?

> **⏱️ Tiempo estimado: 10 minutos**

Un **conjunto** es una colección bien definida de elementos distintos.

### Formas de Representar un Conjunto

**1. Por extensión** (listando todos los elementos):
```
A = {1, 2, 3, 4, 5}
B = {perro, gato, loro, pez}
```

**2. Por comprensión** (describiendo la propiedad):
```
A = {x | x es un número natural par menor que 10}
A = {2, 4, 6, 8}
```

**3. Mediante diagrama de Venn:**

```
        Universo (U)
  ┌─────────────────────────┐
  │                         │
  │    ┌───────────┐        │
  │    │           │        │
  │    │     A     │        │
  │    │  {1,2,3}  │        │
  │    └───────────┘        │
  │                         │
  └─────────────────────────┘
```

### Notación Importante

| Símbolo | Significado | Ejemplo |
|---------|-------------|---------|
| `∈` | "pertenece a" | 3 ∈ A |
| `∉` | "no pertenece a" | 7 ∉ A |
| `⊆` | "es subconjunto de" | {1,2} ⊆ A |
| `∅` o `{}` | Conjunto vacío | ∅ |
| `U` | Conjunto universal | Todos los elementos posibles |
| `n(A)` | Cardinalidad | n({a,b,c}) = 3 |

### 🔍 Ejemplo Real

Sea U = {todos los estudiantes del curso}

```
A = {estudiantes que practican fútbol}
B = {estudiantes que tocan algún instrumento}
```

Con estos dos conjuntos podemos hacernos preguntas interesantes... ¡y las responderemos con operaciones!

---

## 3. 🔵🟡 Unión de Conjuntos (A ∪ B)

> **⏱️ Tiempo estimado: 17 minutos**

### Definición

La **unión** de dos conjuntos A y B es el conjunto formado por **todos los elementos que pertenecen a A, a B, o a ambos**.

```
A ∪ B = {x | x ∈ A  ó  x ∈ B}
```

> 🔑 **Palabra clave: "O"** — Para que un elemento esté en A ∪ B, basta con que esté en A **O** en B (o en los dos).

### Representación Gráfica

```
          A ∪ B  (zona sombreada = toda el área de los círculos)

    ┌─────────────────────────────────┐
    │  Universo (U)                   │
    │                                 │
    │   ┌───────────────────────┐     │
    │   │ A         │         B │     │
    │   │           │           │     │
    │   │  Solo A   │   Solo B  │     │
    │   │           │           │     │
    │   │        A ∩ B          │     │
    │   └───────────────────────┘     │
    │   [████████████████████████]    │
    │   Toda esta área = A ∪ B        │
    └─────────────────────────────────┘
```

### Ejemplo Numérico

```
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

A ∪ B = {1, 2, 3, 4, 5, 6, 7, 8}
```

> ⚠️ **¡Importante!** Los elementos que aparecen en los dos conjuntos (4 y 5) se escriben **una sola vez** en la unión.

### Diagrama de Venn Detallado

```
                A ∪ B

    ┌───────────────────────────────────────┐
    │ U                                     │
    │                                       │
    │   ┌───────────┬────────┬──────────┐   │
    │   │           │        │          │   │
    │   │  Solo A   │ A ∩ B  │  Solo B  │   │
    │   │  {1,2,3}  │ {4, 5} │ {6,7,8}  │   │
    │   │           │        │          │   │
    │   └───────────┴────────┴──────────┘   │
    │                                       │
    │           Todo esto = A ∪ B           │
    └───────────────────────────────────────┘
```

### Propiedades de la Unión

| Propiedad | Expresión |
|-----------|-----------|
| Conmutativa | A ∪ B = B ∪ A |
| Asociativa | (A ∪ B) ∪ C = A ∪ (B ∪ C) |
| Elemento neutro | A ∪ ∅ = A |
| Idempotente | A ∪ A = A |
| Con el universo | A ∪ U = U |

### ✏️ Practica Tú

**Ejercicio guiado:**

Sea:
```
P = {a, e, i, o, u}        (vocales)
Q = {a, b, c, d, e}        (primeras letras del alfabeto)
```

a) Halla P ∪ Q  
b) ¿Cuántos elementos tiene P ∪ Q? (Cardinalidad)  
c) Dibuja el diagrama de Venn correspondiente

> 💡 **Pista:** n(A ∪ B) = n(A) + n(B) − n(A ∩ B)

---

## 4. 🟢 Intersección de Conjuntos (A ∩ B)

> **⏱️ Tiempo estimado: 18 minutos**

### Definición

La **intersección** de dos conjuntos A y B es el conjunto de los elementos que pertenecen **a A Y también a B al mismo tiempo**.

```
A ∩ B = {x | x ∈ A  y  x ∈ B}
```

> 🔑 **Palabra clave: "Y"** — Un elemento está en A ∩ B solo si está en A **Y** en B simultáneamente.

### Representación Gráfica

```
          A ∩ B  (zona sombreada = solo el centro)

    ┌─────────────────────────────────┐
    │  Universo (U)                   │
    │                                 │
    │   ┌───────────┬────────┬─────┐  │
    │   │           │ [████] │     │  │
    │   │     A     │ A ∩ B  │  B  │  │
    │   │           │ [████] │     │  │
    │   └───────────┴────────┴─────┘  │
    │            ↑                    │
    │     Solo esta parte coloreada   │
    └─────────────────────────────────┘
```

### Ejemplo con Contexto Real

```
🎮 Videojuegos disponibles en plataformas:

A = {juegos en PlayStation}  = {FIFA, GTA, Minecraft, Fortnite, Valorant}
B = {juegos en Xbox}         = {FIFA, GTA, Halo, Forza, Minecraft}

A ∩ B = {FIFA, GTA, Minecraft}
        ↑ Juegos disponibles en AMBAS plataformas
```

### Diagrama de Venn

```
  ┌────────────────────────────────────────────────┐
  │ U = todos los videojuegos                      │
  │                                                │
  │  ┌─────────────┬─────────────┬──────────────┐  │
  │  │             │             │              │  │
  │  │  Fortnite   │    FIFA     │    Halo      │  │
  │  │  Valorant   │    GTA      │    Forza     │  │
  │  │             │  Minecraft  │              │  │
  │  │             │             │              │  │
  │  └─────────────┴─────────────┴──────────────┘  │
  │   ←── Solo A ──│←─ A ∩ B ──→│─── Solo B ──→    │
  └────────────────────────────────────────────────┘
```

### Conjuntos Disjuntos

Cuando dos conjuntos no comparten ningún elemento:

```
A ∩ B = ∅    ← Conjuntos disjuntos

Ejemplo:
A = {números pares}   = {2, 4, 6, 8...}
B = {números impares} = {1, 3, 5, 7...}

A ∩ B = ∅  (ningún número es par e impar a la vez)
```

```
    Diagrama de conjuntos disjuntos:

    ┌──────────────────────────────────────┐
    │ U                                    │
    │                                      │
    │   ┌──────────┐     ┌──────────┐      │
    │   │          │     │          │      │
    │   │    A     │     │    B     │      │
    │   │          │     │          │      │
    │   └──────────┘     └──────────┘      │
    │      (Los círculos NO se tocan)      │
    └──────────────────────────────────────┘
```

### ✏️ Practica Tú

En un grupo de 30 estudiantes se sabe que:
- 18 tienen cuenta en Instagram (conjunto I)
- 15 tienen cuenta en TikTok (conjunto T)
- 8 tienen cuenta en **ambas** redes

a) Representa la situación en un diagrama de Venn  
b) Halla I ∩ T  
c) ¿Cuántos estudiantes tienen Instagram pero **no** TikTok?  
d) ¿Cuántos estudiantes no tienen ninguna de las dos? *(Usa U = 30)*

---

## 5. 🔴 Diferencia de Conjuntos (A − B)

> **⏱️ Tiempo estimado: 17 minutos**

### Definición

La **diferencia** de A menos B es el conjunto de los elementos que **pertenecen a A pero NO pertenecen a B**.

```
A − B = {x | x ∈ A  y  x ∉ B}
```

> 🔑 **Clave:** A − B ≠ B − A  *(¡La diferencia NO es conmutativa!)*

### Representación Gráfica

```
       A − B                    B − A
  (lo de A sin B)           (lo de B sin A)

┌──────────────────┐    ┌──────────────────┐
│ U                │    │ U                │
│                  │    │                  │
│  ┌───┬───────┐   │    │  ┌───────┬───┐   │
│  │[█]│       │   │    │  │       │[█]│   │
│  │[█]│   B   │   │    │  │   A   │[█]│   │
│  │ A │       │   │    │  │       │[█]│   │
│  └───┴───────┘   │    │  └───────┴───┘   │
│  ↑ Solo esto     │    │         ↑ Solo   │
└──────────────────┘    └──────────────────┘
```

### Ejemplo Concreto

```
A = {1, 2, 3, 4, 5}
B = {3, 4, 5, 6, 7}

A − B = {1, 2}         ← Lo de A que NO está en B
B − A = {6, 7}         ← Lo de B que NO está en A
A ∩ B = {3, 4, 5}      ← Lo que comparten (excluido de ambas diferencias)
```

### Visualización Comparativa

```
              Universo U
┌──────────────────────────────────────────┐
│                                          │
│  ┌──────────────────────────────────┐    │
│  │         A              B         │    │
│  │  {1,2}  │   {3,4,5}   │  {6,7}  │    │
│  │         │             │         │    │
│  └─────────┴─────────────┴─────────┘    │
│     A−B         A∩B         B−A         │
└──────────────────────────────────────────┘
```

### Ejemplo de Vida Real

```
🎓 Materias:
A = {materias que aprobó Laura}  = {Matemáticas, Inglés, Historia, Arte}
B = {materias que aprobó Sofía}  = {Inglés, Historia, Biología, Química}

A − B = {Matemáticas, Arte}
→ Materias que aprobó Laura pero Sofía NO aprobó

B − A = {Biología, Química}
→ Materias que aprobó Sofía pero Laura NO aprobó
```

### ✏️ Practica Tú

Sea:
```
X = {letras de la palabra "COMPUTADORA"}
Y = {letras de la palabra "PROGRAMAR"}
```

a) Lista los elementos de X y de Y (sin repetir letras)  
b) Halla X − Y  
c) Halla Y − X  
d) Verifica que X − Y ≠ Y − X  
e) ¿Qué relación existe entre A − B, B − A y A ∩ B?

---

## 6. ⚫ Complemento de un Conjunto (Aᶜ)

> **⏱️ Tiempo estimado: 18 minutos**

### Definición

El **complemento** de A (respecto al universo U) es el conjunto de **todos los elementos del universo que NO pertenecen a A**.

```
Aᶜ = {x | x ∈ U  y  x ∉ A}
```

También se escribe como: **A'**, **Ā**, **~A**

> 🔑 **Recuerda:** El complemento siempre depende del **Universo** que definamos.

### Representación Gráfica

```
           Aᶜ  (todo lo sombreado fuera del círculo A)

    ┌──────────────────────────────────┐
    │ [██████████████████████████████] │
    │ [████]  ┌───────────┐  [███████] │
    │ [████]  │           │  [███████] │
    │ [████]  │     A     │  [███████] │
    │ [████]  │           │  [███████] │
    │ [████]  └───────────┘  [███████] │
    │ [██████████████████████████████] │
    └──────────────────────────────────┘
    [█] = Todo lo que NO es A = Aᶜ
```

### Ejemplo

```
U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {2, 4, 6, 8, 10}    (números pares)

Aᶜ = {1, 3, 5, 7, 9}   (números impares = los que no están en A)
```

### Propiedades del Complemento

| Propiedad | Expresión | Significado |
|-----------|-----------|-------------|
| Doble negación | (Aᶜ)ᶜ = A | Si negas dos veces, vuelves al original |
| Complemento del universo | Uᶜ = ∅ | Lo que no está en todo = nada |
| Complemento del vacío | ∅ᶜ = U | Lo que no está en nada = todo |
| Ley de Morgan 1 | (A ∪ B)ᶜ = Aᶜ ∩ Bᶜ | ¡Muy usada en programación! |
| Ley de Morgan 2 | (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ | ¡Muy usada en programación! |

### 🔗 Relación entre Complemento y Diferencia

```
Aᶜ = U − A

El complemento de A es la diferencia entre el universo y A.
¡Son la misma operación cuando B = U!
```

### Las Leyes de De Morgan (¡Muy Importante!)

```
Ley 1: (A ∪ B)ᶜ = Aᶜ ∩ Bᶜ
"El complemento de una unión es la intersección de los complementos"

Ley 2: (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ
"El complemento de una intersección es la unión de los complementos"
```

**Verificación con ejemplo:**

```
U = {1, 2, 3, 4, 5, 6, 7, 8}
A = {1, 2, 3, 4}
B = {3, 4, 5, 6}

A ∪ B = {1, 2, 3, 4, 5, 6}
(A ∪ B)ᶜ = {7, 8}           ← Lado izquierdo de la ley

Aᶜ = {5, 6, 7, 8}
Bᶜ = {1, 2, 7, 8}
Aᶜ ∩ Bᶜ = {7, 8}            ← Lado derecho de la ley

✅ ¡Son iguales! Se cumple la Primera Ley de De Morgan
```

### ✏️ Practica Tú

Sea:
```
U = {a, b, c, d, e, f, g, h}
A = {a, c, e, g}
B = {b, c, d, e}
```

a) Halla Aᶜ  
b) Halla Bᶜ  
c) Halla (A ∩ B)ᶜ  
d) Halla Aᶜ ∪ Bᶜ  
e) Verifica la Segunda Ley de De Morgan: ¿Se cumple que (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ?

---

## ⏸️ DESCANSO 1 — 15 Minutos

```
╔═══════════════════════════════════════════════════════════╗
║                                                           ║
║   🎉  ¡Buen trabajo!  Han completado 2 horas de sesión.   ║
║                                                           ║
║   ☕ Tómate 15 minutos para:                              ║
║                                                           ║
║   • Hidratarte y comer algo                               ║
║   • Levantarte y moverte un poco                          ║
║   • Descansar la vista de la pantalla o tablero           ║
║                                                           ║
║   🕐 Regresamos en 15 minutos para conectar todo          ║
║      esto con la PROGRAMACIÓN                             ║
║                                                           ║
╚═══════════════════════════════════════════════════════════╝
```

---

## 8. 💻 Conjuntos y Lógica en Programación

> **⏱️ Tiempo estimado: 30 minutos**

¡Bienvenidos de vuelta! Ahora viene la parte donde todo cobra sentido para el mundo digital.

### ¿Por Qué los Conjuntos son Importantes en Programación?

Cada vez que un programa **filtra, busca o combina datos**, está aplicando operaciones de conjuntos. Desde un buscador web hasta una app de música, todos usan esta lógica millones de veces por segundo.

### Tabla de Equivalencias: Conjuntos ↔ Programación

| Operación con conjuntos | Operador lógico | Palabra clave | Ejemplo en código |
|------------------------|-----------------|---------------|-------------------|
| Unión (A ∪ B) | OR / `||` | "O" | `if (esFan OR tieneBoleta)` |
| Intersección (A ∩ B) | AND / `&&` | "Y" | `if (esMayor AND tieneID)` |
| Complemento (Aᶜ) | NOT / `!` | "NO" | `if (!estaLogueado)` |
| Diferencia (A − B) | AND + NOT | "Y NO" | `if (enListaA AND !enListaB)` |

### Ejemplo 1: Sistema de Acceso a una Plataforma

Imagina que una plataforma online define estos conjuntos:

```
U  = {todos los usuarios registrados}
P  = {usuarios con suscripción Premium}
A  = {usuarios mayores de 18 años}
V  = {usuarios con cuenta verificada}
```

**¿Quiénes pueden acceder al contenido exclusivo?**
Solo aquellos que cumplan: **Premium Y verificados**

```
Conjunto que puede acceder = P ∩ V

Pseudocódigo:
─────────────────────────────────────────────────
SI (esPremium AND estaVerificado) ENTONCES
    mostrar_contenido_exclusivo()
SINO
    mostrar_contenido_basico()
FIN SI
─────────────────────────────────────────────────
```

### Ejemplo 2: Filtro de Búsqueda en una Tienda Online

```
U = {todo el catálogo de productos}
Z = {productos en zona de envío del usuario}
D = {productos con descuento activo}
S = {productos con stock disponible}
```

**Filtro: "con descuento, con envío y disponible"**

```
Resultado = D ∩ Z ∩ S

Pseudocódigo:
──────────────────────────────────────────────────────────
PARA CADA producto EN catalogo HACER
    SI (tieneDescuento AND hayEnvio AND hayStock) ENTONCES
        agregar_a_resultados(producto)
    FIN SI
FIN PARA
──────────────────────────────────────────────────────────
```

**Filtro: todo EXCEPTO los agotados**

```
Resultado = Sᶜ  (complemento de S)

Pseudocódigo:
──────────────────────────────────────
SI (NOT estaAgotado) ENTONCES
    mostrar(producto)
FIN SI
──────────────────────────────────────
```

### Ejemplo 3: Bases de Datos — Consultas SQL

Las bases de datos usan operaciones de conjuntos directamente con palabras reservadas:

```sql
-- UNION: todos los clientes de Colombia O México
SELECT nombre FROM clientes WHERE pais = 'Colombia'
UNION
SELECT nombre FROM clientes WHERE pais = 'México';

-- INTERSECT: estudiantes inscritos en Matemáticas Y en Física
SELECT id FROM inscritos WHERE materia = 'Matemáticas'
INTERSECT
SELECT id FROM inscritos WHERE materia = 'Física';

-- EXCEPT: clientes que compraron en enero pero NO en febrero
SELECT id FROM compras WHERE mes = 'Enero'
EXCEPT
SELECT id FROM compras WHERE mes = 'Febrero';
```

### Las Leyes de De Morgan en Código

```
Matemáticas:    (A ∪ B)ᶜ = Aᶜ ∩ Bᶜ
Programación:   !(A || B)  ===  !A && !B

Matemáticas:    (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ
Programación:   !(A && B)  ===  !A || !B
```

**Ejemplo práctico en JavaScript:**

```javascript
// Condición: el usuario NO puede entrar si NO es admin O está suspendido

// Forma original:
if ( !(esAdmin || estaSuspendido) ) { permitirAcceso(); }

// Aplicando De Morgan (equivalente y más legible):
if ( !esAdmin && !estaSuspendido ) { permitirAcceso(); }

// Ambas condiciones producen exactamente el mismo resultado
```

### 🧩 Actividad Mental Rápida

Relaciona cada situación con la operación de conjuntos correcta:

| Situación | Operación |
|-----------|-----------|
| Usuarios que tienen Netflix **O** HBO | |
| Canciones en tu playlist **Y** con más de 3 min | |
| Películas del catálogo que **NO** están en tu historial | |
| Amigos de Facebook que **NO** son tus seguidores en Instagram | |

> ✍️ Escribe la expresión simbólica para cada caso, definiendo primero tus conjuntos.

---

## 9. 👥 Trabajo Colaborativo en Equipos

> **⏱️ Tiempo estimado: 45 minutos**  
> **Organización:** Equipos de 3–4 personas

### Instrucciones Generales

Formen equipos de **3 a 4 personas** y asignen un rol a cada integrante:

| Rol | Responsabilidad |
|-----|----------------|
| 📐 Matemático/a | Plantea y resuelve los conjuntos simbólicamente |
| 🎨 Diseñador/a visual | Dibuja el diagrama de Venn |
| 💻 Programador/a | Traduce las operaciones a pseudocódigo o código |
| 🎤 Vocero/a | Presenta las conclusiones al grupo |

> Si el equipo es de 3 personas, uno asume dos roles.

---

### 🏆 MISIÓN 1: El Sistema de la Escuela (15 min)

**Contexto:** Tu colegio tiene una plataforma digital y necesita organizar la información de los estudiantes.

```
U = {todos los 40 estudiantes del grado 10°}

D = {estudiantes que entregaron el proyecto de Diseño}
    = {Ana, Beto, Carlos, Diana, Elena, Fausto, Gina, Héctor, Iris, Juan}

M = {estudiantes que entregaron el proyecto de Matemáticas}
    = {Beto, Diana, Fausto, Héctor, Juan, Karen, Luis, Marta, Nora, Oscar}

T = {estudiantes que entregaron ambos proyectos a tiempo}
    = {Beto, Diana, Fausto, Héctor, Juan}
```

**El equipo debe responder:**

a) Halla **D ∪ M** y explica qué representa en este contexto  
b) Halla **D ∩ M** y compara con T. ¿Qué observan?  
c) Halla **D − M**: ¿Qué estudiantes están en esta situación y qué significa?  
d) Halla **Dᶜ**: ¿Qué representa para el/la docente de Diseño?  
e) Si hay 40 estudiantes en total, ¿cuántos NO entregaron ningún proyecto? Muéstralo en el diagrama de Venn.  
f) **Reto programación:** Escribe el pseudocódigo que envíe aviso automático a los estudiantes que entregaron Diseño pero NO Matemáticas.

---

### 🏆 MISIÓN 2: La App de Streaming (15 min)

**Contexto:** Trabajan en el equipo de análisis de datos de una app de música.

```
U = {las 100 canciones más escuchadas este mes}

R = {canciones del género reggaetón}  →  n(R) = 35
P = {canciones del género pop}        →  n(P) = 40
E = {canciones en español}            →  n(E) = 55

Datos adicionales:
  R ∩ P = ∅  (ninguna canción es reggaetón Y pop a la vez)
  R ⊆ E      (todo el reggaetón está en español)
  n(P ∩ E) = 20
```

**El equipo debe responder:**

a) Dibuja un diagrama de Venn con los tres conjuntos  
b) ¿Cuántas canciones son pop en español?  
c) ¿Cuántas canciones de pop son en **otro idioma**?  
d) ¿Cuántas canciones no son ni reggaetón, ni pop?  
e) Halla n(R ∪ P ∪ E) paso a paso usando la fórmula de inclusión-exclusión  
f) **Reto programación:** Escribe las condiciones lógicas para filtrar:
   - Solo canciones en español que NO sean reggaetón
   - Canciones de pop O reggaetón, sin importar el idioma

---

### 🏆 MISIÓN 3: El Torneo de Videojuegos (Opcional — si terminan antes)

**Contexto:** Organizan un torneo estudiantil con tres categorías.

```
U = {80 estudiantes inscritos al torneo}

F = {participantes en Fútbol Virtual}   →  n(F) = 45
L = {participantes en LOL / MOBA}       →  n(L) = 38
B = {participantes en Battle Royale}    →  n(B) = 30

n(F ∩ L) = 15
n(F ∩ B) = 10
n(L ∩ B) = 12
n(F ∩ L ∩ B) = 5
```

**El equipo debe responder:**

a) Usando la fórmula de inclusión-exclusión, halla n(F ∪ L ∪ B):

```
n(F ∪ L ∪ B) = n(F) + n(L) + n(B) − n(F∩L) − n(F∩B) − n(L∩B) + n(F∩L∩B)
```

b) ¿Cuántos estudiantes NO participan en ninguna categoría?  
c) ¿Cuántos participan **solo** en Battle Royale?  
d) Dibuja el diagrama de Venn con tres conjuntos y ubica los valores en cada región  
e) **Reto programación:** ¿Cómo identificarías en código a alguien inscrito en los tres torneos?

---

### 📊 Socialización de Resultados

Cada equipo tendrá **3 minutos** para compartir:
- La respuesta que les resultó más difícil y cómo la resolvieron
- La solución de pseudocódigo que construyeron

---

## ⏸️ DESCANSO 2 — 15 Minutos

```
╔═══════════════════════════════════════════════════════════╗
║                                                           ║
║   ✨ ¡Excelente trabajo colaborativo!                     ║
║                                                           ║
║   ☕ 15 minutos de descanso bien merecidos.               ║
║                                                           ║
║   • Levántate y estírate                                  ║
║   • Hidratación y snack si tienes                         ║
║   • Comenta con tu equipo qué fue lo más interesante      ║
║                                                           ║
║   🎯 Al regresar: ejercicios individuales y reto final    ║
║                                                           ║
╚═══════════════════════════════════════════════════════════╝
```

> **Nota pedagógica:** Este segundo descanso se ubica después del trabajo colaborativo intenso y la socialización, cuando los estudiantes necesitan un momento de cierre antes del tramo final individual. Permite resetear cognitivamente y afrontar los ejercicios de aplicación con concentración renovada.

---

## 11. ✏️ Ejercicios de Aplicación Individual

> **⏱️ Tiempo estimado: 30 minutos**

Resuelve los siguientes ejercicios de forma **individual** en tu cuaderno. Muestra todos los procedimientos.

---

### 📝 Ejercicio 1 — Operaciones Básicas

Sea:
```
U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {1, 2, 3, 4, 6}
B = {2, 4, 6, 8, 10}
C = {1, 3, 5, 7, 9}
```

Calcula y dibuja el diagrama de Venn para cada caso:

| # | Operación | Resultado |
|---|-----------|-----------|
| a | A ∪ B | |
| b | A ∩ B | |
| c | A − B | |
| d | B − A | |
| e | Aᶜ | |
| f | (A ∪ B)ᶜ | |
| g | Aᶜ ∩ Bᶜ | |
| h | Verifica De Morgan comparando f y g | |

---

### 📝 Ejercicio 2 — Problema Contextualizado

En una encuesta a 50 jóvenes sobre hábitos de estudio:
- 28 usan YouTube para estudiar (conjunto Y)
- 22 usan podcasts para estudiar (conjunto P)
- 10 usan **ambos** recursos
- El resto no usa ninguno de los dos

a) Representa la situación en un diagrama de Venn  
b) Halla n(Y ∪ P)  
c) ¿Cuántos jóvenes usan **solo** YouTube?  
d) ¿Cuántos no usan ni YouTube ni podcasts?  
e) Halla Yᶜ y explica qué representa  
f) Verifica con la fórmula: n(Y ∪ P) = n(Y) + n(P) − n(Y ∩ P)

---

### 📝 Ejercicio 3 — Lógica y Conjuntos

Una biblioteca digital tiene:

```
U = {todos los libros de la biblioteca digital}
F = {libros de ficción}
E = {libros en español}
G = {libros gratuitos}
```

Describe con palabras qué conjunto representa cada expresión:

| Expresión | Descripción en palabras |
|-----------|------------------------|
| F ∩ E | |
| F ∪ G | |
| E − G | |
| (F ∩ G)ᶜ | |
| Fᶜ ∩ Eᶜ | |

Luego, escribe el **pseudocódigo** para filtrar los libros de ficción en español que sean gratuitos.

---

### 📝 Ejercicio 4 — Desafío: Leyes de De Morgan

Dado:
```
U = {a, b, c, d, e, f, g, h, i, j}
M = {a, b, c, d, e}
N = {c, d, e, f, g}
```

a) Calcula (M ∪ N)ᶜ  
b) Calcula Mᶜ ∩ Nᶜ  
c) ¿Se cumple la Primera Ley de De Morgan? Justifica  
d) Calcula (M ∩ N)ᶜ  
e) Calcula Mᶜ ∪ Nᶜ  
f) Verifica la Segunda Ley de De Morgan

---

## 12. 🏅 Reto Final: El Gran Desafío

> **⏱️ Opcional — Para quienes terminen antes**

### 🌐 Diseña tu Propio Sistema

Crea un sistema digital imaginario que use operaciones de conjuntos. Puede ser:
- Una app para organizar tareas escolares
- Un sistema de recomendación de series
- Una plataforma de torneos deportivos
- ¡Lo que se te ocurra!

**Debes:**

1. Definir el **conjunto universo** y al menos **3 conjuntos** relevantes para tu app
2. Describir qué representa cada conjunto
3. Plantear **3 situaciones o consultas** que un usuario podría hacer
4. Resolver cada situación usando operaciones de conjuntos
5. Escribir el **pseudocódigo** para al menos una de las consultas
6. Dibujar el **diagrama de Venn** correspondiente

> 💡 **Dato:** Los mejores sistemas digitales del mundo (Netflix, Spotify, Google) aplican estas operaciones millones de veces por segundo para mostrarte exactamente lo que quieres ver.

---

## 13. 🎯 Resumen y Cierre

> **⏱️ Tiempo estimado: 15 minutos**

### Mapa Conceptual de las Operaciones

```
                    ┌─────────────────────┐
                    │  OPERACIONES CON    │
                    │     CONJUNTOS       │
                    └──────────┬──────────┘
                               │
          ┌──────────┬─────────┼──────────┬──────────┐
          ▼          ▼         ▼          ▼          ▼
    ┌──────────┐ ┌────────┐ ┌───────┐ ┌────────┐ ┌──────────┐
    │  UNIÓN   │ │INTERSE.│ │DIFER. │ │COMPLE. │ │De Morgan │
    │  A ∪ B   │ │ A ∩ B  │ │ A−B   │ │  Aᶜ    │ │  Leyes   │
    │          │ │        │ │       │ │        │ │          │
    │  OR / || │ │AND / &&│ │AND+NOT│ │ NOT/!  │ │!(A||B)=  │
    │          │ │        │ │       │ │        │ │ !A && !B │
    └──────────┘ └────────┘ └───────┘ └────────┘ └──────────┘
```

### Tabla Resumen

| Operación | Símbolo | Lógica | Descripción |
|-----------|---------|--------|-------------|
| Unión | A ∪ B | A OR B | Todo lo de A, B o ambos |
| Intersección | A ∩ B | A AND B | Solo lo que está en A Y en B |
| Diferencia | A − B | A AND NOT B | Lo de A que no está en B |
| Complemento | Aᶜ | NOT A | Todo lo del universo que no es A |

### ✅ Lista de Verificación de Aprendizaje

Marca con honestidad cada ítem que puedas hacer con confianza:

- [ ] Puedo listar los elementos de la unión de dos conjuntos sin repetir
- [ ] Puedo identificar correctamente los elementos de la intersección
- [ ] Puedo calcular A − B y B − A y entender por qué son diferentes
- [ ] Sé calcular el complemento dado un universo específico
- [ ] Conozco y puedo verificar las Leyes de De Morgan
- [ ] Sé dibujar diagramas de Venn para dos o tres conjuntos
- [ ] Puedo relacionar las operaciones con operadores lógicos en código
- [ ] Puedo escribir pseudocódigo con condiciones basadas en conjuntos

### 🗣️ Reflexión Final

Responde en tu cuaderno (3–4 oraciones):

> *¿En qué aspecto de tu vida diaria o en qué tecnología que uses regularmente crees que se aplican las operaciones con conjuntos? ¿Por qué crees que los programadores necesitan dominar estas operaciones?*

---

## 📖 Glosario

| Término | Definición |
|---------|------------|
| **Conjunto** | Colección bien definida de elementos distintos |
| **Elemento** | Cada objeto que pertenece a un conjunto |
| **Universo (U)** | El conjunto de todos los elementos posibles en un contexto dado |
| **Conjunto vacío (∅)** | El conjunto que no tiene ningún elemento |
| **Cardinalidad** | Número de elementos de un conjunto. Se denota n(A) |
| **Subconjunto** | A ⊆ B si todo elemento de A también está en B |
| **Diagrama de Venn** | Representación gráfica de conjuntos usando regiones ovales |
| **Unión** | A ∪ B: elementos en A, en B o en ambos |
| **Intersección** | A ∩ B: elementos en A y en B simultáneamente |
| **Diferencia** | A − B: elementos en A que no están en B |
| **Complemento** | Aᶜ: elementos del universo que no están en A |
| **Conjuntos disjuntos** | Dos conjuntos cuya intersección es vacía |
| **Operador lógico** | Símbolo (AND, OR, NOT) que combina condiciones en programación |
| **Pseudocódigo** | Descripción textual de un algoritmo usando lenguaje natural estructurado |

---

## 📚 Referencias y Recursos Adicionales

### Para Profundizar

- 📺 **YouTube:** Busca "Operaciones con conjuntos - Khan Academy en Español"
- 🌐 **GeoGebra:** Permite crear diagramas de Venn interactivos → [geogebra.org](https://www.geogebra.org)
- 📖 **Libro:** Matemáticas Discretas — Capítulo de Teoría de Conjuntos (cualquier edición de grado 10°)

### Conjuntos en Python (para explorar en casa 🐍)

Python tiene un tipo de dato nativo llamado `set` que implementa todas estas operaciones:

```python
A = {1, 2, 3, 4, 5}
B = {3, 4, 5, 6, 7}

print(A | B)   # Unión       → {1, 2, 3, 4, 5, 6, 7}
print(A & B)   # Intersección → {3, 4, 5}
print(A - B)   # Diferencia  → {1, 2}
print(A ^ B)   # Dif. simétrica → {1, 2, 6, 7}

# Verificando De Morgan:
U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
Ac = U - A
Bc = U - B
print((A | B) == U - (Ac & Bc))  # True ✅
```

> Puedes probarlo gratis en [replit.com](https://replit.com) o [python.org/shell](https://www.python.org/shell/)

---

## 🎓 Criterios de Evaluación

| Criterio | Indicador | Peso |
|----------|-----------|------|
| **Conceptual** | Identifica y define correctamente cada operación | 20% |
| **Procedimental** | Aplica las operaciones para obtener resultados correctos | 35% |
| **Representación** | Usa correctamente diagramas de Venn y notación simbólica | 20% |
| **Conexión TIC** | Relaciona las operaciones con condiciones lógicas en código | 15% |
| **Trabajo en equipo** | Participa activamente y aporta al equipo | 10% |

---

> 📝 **Nota para el/la docente:** Este material puede adaptarse para trabajo asincrónico o virtual. Se recomienda que el trabajo colaborativo (sección 9) sea supervisado en tiempo real para garantizar el diálogo matemático entre pares. Las misiones pueden asignarse de forma diferenciada según el nivel del grupo. El reto final (sección 12) es ideal como tarea de extensión o evaluación alternativa.

---

*Material elaborado con fines educativos. Diseñado bajo principios de aprendizaje activo y pensamiento computacional.*  
*Licencia: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)*

---
*Versión 1.0 — Marzo 2026*
