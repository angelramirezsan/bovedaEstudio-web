---
title: "Trade-offs"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Non-Functional Requirements]]"
related:
  - "[[Architecture Decision Records]]"
  - "[[Solution Architecture]]"
  - "[[Scalability]]"
tags:
  - solution-architecture
  - decisiones
---

# Trade-offs

## ¿Qué es?
Un trade-off es un compromiso: mejorar algo a costa de empeorar otra cosa. En arquitectura casi ninguna decisión es "buena o mala" en absoluto; es "mejor para X, peor para Y". Diseñar es elegir qué priorizar.

**Definición técnica:** situación de decisión en la que optimizar un atributo (rendimiento, costo, simplicidad, seguridad) implica sacrificar otro, obligando a priorizar según los [[Non-Functional Requirements]] y el contexto del negocio.

---

## ¿Por qué existe?
No existe la solución perfecta: los recursos, el tiempo y las leyes de la ingeniería imponen límites. Reconocer los trade-offs existe para tomar decisiones conscientes en vez de buscar una imposible "mejor opción absoluta".

---

## ¿Qué problema resuelve?
- La ilusión de que hay una solución óptima para todo.
- Decisiones tomadas sin ver lo que se está sacrificando.
- Discusiones sin fin por no reconocer que se está eligiendo entre compromisos.

---

## ¿Cómo funciona?
Ante una decisión, se identifican los atributos en conflicto y se prioriza según los objetivos. Ejemplos clásicos: consistencia vs. disponibilidad (teorema CAP en [[Distributed Systems]]), rendimiento vs. seguridad, simplicidad vs. flexibilidad, costo vs. tiempo. El razonamiento se registra en un [[Architecture Decision Records]]. La clave es hacer explícito lo que se gana y lo que se pierde.

---

## Ejemplo sencillo
Al elegir un medio de transporte: el avión es rápido pero caro; el autobús es barato pero lento. No hay uno "mejor" en absoluto; depende de si priorizas tiempo o dinero. Toda decisión de arquitectura tiene esta forma.

---

## Conceptos relacionados
- [[Non-Functional Requirements]] — los atributos que suelen entrar en conflicto.
- [[Architecture Decision Records]] — donde se documenta el trade-off elegido.
- [[Scalability]] — a menudo se equilibra frente a costo o simplicidad.
- [[Solution Architecture]] — gestionar trade-offs es la esencia del rol de arquitecto.

---

## Antes de estudiar esto
- [[Non-Functional Requirements]]

---

## Después de estudiar esto
- [[Architecture Decision Records]]
- [[Solution Architecture]]

---

## Preguntas de comprobación
1. ¿Por qué casi ninguna decisión de arquitectura es "buena o mala" en absoluto?
2. Da un ejemplo de dos atributos que suelan entrar en conflicto.
3. ¿Cómo ayuda hacer explícito un trade-off?
4. ¿Dónde se documenta el razonamiento de un trade-off?

---

## Errores comunes
- Buscar la "mejor solución" ignorando que todo implica compromisos.
- Optimizar un atributo sin notar el que se está degradando.
- No documentar por qué se aceptó un trade-off concreto.

---

## Resumen
- Un trade-off es mejorar algo a costa de otra cosa.
- En arquitectura no hay óptimo absoluto, sino priorización.
- Se prioriza según los requisitos no funcionales y el negocio.
- El razonamiento se documenta en un ADR.
- Gestionarlos bien es la esencia del rol de arquitecto.

---

## Fuentes
- Bass, Clements, Kazman — *Software Architecture in Practice* (Addison-Wesley), ISBN 978-0136886099.
- Neal Ford & Mark Richards — *Fundamentals of Software Architecture* (O'Reilly, 2020), ISBN 978-1492043454.
