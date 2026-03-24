# Álgebra Proposicional

## Material de Estudio para Estudiantes

---

## 📋 Información del Curso

| Aspecto | Detalle |
|---------|---------|
| **Nivel educativo** | Décimo grado (15-16 años) |
| **Duración total** | 4 horas (240 minutos) |
| **Descansos** | 2 de 15 minutos (minuto 120 y minuto 180) |
| **Área** | Lógica y Matemáticas |

---

## 🎯 Objetivos de Aprendizaje

Al finalizar esta unidad, serás capaz de:

1. **Identificar** proposiciones simples y compuestas en contextos cotidianos
2. **Construir** tablas de verdad para operaciones lógicas básicas
3. **Aplicar** los conectivos lógicos (conjunción, disyunción, negación) en la resolución de problemas
4. **Evaluar** la veracidad de proposiciones compuestas mediante el análisis lógico
5. **Diseñar** algoritmos simples usando pseudocódigo con estructuras condicionales

---

## 📚 Introducción: ¿Qué es el Álgebra Proposicional?

### 🔍 La Lógica en Nuestra Vida Diaria

Cada día tomamos decisiones basadas en condiciones lógicas, aunque no nos demos cuenta. Cuando dices "Si estudio, entonces pasaré el examen" o "Puedo salir si hago la tarea y limpio mi cuarto", estás usando lógica proposicional sin saberlo.

**El álgebra proposicional** es la rama de la matemática que estudia las proposiciones y las formas en que se combinan para obtener nuevas proposiciones. Es el fundamento de:

- La programación de computadoras
- Los circuitos eléctricos y electrónicos
- La toma de decisiones automatizada
- El razonamiento jurídico y filosófico

### 💡 ¿Por qué aprender esto?

La lógica proposicional desarrolla tu capacidad de:
- Razonar de manera ordenada y sistemática
- Identificar errores en argumentos
- Programar y crear algoritmos
- Tomar decisiones basadas en condiciones claras

---

## 🧠 Sesión 1: Fundamentos de Proposiciones

### ⏱️ Duración: 120 minutos (con descanso incluido)

---

## 1. ¿Qué es una Proposición?

### Definición

Una **proposición** es una oración declarativa que puede ser verdadera (V) o falsa (F), pero nunca ambas a la vez.

### Ejemplos para Discusión

| Oración | ¿Es proposición? | ¿Por qué? |
|---------|------------------|-----------|
| "El sol es una estrella" | ✅ Sí | Es verdadera |
| "5 + 3 = 8" | ✅ Sí | Es verdadera |
| "Bogotá es la capital de Colombia" | ✅ Sí | Es verdadera |
| "2 + 2 = 5" | ✅ Sí | Es falsa (pero sigue siendo proposición) |
| "¿Qué hora es?" | ❌ No | Es una pregunta |
| "¡Hola!" | ❌ No | Es una exclamación |
| "Cierra la puerta" | ❌ No | Es una orden/imperativo |
| "x + 3 = 7" | ❌ No | No se puede determinar sin conocer x |

### 📝 Actividad 1: Identificación de Proposiciones

**Instrucciones:** Clasifica cada oración como proposición (P) o no proposición (NP). Si es proposición, indica si es verdadera (V) o falsa (F).

1. "El agua hierve a 100°C al nivel del mar" → _______
2. "Los pingüinos pueden volar" → _______
3. "¡Vamos al parque!" → _______
4. "3 × 4 = 12" → _______
5. "Colombia está en Europa" → _______
6. "x es mayor que 5" → _______
7. "El número 7 es par" → _______
8. "¿Te gusta la música?" → _______

---

## 2. Proposiciones Simples vs. Compuestas

### Proposiciones Simples (Atómicas)

Son aquellas que expresan una sola idea y no containen otras proposiciones en su estructura.

**Ejemplos:**
- "Hoy es lunes"
- "El cielo es azul"
- "Mi perro se llama Max"
- "6 > 3"

