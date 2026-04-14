# Introducción a la Programación y el Pensamiento Algorítmico

## Guía del Docente — Clase Inaugural

**Duración:** 3 horas (180 minutos)
**Población:** Estudiantes de 15-16 años (10º grado)
**Modalidad:** Presencial con actividades prácticas y colaborativas

---

## Parte 1: Bienvenida e Introducción a la Asignatura (30 minutos)

### 1.1 El Mundo que Nos Rodea

Cada día, miles de millones de dispositivos ejecutan instrucciones invisibles que hacen funcionar nuestro mundo: el teléfono que desbloqueas con tu huella digital, el aplicativo que te muestra el estado de tus notas, el sistema que determina qué video aparece primero en tu feed. Todo esto funciona porque alguien, en algún momento, diseñó una serie de pasos precisos para que una máquina los ejecutara.

Esa es, en esencia, la misión de esta asignatura: aprender a **hablar con la máquina** en su idioma, pero no como algo ajeno o técnico, sino como una extensión natural del pensamiento humano. No se trata simplemente de "aprender a programar". Se trata de desarrollar una forma de pensar — **estructurada, lógica y creativa** — que te servirá no solo frente al computador, sino en prácticamente cualquier situación de tu vida.

> **Reflexión:** Cuando descubres que puedes darle instrucciones claras a una máquina para que resuelva problemas por ti, empiezas a verte a ti mismo como alguien con poder de crear, no solo de consumir tecnología.

### 1.2 ¿Qué vamos a aprender?

Durante este curso abordaremos:

| Unidad | Descripción |
|--------|-------------|
| **Fundamentos del pensamiento algorítmico** | Cómo plantear soluciones como secuencias de pasos |
| **Entrada, proceso y salida** | La lógica fundamental de toda computación |
| **Tipos de datos** | Números, textos, decisiones y repeticiones |
| **Estructuras de control** | Condiciones y ciclos |
| **Funciones y modularización** | Organizar soluciones en piezas reutilizables |
| **Proyecto integrador** | Aplicar todo lo aprendido a un problema real |

### 1.3 ¿Por qué es importante el pensamiento algorítmico?

No necesitas ser "bueno en matemáticas" para programar. Lo que necesitas es:

- **Paciencia** para analizar un problema paso a paso
- **Curiosidad** por entender cómo funcionan las cosas
- **Creatividad** para encontrar soluciones diferentes
- **Rigocidad** para verificar que tu solución realmente funciona

Estas habilidades se desarrollan con la práctica, y esta clase es el primer paso.

---

## Parte 2: Pensamiento Algorítmico — ¿Qué es un Algoritmo? (40 minutos)

### 2.1 Definición Informal

Un **algoritmo** es una **secuencia finita y ordenada de pasos** que permiten resolver un problema o alcanzar un objetivo.

La palabra "algoritmo" proviene del nombre del matemático persa **Al-Khwarizmi** (siglo IX), quien escribió sobre métodos para realizar cálculos. Sin embargo, los algoritmos existen mucho antes de las computadoras — existen desde que el ser humano necesita resolver problemas de manera sistemática.

### 2.2 Algoritmos en la Vida Cotidiana

Los algoritmos no son únicamente procesos que ejecutan los computadores. Los ejecutamos nosotros constantemente, a veces sin darnos cuenta.

**Ejemplo 1: Receta de cocina**

```
1. Sacar los ingredientes del refrigerador
2. Medir 2 tazas de harina
3. Agregar 1 cucharadita de sal
4. Mezclar los ingredientes secos
5. Agregar 1 huevo y 1 taza de leche
6. Revolver hasta obtener una mezcla homogénea
7. Calentar el sartén a fuego medio
8. Verter 1/4 taza de mezcla por cada panqueque
9. Cocinar 2 minutos por lado
10. Servir caliente
```

**Ejemplo 2: Buscar un libro en la biblioteca**

