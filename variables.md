# Guía de Estudio: Variables en Python

**Curso de Programación - Nivel Básico**  
**Público objetivo: Jóvenes de 15-16 años**

---

## ¿Qué es una Variable?

Una **variable** es un contenedor que guarda un valor en la memoria del programa. Piensa en ella como una caja etiquetada donde guardas información que luego puedes usar o cambiar.

```
┌─────────────────┐
│    edad = 16    │  →  La caja "edad" contiene el número 16
└─────────────────┘
```

---

## 1. Crear Variables

En Python, crear una variable es simple: escribes el nombre, el signo `=`, y el valor.

```python
# Variables de diferentes tipos
nombre = "Carlos"      # Texto (string)
edad = 16              # Número entero (int)
altura = 1.75          # Número decimal (float)
es_estudiante = True   # Booleano (True/False)
```

### Tipos de Datos Básicos

| Tipo | Ejemplo | Descripción |
|------|---------|-------------|
| `int` | `15`, `100`, `-5` | Números enteros |
| `float` | `1.75`, `3.14`, `0.5` | Números con decimales |
| `str` | `"Hola"`, `'Ana'` | Texto (strings) |
| `bool` | `True`, `False` | Valores lógicos |

---

## 2. Usar Variables

### En expresiones aritméticas

```python
ancho = 5
largo = 10
area = ancho * largo  # 50

radio = 3
pi = 3.14159
circunferencia = 2 * pi * radio  # 18.85
```

### En comparaciones (expresiones relacionales)

```python
nota = 85
aprobado = nota >= 60  # True

edad = 16
es_adolescente = 13 <= edad <= 19  # True
```

### En expresiones lógicas (booleanas)

```python
tiene_dinero = True
tiene_tiempo = False
puede_salir = tiene_dinero and tiene_tiempo  # False

es_fin_semana = True
esta_lloviendo = False
paseo = es_fin_semana and not esta_lloviendo  # True
```

### En estructuras de control

```python
temperatura = 25
llueve = False

if temperatura > 30 and not llueve:
    print("Ve a la playa")
elif temperatura >= 15 and not llueve:
    print("Sal a caminar")
else:
    print("Quédate en casa")
```

---

## 3. Reglas para Nombrar Variables

| ✅ Correcto | ❌ Incorrecto | Por qué |
|------------|--------------|---------|
| `edad` | `2edad` | No puede empezar con número |
| `nota_final` | `nota-final` | El guion se confunde con resta |
| `tiene_permiso` | `tiene permiso` | No puede haber espacios |
| `_temp` | `class` | `class` es palabra reservada |

### Convenciones recomendadas

```python
# ✅ BUENO - Usar minúsculas con guiones bajos
nombre_estudiante = "Ana"
calificacion_final = 95
es_aprobado = True
contador = 0

# ❌ EVITAR - Nombres poco claros
n = "Ana"
c = 95
e = True
x = 0
```

### Buenos nombres son descriptivos

```python
# ❌ Malo - ¿Qué significa?
x = 75

# ✅ Bueno - Se entiende inmediatamente
nota = 75
```

---

## 4. Modificar Variables

### Actualizar el valor

```python
edad = 16
print(edad)  # 16

edad = 17    # El valor anterior (16) se sobrescribe
print(edad)  # 17
```

### Operaciones con la misma variable

```python
contador = 0
contador = contador + 1  # 1
contador = contador + 1  # 2
contador += 1            # 3 (forma abreviada)
```

```python
puntaje = 100
puntaje -= 25            # 75 (restar)
puntaje *= 2             # 150 (multiplicar)
```

---

## 5. Variables en Estructuras de Control

### En if/elif/else

```python
edad = 16

if edad < 13:
    print("Niño")
elif edad <= 19:
    print("Adolescente")
elif edad <= 59:
    print("Adulto")
else:
    print("Adulto mayor")
```

### En ciclos (while/for)

```python
# While: usar variable como contador
contador = 1
while contador <= 3:
    print(f"Iteración {contador}")
    contador += 1

# For: iterar usando variable
frutas = ["manzana", "banana", "cereza"]
for fruta in frutas:
    print(f"Me gusta la {fruta}")
```

---

## 📝 Ejercicios Prácticos

### Ejercicio 1: Calculadora de área

```python
# Calcula el área de un rectángulo
ancho = 8
largo = 12
area = ancho * largo
print(f"El área es: {area}")
```

<details>
<summary>✅ Ver respuesta</summary>
El área es: 96
</details>

### Ejercicio 2: Verificar aprobación

```python
# ¿El estudiante apruebó?
nota = 72
aprobado = nota >= 60
print(f"¿Aprobado? {aprobado}")
```

<details>
<summary>✅ Ver respuesta</summary>
¿Aprobado? True
</details>

### Ejercicio 3: Condición lógica

```python
# ¿Puede salir?
tiene_dinero = True
tiene_permiso = False
puede_salir = tiene_dinero or tiene_permiso
print(f"¿Puede salir? {puede_salir}")
```

<details>
<summary>✅ Ver respuesta</summary>
¿Puede salir? True
</details>

### Ejercicio 4: Clasificador de temperatura

```python
temperatura = 22

if temperatura > 30:
    print("Calor")
elif temperatura >= 15:
    print("Agradable")
else:
    print("Frío")
```

<details>
<summary>✅ Ver respuesta</summary>
Agradable
</details>

### Ejercicio 5: Contador con while

```python
contador = 1
while contador <= 4:
    print(contador)
    contador += 1
```

<details>
<summary>✅ Ver respuesta</summary>
1
2
3
4
</details>

---

## 📋 Resumen Rápido

```python
# Crear variables
nombre = "Ana"
edad = 16
altura = 1.70
es_estudiante = True

# Usar en operaciones
año_siguiente = edad + 1
es_mayor = edad >= 18

# Usar en condiciones
if es_estudiante and edad >= 15:
    print("Puede obtener credencial")

# Modificar
contador = 0
contador += 1  # Ahora vale 1
```

---

## ✅ Autoevaluación

| # | Pregunta | Tu respuesta |
|---|----------|--------------|
| 1 | ¿Cómo se crea una variable llamada `edad` con valor 15? | |
| 2 | ¿Cuál es el tipo de `3.14`? | |
| 3 | ¿Qué operador se usa para comparar si dos valores son iguales? | |
| 4 | ¿Cómo aumentas `contador` en 1 de forma abreviada? | |
| 5 | ¿Por qué `nota-final` es un mal nombre de variable? | |

<details>
<summary>✅ Respuestas</summary>

1. `edad = 15`
2. float
3. `==`
4. `contador += 1`
5. El guion se confunde con el operador resta

</details>

---

*Material creado para el curso de programación autoguiado*