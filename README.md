# Proyecto final de Principios de Programación

Cada algoritmo debe implementarse tanto en **Perl** como en **C** (ojo: **NO** en C++). Deben emplear variables con nombres significativos e incluir comentarios (documentación interna) que expliquen la lógica empleada por su programa. También deberán incluir un breve diccionario de datos en su programa, describiendo cómo se emplea cada variable y qué significa. La revisión será mediante presentaciones de sus proyectos en el salón de clase. El orden de las evaluaciones se informará más adelante.

## Instrucciones para la entrega

1. Formato de archivos:

   - Cada algoritmo debe nombrarse siguiendo EXACTAMENTE este formato:
     ```
     0{número_de_algoritmo}_{nombre_del_algoritmo}.{extensión}
     ```
   - Ejemplos:
     - Para el problema 1:
       - `01_el_lenguaje_secreto_de_las_tortugas.pl`
       - `01_el_lenguaje_secreto_de_las_tortugas.c`

2. Estructura de carpetas:

   - Crear DOS carpetas con los siguientes nombres exactos:
     - `Perl`: Contendrá todos los archivos .pl
     - `C`: Contendrá todos los archivos .c

   Estructura esperada:

   ```
   proyecto/
   ├── C/
   │   ├── 01_el_lenguaje_secreto_de_las_tortugas.c
   │   └── 02_otro_problema.c
   └── Perl/
       ├── 01_el_lenguaje_secreto_de_las_tortugas.pl
       └── 02_otro_problema.pl
   ```

3. Archivo comprimido:

   - Todas las carpetas deben comprimirse en un único archivo ZIP
   - El archivo ZIP debe nombrarse siguiendo EXACTAMENTE este formato:
     ```
     {número_de_lista}_{apellido_1}_{apellido_2}_{nombre_1}_proyecto.zip
     ```
   - Para el número de lista:
     - Números menores a 10: usar 0 inicial (01, 02, ..., 09)
     - Números mayores a 9: escribir normalmente (10, 11, ...)
   - Ejemplos:
     - Si eres el número 01 de la lista: `01_velez_santiago_jesus_proyecto.zip`
     - Si eres el número 15 de la lista: `15_velez_santiago_jesus_proyecto.zip`

4. Envío:
   - El archivo ZIP debe enviarse por correo electrónico a mi correo (dado en clase)
   - El asunto del correo debe ser el mismo nombre del archivo ZIP sin la extensión
   - Ejemplos del asunto:
     - `01_velez_santiago_jesus_proyecto`
     - `15_velez_santiago_jesus_proyecto`
   - La entrega por correo es obligatoria y debe realizarse ANTES de la revisión presencial

Errores comunes a evitar:

- Usar espacios en lugar de guiones bajos
- Olvidar incluir el "0" en números menores a 10
- Usar mayúsculas incorrectamente en los nombres de carpetas
- Enviar archivos sueltos en lugar de la estructura de carpetas requerida
- Incluir caracteres especiales o acentos en los nombres de archivos
- Olvidar quitar la extensión .zip en el asunto del correo

Lista de verificación:

```
□ Nombres de algoritmos con formato correcto.
□ Archivos .pl en carpeta "Perl"
□ Archivos .c en carpeta "C"
□ Estructura de carpetas correcta
□ Archivo ZIP nombrado correctamente
□ Asunto del correo sin la extensión .zip
□ Entrega realizada antes de la revisión presencial
```

Importante:

- El incumplimiento de cualquiera de estas instrucciones resultará en una penalización sobre la calificación total del proyecto.
- Revisa cuidadosamente los nombres de archivos y carpetas antes de enviar, prestando especial atención a mayúsculas, minúsculas y guiones bajos.

## Problemas