```
1. Ir a la sección de Biblioteca General
2. Identificar la primera letra del título del libro
3. Dirigirse al estante correspondiente (A, B, C, ...)
4. Buscar el libro en orden numérico
5. Verificar que el título coincide
6. Si lo encuentras, tomarlo; si no, pedir ayuda al bibliotecario
```

**Ejemplo 3: Vestirse según el clima**

```
1. Mirar por la ventana o consultar el clima
2. Si la temperatura es menor a 15°C:
   a. Tomar una chaqueta
   b. Ponerse jeans y no shorts
3. Si la temperatura es mayor o igual a 15°C:
   a. No tomar chaqueta
   b. Puede usarse shorts o ropa ligera
4. Listo para salir
```

### 2.3 Características de un Algoritmo

Todo algoritmo debe cumplir las siguientes propiedades:

| Propiedad | Significado |
|-----------|-------------|
| **Finitud** | El algoritmo debe terminar después de un número finito de pasos |
| **Claridad** | Cada paso debe estar definido sin ambigüedad |
| **Entrada** | Puede tener cero o más datos de entrada |
| **Salida** | Produce al menos un resultado |
| **Efectividad** | Los pasos deben poder ejecutarse en un tiempo razonable |

> **Analogía:** Imagina que le das instrucciones a un robot muy literal que no puede adivinar nada. Si le dices "ve a la cocina y tráeme algo de tomar", probablemente te traiga un vaso con agua. Pero si le dices "ve a la cocina, abre el refrigerador, saca el jugo de naranja y sírvelo en el vaso azul que está en el estante superior", el resultado será exactamente lo que esperas. Los algoritmos son instrucciones así de precisas.

### 2.4 Actividad 1: Conversatorio Inicial (15 minutos)

---

## 🎤 Actividad: Conversatorio Inicial — "¿Qué es un Algoritmo?"

### Objetivo
Explorar las ideas previas de los estudiantes sobre algoritmos y establecer conexiones con su vida diaria.

### Dinámica

El docente moderará una conversación grupal. Se sugieren las siguientes preguntas:

1. **Pregunta inicial:** "Sin buscar en internet, ¿alguien puede decir qué significa la palabra 'algoritmo'?"

   *Escuchar respuestas y anotarlas en el tablero sin corregir. Luego contrastar con la definición formal.*

2. **Profundización:** "¿Dónde han escuchado esta palabra antes? ¿En qué contexto?"

   *Celulares, redes sociales, videos de tecnología — explorar las conexiones que los estudiantes hacen.*

3. **Conexión personal:** "¿Alguna vez han seguido pasos para hacer algo? ¿Recuerdan algún ejemplo?"

   *Guiar para que surjan ejemplos de su cotidianidad: recetas, instrucciones de ensamblaje, juegos de mesa, etc.*

4. **El teléfono inteligente:** "¿Creen que su celular usa algoritmos? ¿Para qué?"

   *Abrir la discusión hacia cómo los algoritmos están presentes en tecnologías que usan diariamente.*

### Instrucciones para el docente

- **No corregir** durante la primera ronda de respuestas. El objetivo es que aflore el conocimiento previo.
- **Validar** todas las respuestas con frases como: "Muy interesante", "Eso tiene conexión con lo que veremos".
- **Guiar** con preguntas adicionales si la conversación se estanca: "¿Y qué pasa después de ese paso?"
- **Registrar** las ideas principales en el tablero o en un documento compartido para volver a ellas al final de la clase.

### Cierre del conversatorio (3 minutos)

Sintetizar las ideas principales y hacer notar que:

- Ya utilizan algoritmos sin saberlo
- Un algoritmo no requiere tecnología, solo un método claro
- Las computadoras funcionan ejecutando algoritmos diseñados por personas

---

## Parte 3: Resolución de Problemas con el Computador (35 minutos)

### 3.1 El Ciclo de Solución Algorítmica

Cuando queremos usar el computador para resolver un problema, seguimos un proceso que tiene etapas claramente definidas. Este ciclo es fundamental y lo usaremos durante todo el curso.

