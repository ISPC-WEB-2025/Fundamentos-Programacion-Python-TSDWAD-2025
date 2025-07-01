# Guía de Estructura y Creación de Contenido del Repositorio - Fundamentos de Programación Python

Este documento es una guía para el equipo sobre la organización del repositorio `Fundamentos-Programacion-Python-TSDWAD-2025` y cómo crear y gestionar el material de estudio utilizando Jupyter Notebooks (Google Colab).

---

## 1. Estructura de Carpetas del Repositorio

La siguiente estructura de carpetas se propone para organizar de manera lógica y modular todo el material de la materia. Esta sigue el programa de estudios y facilita la navegación.

```

Fundamentos-Programacion-Python-TSDWAD-2025/
├── Unidad 1 - Introduccion a Python/
│   ├── 01\_Introduccion\_a\_Python\_Fundamentos.ipynb  \# Notebook de ejemplo para el primer tema
│   ├── 02\_Operadores\_y\_Expresiones.ipynb            \# (Ejemplo para el siguiente notebook)
│   └── ejercicios/                                 \# Para posibles scripts de ejercicios adicionales
├── Unidad 2 - Estructuras de Control y Datos/
│   ├── 01\_Estructuras\_Control\_Secuenciales\_Condicionales.ipynb
│   ├── 02\_Estructuras\_Control\_Iterativas\_Bucles.ipynb
│   ├── 03\_Tipos\_Datos\_Simples.ipynb
│   ├── 04\_Listas\_Tuplas\_Diccionarios.ipynb
│   └── ejercicios/
├── Unidad 3 - Funciones y Modularidad/
│   ├── 01\_Funciones\_Definicion\_Uso.ipynb
│   └── ejercicios/
├── Unidad 4 - Introduccion a POO/
│   ├── 01\_Conceptos\_POO\_Clases\_Objetos.ipynb
│   ├── 02\_Fundamentos\_POO\_Abstraccion\_Encapsulamiento.ipynb
│   └── ejercicios/
├── Unidad 5 - POO Avanzada y UML/
│   ├── 01\_Herencia\_Polimorfismo.ipynb
│   ├── 02\_Diseño\_UML\_Introduccion.ipynb
│   └── ejercicios/
├── Unidad 6 - Control\_Depuracion\_Testing/
│   ├── 01\_Errores\_Depuracion.ipynb
│   └── ejercicios/
├── README.md                                       \# Archivo README principal del repositorio
└── .gitignore                                      \# Configuración para ignorar archivos no deseados por Git

````

### Explicación de la Estructura:

* **Raíz del Repositorio (`Fundamentos-Programacion-Python-TSDWAD-2025/`):** Carpeta principal donde se alojará todo el proyecto.
* **Carpetas por Unidad (`Unidad X - Nombre de la Unidad/`):** Cada una representa una sección del programa. La numeración ayuda al orden cronológico y los nombres descriptivos facilitan la identificación del contenido.
* **Jupyter Notebooks (`NN_NombreDelTema.ipynb`):**
    * Archivos `.ipynb` que contienen la teoría, ejemplos y ejercicios interactivos.
    * La numeración `NN_` (ej. `01_`, `02_`) dentro de cada unidad mantiene el orden secuencial de los temas.
    * Los nombres deben ser descriptivos y reflejar el contenido del notebook.
* **Carpeta `ejercicios/` (Opcional dentro de cada Unidad):**
    * Para almacenar scripts de Python (`.py`) o ejercicios más complejos que no se integran directamente en los notebooks.
    * **Alternativa:** Los ejercicios cortos y auto-contenidos pueden incluirse directamente al final del notebook correspondiente.
* **`README.md` (en la raíz):** Es el índice general del repositorio. Contendrá la descripción del curso, objetivos, contenidos y enlaces a cada una de las notebooks.
* **`.gitignore` (en la raíz - recomendado):** Archivo que instruye a Git qué archivos y carpetas debe ignorar (ej. `.ipynb_checkpoints/`, `__pycache__/`, `.vscode/`) para mantener el repositorio limpio.

---

## 2. Creación y Contenido de las Notebooks

Las notebooks combinan explicaciones teóricas (en Markdown) con ejemplos de código (en Python) que se pueden ejecutar interactivamente.

### Ejemplo de  Primera Notebook:

**Nombre del archivo:** `01_Introduccion_a_Python_Fundamentos.ipynb`

Esta notebook se centrará en los conceptos básicos de Python y su entorno.

```python
# Contenido de `01_Introduccion_a_Python_Fundamentos.ipynb`