### Proposiciones Compuestas (Moleculares)

Se forman combinando dos o más proposiciones simples mediante **conectivos lógicos**.

**Estructura básica:**
- **Conjunción** (Y): "p ∧ q" → "Hoy es lunes Y hace sol"
- **Disyunción** (O): "p ∨ q" → "Voy al cine O me quedo en casa"
- **Negación** (NO): "¬p" → "NO hace frío"

### 📝 Actividad 2: Clasificación de Proposiciones

**Instrucciones:** Identifica si cada proposición es simple (S) o compuesta (C). Si es compuesta, identifica el conectivo lógico usado.

1. "El libro es interesante y tiene muchas páginas" → _______
2. "María estudia medicina" → _______
3. "No voy a la fiesta" → _______
4. "Si llueve, entonces me quedo en casa" → _______
5. "El número es par o impar" → _______
6. "Juan juega fútbol" → _______

---

## 3. Operaciones Lógicas Fundamentales

### 3.1 Negación (¬p) - "NO"

La negación invierte el valor de verdad de una proposición.

**Tabla de Verdad de la Negación:**

| p | ¬p |
|---|----|
| V | F |
| F | V |

**Ejemplos cotidianos:**

| p | ¬p (Negación) |
|---|---------------|
| "Hace sol" | "NO hace sol" / "No hace sol" |
| "Tengo hambre" | "NO tengo hambre" |
| "El examen es difícil" | "El examen NO es difícil" |

**💡 Ejemplo en decisiones:**
- Si tu mamá dice: "Tienes que limpiar tu cuarto", la negación sería: "NO tienes que limpiar tu cuarto"

---

### 3.2 Conjunción (p ∧ q) - "Y"

La conjunción es verdadera SOLO cuando ambas proposiciones son verdaderas.

**Tabla de Verdad de la Conjunción:**

| p | q | p ∧ q |
|---|---|-------|
| V | V | **V** |
| V | F | F |
| F | V | F |
| F | F | F |

**Nemotecnia:** Piensa en "Y" como en "Ambas deben cumplirse"

**Ejemplos cotidianos:**

| p | q | p ∧ q | Contexto |
|---|---|-------|----------|
| "Tengo dinero" | "La tienda está abierta" | ¿? | "Puedo comprar" |
| "Terminé la tarea" | "Limpié mi cuarto" | ¿? | "Mis papás me dejan salir" |
| "Tengo credencial" | "Pagué la cuota" | ¿? | "Puedo entrar al club" |

**💡 Ejemplo en decisiones:**
- "Puedo salir a jugar SI Y SOLO SI termino la tarea Y hago la cena"
- ¿Cuándo puedo salir? Solo cuando AMBAS condiciones sean verdaderas

---

### 3.3 Disyunción (p ∨ q) - "O"

La disyunción es verdadera cuando AL MENOS UNA de las proposiciones es verdadera.

**Tabla de Verdad de la Disyunción:**

| p | q | p ∨ q |
|---|---|-------|
| V | V | **V** |
| V | F | **V** |
| F | V | **V** |
| F | F | F |

**Nemotecnia:** Piensa en "O" como en "Una u otra, o ambas"

**Ejemplos cotidianos:**

| p | q | p ∨ q | Contexto |
|---|---|-------|----------|
| "Tomo el bus" | "Tomo el metro" | ¿? | "Llego a tiempo" |
| "Estudio medicina" | "Estudio ingeniería" | ¿? | "Seré profesional" |
| "Es festivo" | "Es domingo" | ¿? | "No hay clase" |

**💡 Ejemplo en decisiones:**
- "Para el almuerzo hay arroz O pasta" → Si hay ambos, también se cumple
- "Trae tu cédula O tu pasaporte" → Cualquiera de los dos funciona

---

### 📝 Actividad 3: Tablas de Verdad Básico

**Instrucciones:** Completa las siguientes tablas de verdad