```
        ┌─────────────────────────┐
        │   ANÁLISIS DEL          │
        │      PROBLEMA           │
        └──────────┬──────────────┘
                   │
                   ▼
        ┌─────────────────────────┐
        │    DISEÑO DEL           │
        │      ALGORITMO          │
        └──────────┬──────────────┘
                   │
                   ▼
        ┌─────────────────────────┐
        │   CODIFICACIÓN          │
        │   (Programación)        │
        └──────────┬──────────────┘
                   │
                   ▼
        ┌─────────────────────────┐
        │   PRUEBAS Y              │
        │   VALIDACIÓN            │
        └──────────┬──────────────┘
                   │
                   ▼
        ┌─────────────────────────┐
        │   CORRECCIÓN Y          │
        │     MEJORA              │
        └─────────────────────────┘
```

Veamos cada etapa en detalle:

### 3.2 Entrada (Input)

La **entrada** son todos los datos que el algoritmo necesita para trabajar. Piensa en ella como la materia prima.

**Ejemplos de entradas:**

- En una calculadora: los números que introduces (ej: 5 y 3)
- En un sistema de login: el usuario y la contraseña
- En un juego de adivinar: el número secreto y los intentos del jugador

**Preguntas clave para identificar la entrada:**

- ¿Qué información me dan antes de comenzar?
- ¿Qué datos necesito para resolver el problema?
- ¿Hay valores que el usuario debe proporcionarme?

### 3.3 Proceso

El **proceso** es el conjunto de operaciones que transforman las entradas en salidas. Es el "cerebro" del algoritmo.

**Ejemplos de procesos:**

- Calcular el área de un rectángulo: `ancho × alto`
- Validar credenciales: comparar lo ingresado con lo almacenado
- Determinar si un número es par: verificar si el residuo de dividir entre 2 es cero

### 3.4 Salida (Output)

La **salida** es el resultado final que el algoritmo produce. Es lo que el usuario recibe después de que el proceso se ejecuta.

**Ejemplos de salidas:**

- En una calculadora: el resultado de la operación (ej: 15)
- En un sistema de login: "Bienvenido" o "Credenciales incorrectas"
- En un juego: el mensaje de victoria o derrota

### 3.5 Ejemplo Integrado: Calculadora de Índice de Masa Corporal (IMC)

```
ENTRADA:
- Peso de la persona (en kilogramos)
- Altura de la persona (en metros)

PROCESO:
1. Multiplicar la altura por sí misma (calcular altura²)
2. Dividir el peso entre el resultado anterior
3. Redondear el resultado a 2 decimales

SALIDA:
- El valor del IMC (por ejemplo: 22.5)
```

### 3.6 Ejemplo Guiado: El Despertador

Antes de que intenten resolver los problemas, veamos juntos cómo se hace con un ejemplo completo.

**Problema:** María quiere preparar un vaso de café. Ella tiene café instantáneo, azúcar, una taza, una cuchara y agua caliente.

```
ENTRADA:
- Café instantáneo (cucharadas)
- Azúcar (cucharadas)
- Agua caliente (mililitros)
- Taza vacía

PROCESO:
1. Verter 2 cucharadas de café en la taza
2. Agregar 1 cucharada de azúcar
3. Verter 200 ml de agua caliente
4. Revolver con la cuchara hasta que todo se disuelva

SALIDA:
- Una taza de café listo para beber
```

---

### 3.7 Ejemplo Guiado: Calculadora de Cambio

**Problema:** Un cajero debe calcular el cambio cuando alguien compra algo.

```
ENTRADA:
- Precio del producto (número decimal)
- Dinero entregado por el cliente (número decimal)

PROCESO:
1. Restar el precio del producto al dinero entregado
2. El resultado es el cambio que debe darsele al cliente

SALIDA:
- La cantidad de dinero que se debe devolver (número decimal)
```

---

### 3.8 Actividad 2: Taller Diagnóstico (20 minutos)

---