1. **El lenguaje secreto de las tortugas:**

   Las tortugas marinas tienen un sistema de comunicación que los humanos aún no entendemos del todo. Imagina que han descubierto que las tortugas se comunican mediante una secuencia de 16 señales que pueden ser "0" o "1". Cada señal es introducida por un investigador desde el teclado. Esta secuencia representa un mensaje binario que debe ser convertido a decimal para entender su significado en términos de estudios científicos.

   **Parte a:**

   Desarrolla un algoritmo que convierta esta secuencia binaria de las tortugas, representada por un arreglo de 16 elementos, en su equivalente decimal y lo imprima. **Restricción:** Para el cálculo de cada potencia de 2 no es posible utilizar ningún operador aritmético (`+`, `-`, `*`, `/`, `%`), ni de incremento o decremento (`++`, `--`), ni operadores o funciones para elevar a algún exponente o para calcular raíces, ni funciones matemáticas logarítmicas o trigonométricas (es decir, deben usar corrimientos de bits).

   **Parte b:**

   Los investigadores desean enviar un mensaje a las tortugas. Debes desarrollar un algoritmo que lea un número decimal desde el teclado (el mensaje humano) y lo convierta en su equivalente binario, almacenándolo en un arreglo de 16 elementos como en el caso anterior. Luego, el algoritmo debe recorrer el arreglo para imprimir la secuencia binaria que será enviada a las tortugas.

2. **El inventario del zoológico:**

   Un zoológico tiene dos listas de animales: la lista **A** contiene los animales del sector terrestre y la lista **B** contiene los animales del sector acuático. Cada lista puede tener un número diferente de animales. Los administradores del zoológico necesitan analizar la diversidad y superposición de especies entre ambos sectores.

   Desarrolla un algoritmo que lea ambas listas desde el teclado e imprima:

   - **La unión** de ambas listas (todos los animales presentes en el zoológico sin repetir).
   - **La intersección** de ambas listas (animales que pueden vivir tanto en tierra como en agua, como los cocodrilos).
   - **Las diferencias simétrica y asimétrica** de ambos conjuntos (para identificar especies únicas de cada sector y posibles reasignaciones).

   **Nota:** Para este programa, emplea la técnica de codificación en números binarios vista en clase, con las funciones de codificación y decodificación, y utiliza operadores sobre bits para manejar los conjuntos.

3. **Clasificación de hábitats extremos:**

   En un estudio sobre las altitudes y profundidades a las que diferentes especies de animales pueden vivir, los científicos han recopilado **N** (N ≤ 10,000) registros donde cada número representa una altitud en metros, en el rango de **-20,000 hasta 20,000** metros (desde las profundidades oceánicas hasta las alturas de la atmósfera). Necesitan ordenar estos datos en forma ascendente para analizar la distribución de especies según la altitud.

   Diseña un algoritmo que lea este conjunto de datos desde el teclado, ordene las altitudes utilizando el **Método de Burbuja**, y las imprima en pantalla.

4. **El contador de huevos de la gallina sabia:**

   Una gallina ha puesto un número **N** de huevos (positivo, entero, máximo seis cifras) y quiere informar al granjero cuántos huevos ha puesto, pero en palabras para mayor claridad.

   Diseña un algoritmo que lea el número **N** desde el teclado y lo imprima en palabras. Por ejemplo, si la gallina puso `645376` huevos, el programa debe imprimir:

   ```
   seiscientos cuarenta y cinco mil trescientos setenta y seis
   ```

5. **Búsqueda del ave migratoria perdida:**

   En un estudio de aves migratorias, cada ave está identificada con un número **N** que representa su posición en una escala de altitud que va desde **-20,000 hasta 20,000** metros (considerando aves que vuelan a gran altura y otras que se sumergen en aguas profundas). Los observadores han registrado **M** (M ≤ 10,000) posiciones de aves, ordenadas en forma ascendente.

   Diseña un algoritmo que lea el número **N** (posición altitudinal del ave perdida) y luego lea el conjunto ordenado de **M** posiciones desde el teclado. El algoritmo debe ubicar en qué posición (de 0 a M-1) se encuentra el ave **N** e imprimir en pantalla dicha posición. Si el ave no existe en el conjunto, se debe informar al usuario con un mensaje adecuado.

   **Importante:** El algoritmo debe ser eficiente y no recorrer todo el arreglo; utiliza **Búsqueda Binaria** para encontrar al ave rápidamente.