#### Tabla 1: Negación

| p | q | ¬p | ¬q |
|---|---|----|----|
| V | V | | |
| V | F | | |
| F | V | | |
| F | F | | |

#### Tabla 2: Conjunción

| p | q | p ∧ q |
|---|---|-------|
| V | V | |
| V | F | |
| F | V | |
| F | F | |

#### Tabla 3: Disyunción

| p | q | p ∨ q |
|---|---|-------|
| V | V | |
| V | F | |
| F | V | |
| F | F | |

---

### 📝 Actividad 4: Evaluando Proposiciones Compuestas

**Instrucciones:** Determina el valor de verdad de las proposiciones compuestas

**Contexto:** Imagina que es un día entre semana (no fin de semana) y estás en clase.

1. "Es de día Y estamos en clase"
   - p = "Es de día" (V)
   - q = "Estamos en clase" (V)
   - p ∧ q = _______

2. "Es fin de semana O es lunes"
   - p = "Es fin de semana" (F)
   - q = "Es lunes" (F, si es martes)
   - p ∨ q = _______

3. "NO es de noche"
   - p = "Es de noche" (F)
   - ¬p = _______

4. "Tengo 15 años Y soy estudiante"
   - p = "Tengo 15 años" (V)
   - q = "Soy estudiante" (V)
   - p ∧ q = _______

---

## 🔄 Descanso: 15 minutos

**Tiempo: minuto 120**

**Actividades sugeridas durante el descanso:**
- Stretching básico
- Hidratarse
- Interactuar con compañeros
- Respirar aire fresco si es posible

---

## 🧠 Sesión 2: Aplicaciones y Profundización

### ⏱️ Duración: 105 minutos (hasta minuto 225)

---

## 4. Construyendo Tablas de Verdad Complejas

### Combinando Operaciones

Ahora combinaremos las tres operaciones lógicas para crear proposiciones más complejas.

**Estructura:** ¬(p ∧ q)

**Ejemplo paso a paso:**

Construyamos la tabla de verdad para: **¬(p ∧ q)**

| p | q | p ∧ q | ¬(p ∧ q) |
|---|---|-------|----------|
| V | V | V | **F** |
| V | F | F | **V** |
| F | V | F | **V** |
| F | F | F | **V** |

**¿Qué significa?** "NO (p Y q)" es verdadero excepto cuando AMBAS proposiciones son verdaderas.

### 📝 Actividad 5: Tablas de Verdad Compuestas

**Instrucciones:** Completa las siguientes tablas de verdad

#### Tabla A: (p ∨ q) ∧ ¬p

| p | q | p ∨ q | ¬p | (p ∨ q) ∧ ¬p |
|---|---|-------|----|--------------|
| V | V | | | |
| V | F | | | |
| F | V | | | |
| F | F | | | |

#### Tabla B: ¬p ∧ ¬q

| p | q | ¬p | ¬q | ¬p ∧ ¬q |
|---|---|----|----|---------|
| V | V | | | |
| V | F | | | |
| F | V | | | |
| F | F | | | |

#### Tabla C: (p ∧ q) ∨ (¬p ∧ ¬q)

| p | q | p ∧ q | ¬p | ¬q | ¬p ∧ ¬q | (p ∧ q) ∨ (¬p ∧ ¬q) |
|---|---|-------|----|----|---------|---------------------|
| V | V | | | | | |
| V | F | | | | | |
| F | V | | | | | |
| F | F | | | | | |

---

## 5. Dinámica: "Si pasa esto, entonces..."

### 🎯 Objetivo

Interiorizar las estructuras lógicas mediante la creación de condicionales basados en situaciones reales.

### Concepto: La Implicación (→)

Aunque no profundizaremos en la implicación como operación, es importante reconocer su estructura:

**"Si p, entonces q"** o **p → q**

- p se llama **antecedente** (condición)
- q se llama **consecuente** (resultado)