## 🔍 Actividad: Taller Diagnóstico — Resolución de Problemas Cotidianos

### Objetivo
Identificar cómo los estudiantes abordan problemas cotidianos y comenzar a formalizar su pensamiento en términos de entrada-proceso-salida.

### Materiales

- Hojas de trabajo (una por estudiante)
- Lápices y borradores

### Instrucciones

El docente repartirá la siguiente hoja de trabajo. Los estudiantes deben completarla individualmente (10 minutos) y luego compartir sus respuestas en parejas (5 minutos). Las mejores soluciones se compartirán con toda la clase (5 minutos).

---

### HOJA DE TRABAJO — Problema A: El Bus Escolar

**Contexto:** Cada mañana, Carlos debe tomar el bus escolar a las 7:00 AM. Vive a 15 minutos caminando de la parada. Se despierta a las 6:30 AM.

**Tu tarea:** Diseña los pasos que Carlos debe seguir cada mañana para llegar a tiempo al school.

**Importante:** Considera qué información conoce Carlos antes de actuar (ENTRADA), qué decisiones debe tomar (PROCESO) y qué resultado busca (SALIDA).

```
ENTRADA (¿Qué sabe Carlos antes de actuar?):
1. _____________________________________________
2. _____________________________________________
3. _____________________________________________

PROCESO (¿Qué pasos debe seguir Carlos?):
Paso 1: _______________________________________
Paso 2: _______________________________________
Paso 3: _______________________________________
Paso 4: _______________________________________
Paso 5: _______________________________________

SALIDA (¿Cuál es el resultado esperado?):
_______________________________________________
```

---

### HOJA DE TRABAJO — Problema B: Organizar la Mochila

**Contexto:** Luisa tiene que preparar su mochila para el día siguiente. Tiene 5 cuadernos, 3 lápices, 1 libreta, la computadora y el cargador.

**Tu tarea:** Diseña los pasos para que Luisa prepare su mochila correctamente.

```
ENTRADA (¿Qué tiene Luisa al inicio?):
_____________________________________________

PROCESO:
Paso 1: _______________________________________
Paso 2: _______________________________________
Paso 3: _______________________________________
Paso 4: _______________________________________
Paso 5: _______________________________________

SALIDA (¿Cómo debe quedar la mochila al final?):
_______________________________________________
```

---

### HOJA DE TRABAJO — Problema C (Desafío): Tu Propio Ejemplo

**Tu tarea:** Piensa en una actividad que realizas regularmente (vestirte, preparar un snack, hacer una llamada). Identifica la entrada, el proceso y la salida.

```
ACTIVIDAD: ___________________________________

ENTRADA:
_____________________________________________

PROCESO:
1. ___________________________________________
2. ___________________________________________
3. ___________________________________________

SALIDA:
_____________________________________________
```

---

### Reflexión posterior al taller

Después de que los estudiantes completen la actividad, el docente guiará una discusión:

- ¿Pudieron identificar claramente las entradas y salidas?
- ¿Hay pasos que podrían ejecutarse en orden diferente?
- ¿Hay pasos que son repetitivos?
- ¿Qué pasaría si omitieran algún paso?

---

## Parte 4: Tipos de Datos Fundamentales (30 minutos)

### 4.1 ¿Por qué importan los tipos de datos?

Cuando programamos, el computador necesita saber qué tipo de información estamos manejando para saber cómo procesarla. No es lo mismo sumar dos números (2 + 3 = 5) que concatenar dos textos ("Hola" + " mundo" = "Hola mundo"). Por eso existen los **tipos de datos**.

### 4.2 Los Tipos Básicos

#### 4.2.1 Numéricos

**Enteros (int):** Representan números sin parte decimal.

| Ejemplo | Descripción |
|---------|-------------|
| `42` | La respuesta a todo |
| `-7` | Un número negativo |
| `0` | El valor neutro |
| `1000000` | Un millón |

*Usos:* Contar objetos, representar edades, contar días, realizar operaciones matemáticas.

