---
title: "Non-Functional Requirements"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Software Architecture]]"
related:
  - "[[Scalability]]"
  - "[[Availability]]"
  - "[[Reliability]]"
  - "[[Trade-offs]]"
tags:
  - solution-architecture
  - requisitos
---

# Non-Functional Requirements

## ¿Qué es?
Los requisitos no funcionales describen *cómo* debe comportarse un sistema, no *qué* hace. Mientras un requisito funcional dice "el usuario puede pagar", uno no funcional dice "el pago debe completarse en menos de 2 segundos y estar disponible el 99.9% del tiempo".

**Definición técnica:** también llamados *atributos de calidad*, son restricciones y criterios sobre el comportamiento del sistema (rendimiento, escalabilidad, disponibilidad, seguridad, mantenibilidad) que condicionan las decisiones de arquitectura.

---

## ¿Por qué existe?
Un sistema puede cumplir todo lo que hace (funcional) y aun así ser inservible: lento, caído o inseguro. Los requisitos no funcionales existen para definir de forma explícita las cualidades que hacen que el sistema sea usable en el mundo real.

---

## ¿Qué problema resuelve?
- Sistemas que funcionan en pruebas pero fallan bajo carga real.
- Expectativas implícitas ("debe ser rápido") que nadie definió ni midió.
- Decisiones de arquitectura sin criterios claros para justificarlas.

---

## ¿Cómo funciona?
Se expresan de forma medible: latencia (ms), disponibilidad (%), throughput (peticiones/seg), tiempo de recuperación. Guían directamente las decisiones de [[Software Architecture]] y suelen entrar en conflicto entre sí, obligando a [[Trade-offs]] (ej. más seguridad puede reducir rendimiento). Incluyen atributos como [[Scalability]], [[Availability]], [[Reliability]] y seguridad.

---

## Ejemplo sencillo
Al comprar un coche, lo funcional es "que transporte personas". Lo no funcional es "que consuma poco, sea seguro, alcance cierta velocidad y no se averíe". Dos coches cumplen la función, pero sus cualidades los hacen muy distintos.

---

## Conceptos relacionados
- [[Software Architecture]] — la arquitectura existe en gran parte para satisfacerlos.
- [[Scalability]], [[Availability]], [[Reliability]] — son atributos no funcionales concretos.
- [[Trade-offs]] — casi siempre hay que equilibrarlos entre sí.

---

## Antes de estudiar esto
- [[Software Architecture]]

---

## Después de estudiar esto
- [[Scalability]]
- [[Availability]]
- [[Trade-offs]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre un requisito funcional y uno no funcional?
2. ¿Por qué deben ser medibles?
3. Da un ejemplo de dos requisitos no funcionales en conflicto.
4. ¿Cómo influyen en las decisiones de arquitectura?

---

## Errores comunes
- Definirlos de forma vaga ("rápido", "seguro") sin métricas.
- Descubrirlos tarde, cuando la arquitectura ya no los soporta.
- Ignorar que unos compiten con otros y exigen trade-offs.

---

## Resumen
- Describen cómo debe comportarse el sistema, no qué hace.
- Incluyen rendimiento, escalabilidad, disponibilidad, seguridad, etc.
- Deben expresarse de forma medible.
- Guían las decisiones de arquitectura.
- Suelen estar en conflicto y exigen trade-offs.

---

## Fuentes
- ISO/IEC — *25010: Systems and software Quality Requirements*: https://iso25000.com/index.php/en/iso-25000-standards/iso-25010
- Microsoft — *Azure Architecture Center: Quality attributes*: https://learn.microsoft.com/en-us/azure/architecture/guide/design-principles/