"""
# 01 - Introducción a Python y Fundamentos

Este notebook es el punto de partida para tu viaje en la programación con Python. Abordaremos los conceptos fundamentales del lenguaje, sus características clave, la filosofía detrás de su diseño y cómo empezar a escribir tu primer código.

---

## 1. ¿Qué es Python?

Python es un lenguaje de programación de alto nivel que se ha convertido en una herramienta esencial para desarrolladores de todo el mundo. Su diseño enfatiza la legibilidad del código con una sintaxis que permite a los programadores expresar conceptos complejos en menos líneas de código.

## 2. Características Principales de Python

Algunas de las características que hacen a Python tan popular incluyen:

* **Sencillo y legible:** Su sintaxis es clara y se asemeja al lenguaje natural, facilitando el aprendizaje.
* **Multipropósito:** Se utiliza en desarrollo web, ciencia de datos, inteligencia artificial, automatización, scripting y más.
* **Multiplataforma:** Funciona en Windows, macOS, Linux y otros sistemas operativos.
* **Interpretado:** El código se ejecuta directamente sin necesidad de una compilación previa a un formato binario.
* **Comunidad activa:** Cuenta con una gran comunidad de desarrolladores que contribuyen con librerías y soporte.

## 3. El Zen de Python (Tim Peters)

El "Zen de Python" es una colección de principios que influyen en el diseño del lenguaje Python. Puedes acceder a ellos ejecutando `import this` en un intérprete de Python. Aquí algunos de los principios más relevantes para un principiante:
"""

# Bloque de Código
import this

"""
**Principios clave a recordar:**
* **Bello es mejor que feo.**
* **Explícito es mejor que implícito.**
* **Simple es mejor que complejo.**
* **Leíble es mejor que difícil de leer.**
* **Los casos especiales no son lo suficientemente especiales como para romper las reglas.** (Aunque la practicidad le gana a la pureza.)

---

## 4. Entorno de Trabajo: ¿Dónde escribir y ejecutar Python?

Puedes escribir y ejecutar código Python de diversas maneras, adaptándose a tus preferencias y necesidades.

### a) Editores de Código Locales (VS Code, PyCharm, Sublime Text)

Para trabajar en tu computadora:

* **Instalación de Python:** Necesitas tener Python instalado en tu sistema.
* **Editor de Código:** Utiliza un editor como VS Code, que con las extensiones adecuadas (como la de Python y Jupyter) se convierte en un potente entorno de desarrollo.

**Pasos generales para tu primer programa local:**
1.  Abre tu editor (ej. VS Code).
2.  Crea un nuevo archivo con extensión `.py` (ej. `hola.py`).
3.  Escribe tu código.
4.  Ejecuta desde la terminal integrada del editor (`python hola.py`).

### b) Entornos de Código Online (Google Colaboratory - Colab)

Son excelentes para empezar, ya que no requieren ninguna instalación en tu computadora y funcionan directamente en el navegador. **Google Colab es el más recomendado para este curso.**

* **Ventajas:** Acceso instantáneo, fácil de compartir, gratuito, ideal para notebooks interactivos.
* **Desventajas:** Requiere conexión a internet, recursos limitados para tareas muy pesadas.

---

## 5. Tu Primer Programa en Python: "¡Hola Mundo!"

Vamos a escribir y ejecutar nuestro primer código para entender cómo Python procesa instrucciones secuencialmente.

### a) La función `print()`

La función `print()` se usa para mostrar mensajes en la consola.
"""

