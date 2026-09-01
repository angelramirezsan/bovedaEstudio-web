---
title: "Reliability"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Non-Functional Requirements]]"
related:
  - "[[Availability]]"
  - "[[Resilience]]"
  - "[[Observability]]"
tags:
  - solution-architecture
  - atributo-calidad
---

# Reliability

## ¿Qué es?
La fiabilidad es la capacidad de un sistema de funcionar correctamente y sin errores durante un periodo, en las condiciones esperadas. Un sistema fiable hace lo que promete, de forma consistente, incluso cuando algo va mal alrededor.

**Definición técnica:** atributo de calidad que expresa la probabilidad de que un sistema opere sin fallos durante un intervalo dado bajo condiciones definidas. Se mide con indicadores como MTBF (tiempo medio entre fallos) y tasa de errores.

---

## ¿Por qué existe?
Un sistema que a veces da resultados incorrectos o falla de forma impredecible no es confiable, aunque esté "disponible". La fiabilidad existe para asegurar que el comportamiento sea correcto y predecible, no solo que el servicio esté encendido.

---

## ¿Qué problema resuelve?
- Resultados incorrectos o inconsistentes que erosionan la confianza.
- Fallos impredecibles difíciles de anticipar.
- Falta de una medida objetiva de "qué tan confiable es el sistema".

---

## ¿Cómo funciona?
Se logra con [[Testing]] riguroso, manejo correcto de errores, redundancia y [[Observability]] para detectar problemas pronto. Está muy ligada a la [[Availability]] y a la [[Resilience]], pero es distinta: un sistema puede estar disponible (encendido) y aun así ser poco fiable (dando errores). Se apoya en prácticas de ingeniería de fiabilidad (SRE).

---

## Ejemplo sencillo
Un coche fiable arranca siempre y te lleva sin averías inesperadas. Uno que arranca (disponible) pero se apaga a mitad del viaje no es fiable. La diferencia es hacer bien la tarea de forma consistente, no solo estar encendido.

---

## Conceptos relacionados
- [[Availability]] — estar operativo; la fiabilidad es funcionar correctamente mientras lo está.
- [[Resilience]] — recuperarse de fallos ayuda a sostener la fiabilidad.
- [[Observability]] — permite medir errores y detectar degradación.

---

## Antes de estudiar esto
- [[Non-Functional Requirements]]

---

## Después de estudiar esto
- [[Resilience]]
- [[Observability]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre fiabilidad y disponibilidad?
2. ¿Por qué un sistema disponible puede no ser fiable?
3. ¿Qué mide el MTBF?
4. ¿Cómo contribuyen las pruebas y la observabilidad a la fiabilidad?

---

## Errores comunes
- Usar "fiabilidad" y "disponibilidad" como sinónimos.
- Medir solo si el sistema está encendido, no si responde correctamente.
- No instrumentar el sistema para detectar errores silenciosos.

---

## Resumen
- Es funcionar correctamente y de forma consistente durante un periodo.
- Distinta de la disponibilidad (estar operativo).
- Se mide con MTBF y tasa de errores.
- Se logra con pruebas, manejo de errores y observabilidad.
- Es un pilar de la ingeniería de fiabilidad (SRE).

---

## Fuentes
- Google — *Site Reliability Engineering Book*: https://sre.google/sre-book/table-of-contents/
- AWS — *Well-Architected: Reliability Pillar*: https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/welcome.html