**Tabla de Verdad de la Implicación:**

| p | q | p → q |
|---|---|-------|
| V | V | **V** |
| V | F | F |
| F | V | **V** |
| F | F | **V** |

> **Nota:** En lógica, una implicación solo es falsa cuando la condición se cumple pero el resultado no ocurre.

### 📝 Actividad 6: Dinámica en Parejas - "Si... entonces..."

**Instrucciones:** Cada pareja crea 5 proposiciones condicionales basadas en situaciones escolares y luego las comparte con otra pareja.

**Formato:**

```
Si [condición], entonces [consecuencia]
```

**Ejemplos proporcionados:**

1. Si estudio 2 horas, entonces pasaré el examen
2. Si llueve, entonces se cancela el recreo
3. Si traigo la tarea, entonces me dan puntos extra

**Tu turno (crea 5 más):**

1. ______________________________________
2. ______________________________________
3. ______________________________________
4. ______________________________________
5. ______________________________________

**Análisis:** Identifica en cada caso:
- ¿Cuál es el antecedente (p)?
- ¿Cuál es el consecuente (q)?
- ¿En qué caso la implicación sería falsa?

---

### 📝 Actividad 7: Análisis de Decisiones Cotidianas

**Instrucciones:** Analiza las siguientes situaciones usando lógica proposicional

**Situación 1: El fin de semana**

Tu mamá te dice: "Puedes usar el computador SI Y SOLO SI terminas la tarea Y limpias tu cuarto"

| Condición | ¿Se cumple? |
|-----------|--------------|
| Terminaste la tarea | SÍ |
| Limpiaste tu cuarto | SÍ |

¿Puedes usar el computador? _______

| Condición | ¿Se cumple? |
|-----------|--------------|
| Terminaste la tarea | SÍ |
| Limpiaste tu cuarto | NO |

¿Puedes usar el computador? _______

**Situación 2: El viaje escolar**

"Para el viaje se necesita: traer el permiso FIRMADO O tener autorización de los padres, Y pagar la cuota completa"

| Requisitos | Situación A | Situación B |
|-------------|-------------|-------------|
| Permiso firmado | SÍ | NO |
| Autorización padres | NO | SÍ |
| Cuota pagada | SÍ | SÍ |

Situación A: ¿Puede ir? _______
Situación B: ¿Puede ir? _______

---

## 6. Introducción al Pseudocódigo

### ¿Qué es el Pseudocódigo?

El **pseudocódigo** es una forma de escribir algoritmos usando lenguaje común, mezclado con elementos de programación. Es "casi código" pero fácil de entender.

### Estructuras Básicas en Pseudocódigo

#### 1. Declarar Variables

```
edad = 15
tieneTarea = verdadero
nombre = "María"
```

#### 2. Condicional Simple (SI... ENTONCES)

```
SI (condición) ENTONCES
    // hacer algo
FIN SI
```

#### 3. Condicional Compuesto (SI... SINO)

```
SI (condición) ENTONCES
    // hacer algo
SINO
    // hacer otra cosa
FIN SI
```

#### 4. Condiciones Compuestas (Y, O)

```
SI (condición1 Y condicion2) ENTONCES
    // ambas deben cumplirse
FIN SI

SI (condicion1 O condicion2) ENTONCES
    // al menos una debe cumplirse
FIN SI
```

### 📝 Actividad 8: Escribiendo Pseudocódigo

**Instrucciones:** Convierte cada situación en pseudocódigo

**Ejemplo 1: Verificar mayoría de edad**

```
EDAD = 18

SI (EDAD >= 18) ENTONCES
    ESCRIBIR "Eres mayor de edad"
SINO
    ESCRIBIR "Eres menor de edad"
FIN SI
```

**Tu turno:**

**Situación A:** Un sistema que verifica si un estudiante puede entrar al cine