# Bloque de Código
print("¡Hola, mundo desde Python!")
print("Bienvenido al curso de Fundamentos de Programación.")

"""
### b) La función `input()` para interactuar

La función `input()` permite que el usuario ingrese datos desde el teclado.
"""

# Bloque de Código
nombre = input("¿Cuál es tu nombre? ")
print("Es un placer conocerte,", nombre, "!")

"""
### c) Ejemplos combinados de operaciones básicas

Las instrucciones se ejecutan secuencialmente, una tras otra.
"""

# Bloque de Código
print("--- Calculadora Básica ---")
num1_str = input("Ingresa el primer número: ")
num2_str = input("Ingresa el segundo número: ")

num1 = float(num1_str)
num2 = float(num2_str)

suma = num1 + num2
resta = num1 - num2
multiplicacion = num1 * num2
division = num1 / num2

print(f"La suma es: {suma}")
print(f"La resta es: {resta}")
print(f"La multiplicación es: {multiplicacion}")
print(f"La división es: {division}")
print("--- Operaciones finalizadas ---")

"""
---

## 6. Ejercicios Propuestos

Estos ejercicios te ayudarán a familiarizarte con las operaciones básicas y la entrada/salida de datos, preparando el terreno para las estructuras de control.

1.  **Área de un Círculo:** Escribe un programa que pida al usuario el radio de un círculo y calcule su área (Área = π * radio²). Puedes usar `3.14159` como valor de π.
2.  **Conversor de Temperatura:** Escribe un programa que convierta una temperatura dada en grados Celsius a grados Fahrenheit (F = C * 1.8 + 32).
3.  **Hipotenusa de un Triángulo:** Escribe un programa que pida al usuario los dos catetos de un triángulo rectángulo y calcule la hipotenusa (Hipotenusa² = CatetoA² + CatetoB²). Puedes usar `** 0.5` para la raíz cuadrada.
4.  **Saludo Personalizado con Edad:** Escribe un programa que pida al usuario su año de nacimiento, calcule su edad y genere un mensaje de saludo personalizado que incluya su nombre y edad.
"""
````

-----

## 3\. Guía de Creación y Gestión de Notebooks (Google Colab / VS Code)

Este apartado explica cómo crear, editar y descargar los Jupyter Notebooks, que son el formato principal para nuestros apuntes interactivos.

### a) Cómo Crear y Descargar una Notebook en Google Colab (Online - Recomendado)

Google Colab es un entorno de Jupyter Notebook basado en la nube que no requiere instalación y es ideal para empezar.

1.  **Abrir Google Colab:**
      * Abre tu navegador web y ve a: `https://colab.research.google.com/`
      * Haz clic en "Archivo" \> "Nuevo Notebook".
2.  **Copiar Contenido en Celdas:**
      * Un Jupyter Notebook se compone de **celdas**: **Celdas de Texto (Markdown)** para teoría y **Celdas de Código (Python)** para código ejecutable.
      * **Proceso:**
          * Copia el texto Markdown desde el documento de contenido (texto que no está dentro de un bloque de código Python).
          * En Colab, crea una `+ Texto` (celda de texto) y pega el contenido.
          * Copia el código Python desde el documento.
          * En Colab, crea una `+ Código` (celda de código) y pega el código.
          * Repite este proceso para cada sección del contenido de la notebook.
      * **Nota importante:** En los bloques de texto del documento de contenido que están entre triples comillas (`"""`), solo copia el texto *dentro* de las comillas para pegarlo en la celda de Markdown de Colab. Las comillas `"""` son una forma de simular una celda de Markdown dentro de un archivo de texto plano.
3.  **Ejecutar el Código:**
      * Para ejecutar una celda de código, haz clic en el icono de "Play" (▶) que aparece al pasar el cursor sobre la celda.
      * Los resultados se mostrarán justo debajo de la celda.
