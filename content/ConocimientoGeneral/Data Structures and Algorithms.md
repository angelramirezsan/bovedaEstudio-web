---
title: "Data Structures and Algorithms"
type: "concept"
area: "Software Engineering"
level: 1
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[Software Design]]"
  - "[[Databases]]"
  - "[[Scalability]]"
tags:
  - fundamentos
---

# Data Structures and Algorithms

## ¿Qué es?
Son dos ideas que van de la mano. Una **estructura de datos** es una forma de organizar información para poder usarla eficientemente (por ejemplo, una lista, una tabla o un árbol). Un **algoritmo** es una serie de pasos bien definidos para resolver un problema (por ejemplo, ordenar esa lista o buscar un elemento).

**Definición técnica:** una estructura de datos es una organización de datos en memoria que define cómo se almacenan y acceden; un algoritmo es un procedimiento finito y determinista que transforma una entrada en una salida, analizable por su complejidad temporal y espacial.

---

## ¿Por qué existe?
La misma tarea puede ser instantánea o tardar horas según cómo organices los datos y qué pasos sigas. A medida que los sistemas crecen, la eficiencia deja de ser opcional. Estos conceptos existen para razonar sobre rendimiento antes de que un sistema falle bajo carga.

---

## ¿Qué problema resuelve?
- Elegir la representación de datos adecuada para cada operación (buscar, insertar, ordenar).
- Predecir cómo se comportará una solución cuando los datos crezcan.
- Comparar soluciones de forma objetiva mediante la notación Big-O.

---

## ¿Cómo funciona?
Cada estructura optimiza ciertas operaciones a costa de otras: un *array* accede por índice muy rápido pero inserta lento en medio; un *hash map* busca por clave casi instantáneo pero no mantiene orden. Los algoritmos se evalúan con la **notación Big-O** (ej. O(n), O(log n)), que describe cómo escala el costo al crecer la entrada, independientemente del hardware.

---

## Ejemplo sencillo
Buscar un contacto en una agenda desordenada te obliga a revisar página por página (lento). Si está ordenada alfabéticamente, abres por la mitad y descartas medio directorio en cada paso (búsqueda binaria, muy rápido). Misma tarea, distinta estructura y algoritmo, resultados incomparables.

---

## Conceptos relacionados
- [[Programming Languages]] — el lenguaje es el medio para implementar estructuras y algoritmos.
- [[Databases]] — internamente usan estructuras como índices (árboles B) para buscar rápido.
- [[Scalability]] — la eficiencia algorítmica es un factor directo de cómo escala un sistema.

---

## Antes de estudiar esto
- [[Programming Languages]]

---

## Después de estudiar esto
- [[Software Design]]
- [[Databases]]

---

## Preguntas de comprobación
1. ¿Por qué la elección de estructura de datos afecta el rendimiento?
2. ¿Qué describe la notación Big-O y qué NO describe?
3. ¿Por qué una búsqueda binaria es más rápida que una lineal?
4. Da un ejemplo donde un hash map sea mejor que una lista, y viceversa.

---

## Errores comunes
- Optimizar prematuramente sin medir dónde está el problema real.
- Confundir Big-O (cómo escala) con velocidad absoluta (depende del hardware).
- Elegir siempre la misma estructura por costumbre en lugar de por el patrón de acceso.

---

## Resumen
- Las estructuras de datos organizan la información; los algoritmos la procesan.
- La eficiencia depende de elegir la combinación adecuada al problema.
- Big-O permite comparar soluciones según cómo escalan.
- Cada estructura tiene ventajas y compromisos.
- Es la base para razonar sobre rendimiento y escalabilidad.

---

## Fuentes
- NIST — *Dictionary of Algorithms and Data Structures*: https://xlinux.nist.gov/dads/
- Python Software Foundation — *Data Structures*: https://docs.python.org/3/tutorial/datastructures.html
- MIT OpenCourseWare — *Introduction to Algorithms*: https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/