6. **Búsqueda recursiva en el ecosistema subterráneo:**

   En un ecosistema subterráneo, se monitorean diferentes colonias de animales que viven en profundidades que van desde **-20,000 hasta 20,000** metros (considerando niveles subterráneos y sobre la superficie). Cada colonia está identificada por un número **N** que representa su profundidad o altura en metros.

   Realiza un programa **recursivo** que implemente la **Búsqueda Binaria** para encontrar la posición de una colonia específica **N** dentro de un conjunto de **M** colonias (M ≤ 10,000) cuyas profundidades están ordenadas en forma ascendente, de acuerdo con las condiciones del problema anterior.

7. **La red social de las abejas:**

   Las abejas en una colmena tienen una compleja red de comunicación. Cada abeja se conecta con otras mediante "danzas" que representan conexiones en una red no dirigida.

   Desarrolla un algoritmo que lea desde el teclado una lista de conexiones entre abejas (nodos) y genere una matriz que represente dicha red. Posteriormente, el algoritmo debe calcular e imprimir en pantalla para cada abeja:

   - **El número de la abeja** (nodo).
   - **Su grado** (número de conexiones con otras abejas).
   - **Su coeficiente de clustering** (probabilidad de que dos abejas conectadas a una tercera estén conectadas entre sí), lo cual es importante para entender la eficiencia en la comunicación dentro de la colmena.

---

**Nota:** Recuerden utilizar nombres de variables significativos y agregar comentarios que expliquen la lógica del programa. Incluyan un diccionario de datos que describa cómo se emplea cada variable y qué significa.

---

{{< pagebreak >}}

## Ejemplo solución de un problema

### Calculando el total de patas en una reserva de animales

En una reserva natural, hay dos tipos de animales: **avestruces** y **elefantes**. Cada avestruz tiene **2** patas, y cada elefante tiene **4** patas. Los cuidadores necesitan saber el **número total de patas** en la reserva para planificar la distribución del espacio y recursos.

**Objetivo:**

- Escribe un programa que lea desde el teclado el número de avestruces y el número de elefantes en la reserva.
- Calcula e imprime el número total de patas que hay en la reserva.

---

### Solución en **Perl**

```perl
#!/usr/bin/perl
use strict;
use warnings;

=begin
Data Dictionary:
- $legs_per_ostrich: Number of legs per ostrich (constant, value 2).
- $legs_per_elephant: Number of legs per elephant (constant, value 4).
- $num_ostriches: Stores the number of ostriches entered by the user.
- $num_elephants: Stores the number of elephants entered by the user.
- $total_legs: Result of calculating the total number of legs in the reserve.
=cut

# Constants representing the number of legs per animal
my $legs_per_ostrich = 2;
my $legs_per_elephant = 4;

print "Ingrese el número de avestruces: ";
my $num_ostriches = <STDIN>;
chomp($num_ostriches);

print "Ingrese el número de elefantes: ";
my $num_elephants = <STDIN>;
chomp($num_elephants);

# Calculate the total legs to assist in resource planning
my $total_legs = ($num_ostriches * $legs_per_ostrich) + ($num_elephants * $legs_per_elephant);

# Provide the total number of legs to help caretakers with their planning
print "El número total de patas en la reserva es: $total_legs\n";
```

---

### Solución en **C**

```c
#include <stdio.h>

/*
Data Dictionary:
- LEGS_PER_OSTRICH: Number of legs per ostrich (constant, value 2).
- LEGS_PER_ELEPHANT: Number of legs per elephant (constant, value 4).
- num_ostriches: Variable that stores the number of ostriches entered by the user.
- num_elephants: Variable that stores the number of elephants entered by the user.
- total_legs: Variable that stores the result of calculating the total number of legs in the reserve.
*/

#define LEGS_PER_OSTRICH 2
#define LEGS_PER_ELEPHANT 4

int main() {
    int num_ostriches, num_elephants, total_legs;

    printf("Ingrese el número de avestruces: ");
    scanf("%d", &num_ostriches);

    printf("Ingrese el número de elefantes: ");
    scanf("%d", &num_elephants);

    // Calculate the total legs to assist in resource planning
    total_legs = (num_ostriches * LEGS_PER_OSTRICH) + (num_elephants * LEGS_PER_ELEPHANT);

    // Provide the total number of legs to help caretakers with their planning
    printf("El número total de patas en la reserva es: %d\n", total_legs);

    return 0;
}
```