```
// El cine permite entrada si:
// - Tiene 18 años O
// - Está acompañado de un adulto

EDAD = 15
ACOMPAÑADO_DE_ADULTO = verdadero

// Escribe tu pseudocódigo aquí

```

**Situación B:** Un programa que determina si puedes salir a jugar

```
TIENE_TAREA_COMPLETA = falso
TIENE_CUARTO_LIMPIO = verdadero
ES_HORA_DE_SALIR = verdadero

// Escribe tu pseudocódigo aquí


```

**Situación C:** Verificar si un número es par Y positivo

```
NUMERO = 4

// Escribe tu pseudocódigo aquí


```

---

### 📝 Actividad 9: Pseudocódigo con Decisiones Complejas

**Instrucciones:** Completa el pseudocódigo para cada escenario

**Escenario 1: Sistema de calificaciones**

```
// Un estudiante aprueba si:
// - Saque más de 3.0 Y faltó menos de 3 días
// - O sacaron 5.0 exactamente

NOTA = 3.5
DIAS_FALTADOS = 2

SI ( (NOTA > 3.0 Y DIAS_FALTADOS < 3) O NOTA == 5.0 ) ENTONCES
    ESCRIBIR "El estudiante APRUEBA"
SINO
    ESCRIBIR "El estudiante REPRUEBA"
FIN SI
```

**Resultado:** _______ (¿Por qué?)

**Escenario 2: Acceso a la biblioteca**

```
// Puede usar la biblioteca si:
// - Es estudiante Y tiene carné vigente
// - O es docente

ES_ESTUDIANTE = verdadero
CARNÉ_VIGENTE = falso
ES_DOCENTE = false

// Tu pseudocódigo aquí

```

**¿Puede acceder?** _______

---

## 7. Proyecto Final: Construyendo un Analizador de Decisiones

### 📋 Descripción

En grupos de 3-4 personas, crearán un "analizador de decisiones" usando pseudocódigo.

### Requisitos del Proyecto

1. **Contexto:** Elegir una situación de la vida cotidiana (fiesta, viaje, juego, etc.)
2. **Condiciones:** Usar al menos 2 conectivos lógicos (Y, O, NO)
3. **Pseudocódigo:** Escribir el algoritmo completo
4. **Tabla de verdad:** Crear una tabla que muestre todas las combinaciones posibles

### Ejemplo de Referencia

**Tema:** Decidir si puedo ir a una fiesta

```
// CONDICIONES:
// - Tengo permiso de mis papás
// - Tengo dinero suficiente
// - No tengo examen al día siguiente
// - Mis papás conocen a los papás del que da la fiesta

PERMISO = verdadero
DINERO = verdadero
NO_EXAMEN = false
PADRES_CONOCIDOS = verdadero

SI ( (PERMISO Y DINERO) Y (NO_EXAMEN O PADRES_CONOCIDOS) ) ENTONCES
    ESCRIBIR "PUEDO IR A LA FIESTA"
SINO
    ESCRIBIR "NO PUEDO IR A LA FIESTA"
FIN SI
```

### 🎯 Rúbrica de Evaluación

| Criterio | Excelente (4) | Bueno (3) | Regular (2) | Necesita Mejorar (1) |
|----------|---------------|-----------|-------------|----------------------|
| Uso de conectivos | Usa 3 conectivos correctamente | Usa 2 conectivos correctamente | Usa 1 conectivo correctamente | No usa conectivos |
| Claridad del pseudocódigo | Pseudocódigo claro y ejecutable | Pseudocódigo entendible | Pseudocódigo confuso | Pseudocódigo incompleto |
| Tabla de verdad | Completa y correcta | Completa con 1 error | Incompleta | No la incluye |
| Creatividad | Situación muy original y compleja | Situación original | Situación común | Situación muy simple |

---

## 🔄 Descanso: 15 minutos

**Tiempo: minuto 180**

**Actividades sugeridas:**
- Revisar el proyecto en grupos
- Compartir ideas con compañeros
- Snack y descanso

---

