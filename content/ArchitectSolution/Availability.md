---
title: "Availability"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Non-Functional Requirements]]"
related:
  - "[[Reliability]]"
  - "[[Resilience]]"
  - "[[Scalability]]"
tags:
  - solution-architecture
  - atributo-calidad
---

# Availability

## ¿Qué es?
La disponibilidad es la proporción de tiempo en que un sistema está operativo y responde a sus usuarios. Se suele expresar en porcentaje: "99.9% de disponibilidad" significa que puede estar caído como máximo unas 8.7 horas al año.

**Definición técnica:** atributo de calidad que mide el porcentaje de tiempo en que un sistema está en condiciones de prestar servicio, típicamente expresado en "nueves" (99.9%, 99.99%) y formalizado en acuerdos de nivel de servicio (SLA).

---

## ¿Por qué existe?
Un sistema caído no genera valor y erosiona la confianza. Cuanto más crítico es el servicio (pagos, salud), más caro es cada minuto de caída. La disponibilidad existe para cuantificar y comprometer cuánto tiempo debe estar operativo un sistema.

---

## ¿Qué problema resuelve?
- Pérdidas por caídas del servicio.
- Falta de un criterio claro y medible sobre "cuánto tiempo debe estar arriba".
- Expectativas mal alineadas entre proveedor y cliente (de ahí los SLA).

---

## ¿Cómo funciona?
Se mejora con **redundancia** (varias instancias para que si una cae otra siga), **balanceo de carga**, y eliminando **puntos únicos de fallo**. Cada "nueve" adicional cuesta bastante más y suele estar en conflicto con otros atributos ([[Trade-offs]]). Se apoya en [[Scalability]] y [[Resilience]], y se mide con [[Observability]].

---

## Ejemplo sencillo
Es como una tienda: la disponibilidad es cuántas horas está abierta y atendiendo. Tener varias cajas (redundancia) evita que una avería cierre toda la tienda. Prometer "abierto 24/7" (muchos nueves) exige mucha más inversión que "de 9 a 18".

---

## Conceptos relacionados
- [[Reliability]] — relacionada pero distinta: fiabilidad es hacer las cosas bien; disponibilidad es estar operativo.
- [[Resilience]] — la capacidad de recuperarse de fallos sostiene la disponibilidad.
- [[Scalability]] — escalar ayuda a mantenerse disponible bajo carga.

---

## Antes de estudiar esto
- [[Non-Functional Requirements]]

---

## Después de estudiar esto
- [[Reliability]]
- [[Resilience]]

---

## Preguntas de comprobación
1. ¿Qué significa "99.9% de disponibilidad" en tiempo de caída real?
2. ¿Cómo ayuda la redundancia a la disponibilidad?
3. ¿Qué es un punto único de fallo?
4. ¿Por qué cada "nueve" adicional es cada vez más caro?

---

## Errores comunes
- Confundir disponibilidad (estar operativo) con fiabilidad (funcionar correctamente).
- Prometer más nueves de los que la arquitectura puede sostener.
- Ignorar los puntos únicos de fallo hasta que uno provoca la caída.

---

## Resumen
- Mide el porcentaje de tiempo operativo de un sistema.
- Se expresa en "nueves" y se formaliza en SLA.
- Se mejora con redundancia y eliminación de puntos únicos de fallo.
- Cada nueve adicional es más caro.
- Se relaciona con fiabilidad, resiliencia y escalabilidad.

---

## Fuentes
- Google — *SRE Book: Availability*: https://sre.google/sre-book/availability-table/
- AWS — *Well-Architected: Reliability Pillar*: https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/welcome.html