**Decimales (float):** Representan números con parte decimal.

| Ejemplo | Descripción |
|---------|-------------|
| `3.14159` | El número Pi |
| `1.75` | Una estatura en metros |
| `99.9` | Una calificación |
| `0.0` | Valor inicial |

*Usos:* Precios, medidas, calificaciones con decimales, coordenadas.

> **Dato curioso:** En programación, se usa punto (`.`) y no coma para separar la parte decimal: `3.5` no `3,5`.

#### 4.2.2 Texto (Cadenas / String)

Las cadenas de texto (llamadas *strings*) son secuencias de caracteres enclosed entre comillas.

| Ejemplo | Descripción |
|---------|-------------|
| `"Hola"` | Una palabra |
| `"Buenos días"` | Una frase |
| `"123"` | ¡Esto no es un número! Son caracteres |
| `""` | Una cadena vacía |

*Usos:* Nombres, mensajes, direcciones de correo, códigos.

#### 4.2.3 Lógicos (Booleanos)

Los datos booleanos solo pueden tener dos valores: **Verdadero** o **Falso**. Son fundamentales para las decisiones.

| Ejemplo | Significado |
|---------|-------------|
| `True` | Una condición se cumple |
| `False` | Una condición no se cumple |

*Usos:* ¿El usuario está registrado? ¿La contraseña es correcta? ¿El número es mayor que cero?

#### 4.2.4 Sin Valor (Null / None)

A veces algo existe pero no tiene un valor todavía. Esto se representa con `null` o `None` (en Python).

| Ejemplo | Significado |
|---------|-------------|
| `None` | Sin valor asignado |
| `null` | Valor vacío intencional |

*Usos:* Espacios pendientes de completar, respuestas opcionales.

### 4.3 Tabla Resumen de Tipos de Datos

| Tipo | Ejemplos | ¿Qué puedes hacer con él? |
|------|----------|---------------------------|
| **Entero (int)** | `42`, `-7`, `0` | Sumar, restar, multiplicar, comparar |
| **Decimal (float)** | `3.14`, `1.5`, `99.9` | Operaciones matemáticas precisas |
| **Cadena (str)** | `"Hola"`, `"Ana"` | Unir textos, buscar palabras |
| **Booleano (bool)** | `True`, `False` | Evaluar condiciones |
| **Null** | `None`, `null` | Representar ausencia de dato |

### 4.4 Visualizando la importancia de los tipos

```
ENTRADA:  "Juan" (string)     +  "Pérez" (string)  →  "Juan Pérez" (string)
ENTRADA:  5 (int)             +  3 (int)           →  8 (int)
ENTRADA:  "5" (string)         +  "3" (string)       →  "53" (string)  ⚠️
```

> **¡Cuidado!** "5" + "3" no es 8, es "53" porque son textos, no números. El computador hace lo que le dices, no lo que quieres. Por eso es importante usar los tipos correctos.

### 4.5 Ejemplos Guiados con Tipos de Datos

Antes de los ejercicios, veamos cómo los tipos de datos aparecen en problemas reales:

**Ejemplo 1: Sistema de login**

```
ENTRADA:
- Nombre de usuario: "maria_gomez" → Tipo: string
- Contraseña ingresada: "abc123" → Tipo: string

PROCESO:
Comparar lo ingresado con los datos almacenados

SALIDA:
- "Bienvenido" → Tipo: string
- Boolean: True (si es correcto) o False (si es incorrecto)
```

**Ejemplo 2: Calculadora de descuento**

```
ENTRADA:
- Precio original: 150000 → Tipo: int
- Porcentaje de descuento: 10 → Tipo: int

PROCESO:
1. Multiplicar 150000 × 10 y dividir entre 100
2. Restar el resultado del precio original

SALIDA:
- Precio final: 135000 → Tipo: int
```

**Ejemplo 3: Verificador de mayoría de edad**

