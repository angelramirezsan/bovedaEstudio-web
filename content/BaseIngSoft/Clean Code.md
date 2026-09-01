---
title: "Clean Code"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Software Design]]"
related:
  - "[[Design Patterns]]"
  - "[[Testing]]"
  - "[[Documentation]]"
tags:
  - software-engineering
  - calidad
---

# Clean Code

## ¿Qué es?
Clean Code ("código limpio") es la práctica de escribir código que otras personas (y tú en el futuro) puedan leer y entender con facilidad. No se trata de que funcione, sino de que sea claro.

**Definición técnica:** conjunto de prácticas para escribir código legible, expresivo y mantenible: nombres significativos, funciones pequeñas con una sola responsabilidad, evitar duplicación (DRY) y minimizar la complejidad. El término se popularizó con el libro de Robert C. Martin.

---

## ¿Por qué existe?
El código se lee muchas más veces de las que se escribe. Código confuso ralentiza a todo el equipo y multiplica los errores. Clean Code existe para reducir el costo de leer, entender y cambiar el software.

---

## ¿Qué problema resuelve?
- Código que solo entiende quien lo escribió (y a veces ni él).
- Cambios lentos y arriesgados por falta de claridad.
- Errores que se esconden en la complejidad innecesaria.

---

## ¿Cómo funciona?
Se apoya en hábitos concretos: nombres que revelan intención, funciones cortas que hacen una sola cosa, evitar duplicación (**DRY**), minimizar dependencias y comentar el *por qué* (no el *qué*). Es una práctica, no una regla rígida: el juicio importa.

---

## Ejemplo sencillo
Es como escribir instrucciones para un compañero. "Haz eso con la cosa de antes" es confuso; "calcula el total sumando el precio de cada producto" es claro. El código limpio se lee casi como prosa.

---

## Conceptos relacionados
- [[Software Design]] — el código limpio materializa un buen diseño.
- [[Design Patterns]] — patrones bien aplicados aumentan la claridad.
- [[Testing]] — el código limpio es más fácil de probar.

---

## Antes de estudiar esto
- [[Software Design]]

---

## Después de estudiar esto
- [[Design Patterns]]
- [[Documentation]]

---

## Preguntas de comprobación
1. ¿Por qué la legibilidad importa más que la brevedad?
2. ¿Qué significa el principio DRY?
3. ¿Por qué un comentario debería explicar el "por qué" y no el "qué"?
4. ¿Cómo se relaciona el código limpio con la facilidad de hacer pruebas?

---

## Errores comunes
- Confundir "clean code" con "código corto o astuto"; a veces lo claro es más largo.
- Comentar lo obvio en lugar de mejorar el nombre de la variable.
- Aplicar reglas al pie de la letra sin criterio contextual.

---

## Resumen
- Clean Code busca legibilidad y mantenibilidad.
- El código se lee más veces de las que se escribe.
- Nombres claros, funciones pequeñas, sin duplicación.
- Es una práctica basada en juicio, no en reglas rígidas.
- Reduce el costo de cambiar el software.

---

## Fuentes
- Robert C. Martin — *Clean Code* (Prentice Hall, 2008), ISBN 978-0132350884.
- Martin Fowler — *Refactoring*: https://refactoring.com/