## 🧠 Sesión 3: Síntesis y Cierre

### ⏱️ Duración: 15 minutos (minutos 195-210)

---

## 8. Resumen de Conceptos Clave

### 📌 Puntos Fundamentales

| Concepto | Símbolo | Significado | Ejemplo |
|----------|---------|-------------|---------|
| **Negación** | ¬p | Invierte el valor | "No estudio" |
| **Conjunción** | p ∧ q | Ambas verdaderas | "Tengo dinero Y tiempo" |
| **Disyunción** | p ∨ q | Al menos una verdadera | "Tomo bus O metro" |
| **Implicación** | p → q | Si p, entonces q | "Si estudio, paso" |

### 📌 Tablas de Verdad Resumen

```
NEGACIÓN:         CONJUNCIÓN:        DISYUNCIÓN:
p ¬p              p q p∧q           p q p∨q
V F               V V V             V V V
F V               V F F             V F V
                  F V F             F V V
                  F F F             F F F
```

---

## 📝 Actividad Final: Autoevaluación

**Instrucciones:** Responde cada pregunta

1. ¿Cuál es la diferencia entre una proposición simple y una compuesta?
   _________________________________________________________________

2. ¿Cuándo es verdadera una conjunción?
   _________________________________________________________________

3. ¿Cuándo es falsa una disyunción?
   _________________________________________________________________

4. ¿Qué hace la negación a una proposición?
   _________________________________________________________________

5. Escribe un ejemplo de tu vida diaria que use conjunción:
   _________________________________________________________________

6. Escribe un ejemplo de tu vida diaria que use disyunción:
   _________________________________________________________________

7. ¿Para qué sirve el pseudocódigo?
   _________________________________________________________________

---

## 📚 Materiales Adicionales

### Ejercicios Extra para Práctica

**Nivel Básico:**

1. Construye la tabla de verdad para: p ∧ (q ∨ r)
2. Evalúa: "No es cierto que 2 + 2 = 5" (determina si es V o F)
3. Escribe la negación de: "Me gusta el fútbol"

**Nivel Intermedio:**

1. Crea un sistema de login con pseudocódigo que requiera:
   - Usuario correcto Y contraseña correcta
   - O ser administrador

2. Analiza: "Si no estudias, entonces no pasarás el año"
   - ¿Es verdadera o falsa si estudiaste y no pasaste?

**Nivel Avanzado:**

1. Construye la tabla de verdad para: (p → q) ∧ (q → p)
2. Diseña un sistema de recomendación de películas usando pseudocódigo

---

## 📅 Distribución del Tiempo

| Bloque | Contenido | Duración |
|--------|-----------|----------|
| **Sesión 1** | Proposiciones simples y compuestas | 45 min |
| | Operaciones lógicas (¬, ∧, ∨) | 45 min |
| | Tablas de verdad básicas | 30 min |
| **DESCANSO** | | 15 min |
| **Sesión 2** | Tablas de verdad complejas | 25 min |
| | Dinámica "Si... entonces..." | 25 min |
| | Pseudocódigo básico | 40 min |
| | Proyecto en grupos | 15 min |
| **DESCANSO** | | 15 min |
| **Sesión 3** | Síntesis y autoevaluación | 15 min |
| | **TOTAL** | **240 min** |

---

## ✅ Cierre

¡Felicitaciones! Has completado tu introducción al álgebra proposicional. Ahora tienes las herramientas para:

- Pensar de manera más lógica y estructurada
- Entender cómo funcionan las computadoras al tomar decisiones
- Resolver problemas usando un enfoque sistemático
- Escribir algoritmos básicos

**Recuerda:** La lógica está en todo lo que nos rodea. Cada vez que tomas una decisión, estás aplicando principios lógicos, ¡ahora de manera consciente!

---

*Material desarrollado para uso educativo*
*Adaptado para jóvenes de 15-16 años*
*Duración: 4 horas académicas con dos descansos*