```
ENTRADA:
- Edad de la persona: 16 → Tipo: int

PROCESO:
Verificar si la edad es mayor o igual a 18

SALIDA:
- Resultado: False → Tipo: boolean (no es mayor de edad)
```

---

## Parte 5: Presentación Gráfica del Ciclo de Solución (25 minutos)

### 5.1 Actividad 3: Presentación Gráfica (20 minutos + 5 minutos de cierre)

---

## 🎨 Actividad: Presentación Gráfica del Ciclo de Solución Algorítmica

### Objetivo
Crear una representación visual del ciclo de solución algorítmica usando los conceptos de entrada-proceso-salida y tipos de datos.

### Modalidad
Trabajo en grupos de 3-4 estudiantes.

### Materiales

- Hojas de cuaderno o impresas (una por grupo)
- Lápices y colores
- Plantilla impresa (opcional:也可以 dibujar el diagrama a mano)

### Instrucciones

El docente entrega a cada grupo la plantilla siguiente (o los estudiantes la dibujan en su cuaderno) y deben:

1. **Completar** los espacios en blanco con un problema asignado
2. **Ilustrar** cada etapa con un dibujo simple (pueden usar círculos y flechas)
3. **Agregar** flechas para mostrar el flujo
4. **Incluir** un ejemplo de tipo de dato para cada entrada y salida
5. **Preparar** una explicación de 2 minutos para explicar su diagrama

---

```
╔══════════════════════════════════════════════════════════════════╗
║          CICLO DE SOLUCIÓN ALGORÍTMICA (en tu cuaderno)          ║
╠══════════════════════════════════════════════════════════════════╣
║                                                                  ║
║  ┌──────────────────────────────────────────────────────────┐    ║
║  │  ENTRADA (INPUT)                                         │    ║
║  │  Nombre: _______________                                 │    ║
║  │  Tipo de dato: _______________                           │    ║
║  └────────────────────────────┬─────────────────────────────┘    ║
║                               │                                   ║
║                               ▼                                   ║
║  ┌──────────────────────────────────────────────────────────┐    ║
║  │  PROCESO                                                │    ║
║  │  Paso 1: _______________                                │    ║
║  │  Paso 2: _______________                                │    ║
║  │  Paso 3: _______________                                │    ║
║  └────────────────────────────┬─────────────────────────────┘    ║
║                               │                                   ║
║                               ▼                                   ║
║  ┌──────────────────────────────────────────────────────────┐    ║
║  │  SALIDA (OUTPUT)                                        │    ║
║  │  Nombre: _______________                                │    ║
║  │  Tipo de dato: _______________                          │    ║
║  └──────────────────────────────────────────────────────────┘    ║
║                                                                  ║
║  Problema asignado: ________________________________________     ║
╚══════════════════════════════════════════════════════════════════╝
```

---

### Problemas para asignar a cada grupo

**Grupo 1:** Sistema de login simple
- Un usuario ingresa su contraseña y el sistema verifica si es correcta.

**Grupo 2:** Calculadora de promedio
- Un estudiante ingresa 3 calificaciones y el sistema calcula el promedio.

**Grupo 3:** Conversor de temperatura
- El usuario ingresa una temperatura en Celsius y el sistema la convierte a Fahrenheit.

**Grupo 4:** Validador de edad
- El usuario ingresa su edad y el sistema determina si puede votar (18+).

**Grupo 5:** Calculadora de descuento
- El usuario ingresa el precio de un producto y el sistema aplica un 10% de descuento.

### Presentación de grupos

Cada grupo tiene 2 minutos para:

1. Explicar el problema asignado
2. Mostrar cómo identificaron las entradas y salidas
3. Describir los tipos de datos usados
4. Explicar el flujo del proceso

### Cierre de la actividad

El docente destaca los puntos en común entre todos los grupos:

- Todos tienen entradas claras
- Todos tienen un proceso que transforma los datos
- Todos producen una salida significativa
- Todos requieren elegir los tipos de datos correctos

---

## Parte 6: Síntesis y Cierre de la Clase (15 minutos)