4.  **Guardar y Descargar:**
      * Colab guarda automáticamente en tu Google Drive.
      * Para obtener el archivo para el repositorio: Ve a `Archivo` \> `Descargar` \> `Descargar .ipynb`.
      * Este archivo `.ipynb` es el que debes subir a la carpeta correspondiente en tu repositorio de GitHub (ej. `Unidad 1 - Introduccion a Python/`).

### b) Cómo Utilizar Notebooks en VS Code con Extensión Jupyter (Local)

Si prefieres trabajar desde tu computadora:

1.  **Requisitos Previos:**
      * [Visual Studio Code](https://code.visualstudio.com/) instalado.
      * [Python](https://www.python.org/downloads/) instalado en tu sistema.
      * **Extensiones de VS Code:** Instala `Python` y `Jupyter` (ambas de Microsoft) desde la sección de Extensiones de VS Code.
2.  **Clonar el Repositorio:**
    ```bash
    git clone [https://github.com/tu_usuario/Fundamentos-Programacion-Python-TSDWAD-2025.git](https://github.com/tu_usuario/Fundamentos-Programacion-Python-TSDWAD-2025.git)
    ```
3.  **Abrir en VS Code:** Abre la carpeta clonada en VS Code (`Archivo > Abrir Carpeta`).
4.  **Abrir y Editar Notebooks:** Navega al archivo `.ipynb` deseado en el explorador de archivos de VS Code y haz doble clic para abrirlo. Podrás editar y ejecutar celdas como en Colab.
5.  **Guardar Cambios:** Guarda el archivo como cualquier otro (Ctrl+S o Cmd+S).

-----

## 4\. Consejos para la Organización del Contenido en Notebooks

  * **Modularidad por Tema:** Crea una notebook por cada tema principal o subtema importante del programa (ej. "Estructuras de Control", "Tipos de Datos", "Clases y Objetos"). Esto mejora la legibilidad y la gestión.
  * **Ejercicios en la Notebook:** Incluye los ejercicios propuestos al final de cada notebook donde se explican los conceptos relacionados.
  * **Resoluciones (Opcional):** Si se decide proveer soluciones:
      * Crear una segunda notebook con prefijo `_Solucion` (ej. `01_Estructuras_Control_Solucion.ipynb`).
      * Crear una subcarpeta `soluciones/` dentro de cada unidad.
      * Discutir las soluciones en sesiones en vivo.

-----

## 5. Flujo de Trabajo y Colaboración (Git)

Para asegurar una colaboración efectiva y un historial de cambios claro en el repositorio, es fundamental seguir ciertas prácticas con Git.

### a) Convenciones de Commits (Conventional Commits)

Para mantener un historial de Git limpio, legible y consistente, se recomienda seguir la convención de Conventional Commits. Esto facilita entender el propósito de cada cambio con solo mirar el mensaje del commit.


**Formato del Mensaje:**

```

\<tipo\>: \<descripción concisa\>

[cuerpo del mensaje (opcional)]

[pie de página (opcional, ej. referencias a issues)]

````

La **primera línea** (`<tipo>: <descripción concisa>`) es la más importante. Debe ser concisa (idealmente < 50-72 caracteres), imperativa (como una instrucción), y usar la convención de tipo (ej. `feat:`). El resto del mensaje (cuerpo y pie de página) es opcional y se utiliza para añadir detalles o contexto adicional.

**Ejemplo de un buen mensaje de commit y cómo se ejecuta:**

```bash
git commit -m "feat: Crear primera notebook de Introducción a Python" -m "Agrega el notebook inicial con conceptos básicos de Python, Zen de Python, y ejemplos de print/input, incluyendo los primeros ejercicios propuestos. Esto establece la base para las unidades siguientes."
````

  * Utilizamos `-m` para la línea de asunto (el primer `-m`).
  * Utilizamos un segundo `-m` para el cuerpo del mensaje (opcional), lo que permite que el mensaje sea multilínea.

**Tipos de Commit Comunes:**

* **`feat` (features):** Cuando agregas una nueva funcionalidad o característica.
    * Ej: `feat: Añadir sección de estructuras de control`
    * Ej: `feat: Implementar calculadora básica con input/print`
* **`fix` (bug fixes):** Cuando solucionas un error (bug).
    * Ej: `fix: Corregir error en cálculo de área de círculo`
* **`docs` (documentation):** Cambios relacionados con la documentación (READMEs, comentarios en código, guías).
    * Ej: `docs: Actualizar guía de uso del repositorio`
    * Ej: `docs: Añadir comentarios explicativos a ejemplos de bucles`
* **`style` (formatting, no code changes):** Cambios que no afectan la lógica del código, solo su formato (espacios en blanco, indentación, punto y coma omitidos, etc.).
    * Ej: `style: Formatear código según PEP8`
* **`refactor` (refactoring code):** Cambios que refactorizan el código sin cambiar su comportamiento externo.
    * Ej: `refactor: Optimizar función de conversión de temperatura`
* **`test` (adding tests):** Cuando agregas o corriges tests.
    * Ej: `test: Añadir pruebas para función de hipotenusa`
* **`chore` (other changes):** Otros cambios que no son código de producción (ej. actualizaciones de herramientas, configuración de builds).
    * Ej: `chore: Actualizar .gitignore`
    * Ej: `chore: Configurar entorno de desarrollo`
* **`build` (build system changes):** Cambios que afectan el sistema de construcción o dependencias externas (npm, pip).
    * Ej: `build: Añadir requirements.txt con dependencias de Python`
* **`ci` (CI related changes):** Cambios en los archivos y scripts de configuración de CI (Continuous Integration).
    * Ej: `ci: Configurar workflow de GitHub Actions`

**Ejemplo de un buen mensaje de commit:**

```
feat: Crear primera notebook de Introducción a Python

Agrega el notebook inicial con conceptos básicos de Python, Zen de Python, y ejemplos de print/input, incluyendo los primeros ejercicios propuestos. Esto establece la base para las unidades siguientes.
```

**Beneficios:**

* **Historial claro:** Facilita ver qué se hizo en cada cambio.
* **Búsqueda eficiente:** Permite buscar commits por tipo (ej. ver todas las nuevas funcionalidades).
* **Colaboración:** Ayuda al equipo a entender el trabajo de los demás rápidamente.
* **Automatización:** Herramientas pueden generar changelogs automáticamente.
 ---

## Aclaración

Cuando usas `git commit -m "..." -m "..."`, cada `-m` inicia una nueva "línea" o párrafo en el mensaje. Si tu "pie de página" (por ejemplo, `Closes #123`) va después de un salto de línea desde el cuerpo principal, simplemente lo incluyes como parte del segundo (o tercer, etc.) `-m` o, lo que es más común y recomendado para mensajes complejos, **simplemente ejecutas `git commit` sin `-m` y dejas que se abra tu editor de texto predeterminado.**

Cuando se abre el editor, puedes escribir todo el mensaje, incluyendo las líneas en blanco necesarias para separar el asunto, el cuerpo y el pie de página, de forma mucho más clara, por ejemplo:

```
feat: Crear primera notebook de Introducción a Python

Agrega el notebook inicial con conceptos básicos de Python, Zen de Python, y ejemplos de print/input, incluyendo los primeros ejercicios propuestos. Esto establece la base para las unidades siguientes.

# Este sería el pie de página, después de una línea en blanco. Ej:
Closes #123  --> cierra issue 123
Refs #456  --> referencia issue 456
```

**En resumen:**

  * **Para asunto y cuerpo (como el primer ejemplo):** Se puede usar, `git commit -m "Asunto" -m "Cuerpo"`.
  * **Para añadir un pie de página estructurado (como `Closes #XYZ`):** Lo más claro y fácil es **no usar `-m` y escribir todo el mensaje en el editor** que se abre automáticamente con `git commit`.

La convención de Conventional Commits espera que haya una **línea en blanco** entre el cuerpo del mensaje y el pie de página, algo que es más sencillo de gestionar en un editor de texto.


