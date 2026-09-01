---
title: "Software Design"
type: "concept"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Programming Languages]]"
  - "[[Data Structures and Algorithms]]"
related:
  - "[[Clean Code]]"
  - "[[Design Patterns]]"
  - "[[Software Architecture]]"
tags:
  - software-engineering
  - diseno
---

# Software Design

## ¿Qué es?
El diseño de software es decidir cómo se organiza el código por dentro: qué piezas existen, qué hace cada una y cómo se comunican. Es planear la estructura antes y durante la construcción para que el sistema sea entendible y modificable.

**Definición técnica:** el diseño de software es la actividad de definir la estructura de componentes, sus responsabilidades, interfaces y relaciones, aplicando principios como cohesión alta, acoplamiento bajo, separación de responsabilidades y abstracción.

---

## ¿Por qué existe?
Un programa puede "funcionar" y aun así ser un caos imposible de mantener. Sin diseño, cada cambio se vuelve más costoso y arriesgado. El diseño existe para que el software pueda evolucionar sin colapsar.

---

## ¿Qué problema resuelve?
- Código enredado donde tocar una parte rompe otras.
- Dificultad para entender, extender y probar el sistema.
- Duplicación y responsabilidades mezcladas.

---

## ¿Cómo funciona?
Se apoya en principios: **separación de responsabilidades** (cada pieza hace una cosa), **bajo acoplamiento** (las piezas dependen poco entre sí), **alta cohesión** (lo relacionado va junto) y **abstracción** (ocultar detalles tras interfaces claras). Principios como **SOLID** guían el diseño orientado a objetos. El diseño es previo y más granular que la [[Software Architecture]].

---

## Ejemplo sencillo
Es como diseñar los planos de una casa: dónde van las habitaciones, cómo se conectan, dónde pasan las tuberías. Puedes construir sin planos, pero mover una pared después será mucho más caro que haberlo pensado antes.

---

## Conceptos relacionados
- [[Clean Code]] — el diseño se materializa en código legible.
- [[Design Patterns]] — soluciones de diseño probadas para problemas recurrentes.
- [[Software Architecture]] — el diseño opera a menor escala que la arquitectura.

---

## Antes de estudiar esto
- [[Programming Languages]]
- [[Data Structures and Algorithms]]

---

## Después de estudiar esto
- [[Clean Code]]
- [[Design Patterns]]
- [[Software Architecture]]

---

## Preguntas de comprobación
1. ¿Qué significan "alto acoplamiento" y "baja cohesión" y por qué son problemáticos?
2. ¿Por qué un programa que funciona puede tener mal diseño?
3. ¿Qué diferencia hay entre diseño y arquitectura de software?
4. ¿Qué busca la separación de responsabilidades?

---

## Errores comunes
- Confundir "que funcione" con "que esté bien diseñado".
- Sobre-diseñar: añadir abstracciones que nadie necesita todavía.
- Mezclar responsabilidades en una misma pieza (baja cohesión).

---

## Resumen
- El diseño define la estructura interna del software.
- Busca bajo acoplamiento, alta cohesión y separación de responsabilidades.
- Permite que el sistema evolucione con bajo costo.
- Es más granular que la arquitectura.
- Principios como SOLID lo guían.

---

## Fuentes
- Robert C. Martin — *Clean Architecture* (Prentice Hall, 2017), ISBN 978-0134494166.
- Microsoft — *Learn: Architecture and design principles*: https://learn.microsoft.com/en-us/azure/architecture/guide/design-principles/