### 6.1 Resumen de lo Aprendido

Repasemos los conceptos clave de hoy:

```
╔═══════════════════════════════════════════════════════════════════╗
║                     MENSAJES CLAVE DE HOY                        ║
╠═══════════════════════════════════════════════════════════════════╣
║                                                                   ║
║  1. Un algoritmo es una secuencia de pasos para resolver          ║
║     un problema — ya existe en tu vida diaria.                    ║
║                                                                   ║
║  2. La solución algorítica sigue un ciclo:                        ║
║     ANALIZAR → DISEÑAR → CODIFICAR → PROBAR → CORREGIR            ║
║                                                                   ║
║  3. Todo algoritmo trabaja con ENTRADA, PROCESO y SALIDA.         ║
║     Sin entrada no hay procesamiento; sin procesamiento           ║
║     no hay resultado.                                             ║
║                                                                   ║
║  4. Los tipos de datos importan: números, textos, booleanos       ║
║     y valores nulos. El computador hace lo que le dices,          ║
║     no lo que quieres — por eso hay que ser precisos.             ║
║                                                                   ║
║  5. El pensamiento algorítmico no es solo para programadores.     ║
║     Es una forma de razonar que te ayuda en cualquier situación.   ║
║                                                                   ║
╚═══════════════════════════════════════════════════════════════════╝
```

### 6.2 Reflexión Final

La próxima clase empezaremos a traducir estos pasos a código real. Pero hoy lo más importante es que reconozcan que **ya piensan algorítmicamente** — lo han hecho toda la vida sin darle un nombre.

El verdadero desafío no es aprender la sintaxis de un lenguaje de programación. El verdadero desafío es:

- **Analizar** un problema para entenderlo completamente
- **Dividirlo** en pasos manejables
- **Identificar** qué datos necesitas y qué resultados esperas
- **Verificar** que tu solución realmente funciona

Eso es lo que aprenderemos a hacer juntos.

### 6.3 Tarea para la próxima clase (opcional)

Escribe en una hoja los pasos de una actividad que hagas regularmente (cualquiera). Intenta identificar:

- Las entradas (¿qué necesitas antes de empezar?)
- El proceso (¿qué pasos sigues?)
- Las salidas (¿qué resulta al final?)

Trae tu respuesta a la próxima clase — la usaremos como base para nuestra primera actividad práctica de programación.

---

## Anexos

### Anexo A: Distribución Sugerida del Tiempo

| Actividad | Tiempo |
|-----------|--------|
| Parte 1: Bienvenida e introducción | 30 min |
| Parte 2: Pensamiento algorítmico + Conversatorio | 40 min |
| Parte 3: Resolución de problemas (Entrada-Proceso-Salida) | 35 min |
| Parte 4: Tipos de datos | 30 min |
| Parte 5: Presentación gráfica del ciclo | 25 min |
| Parte 6: Síntesis y cierre | 15 min |
| **Tiempo Total** | **180 min** |

### Anexo B: Materiales Necesarios

- Hojas de trabajo impresas (una por estudiante)
- Cuadernos para actividad grupal
- Lápices, colores y borradores
- Proyector o tablero
- Marcadores para tablero

### Anexo C: Criterios de Evaluación Formativa

| Criterio | Nivel Inicial | Nivel en Desarrollo | Nivel Logrado |
|----------|---------------|---------------------|---------------|
| Identifica entradas y salidas en un problema | Necesita ayuda | Identifica algunas | Identifica todas con claridad |
| Comprende el concepto de algoritmo | Confunde con "fórmula" | Entiende parcialmente | Entiende y da ejemplos propios |
| Reconoce tipos de datos básicos | No los diferencia | Reconoce algunos | Clasifica correctamente |
| Colabora en actividades grupales | Participa pasivamente | Aporta algunas ideas | Lidera y contribuye activamente |

---

*Material elaborado para uso educativo — Clase inaugural de Introducción a la Programación*
*Adaptado para estudiantes de 10º grado (15-16 años)*