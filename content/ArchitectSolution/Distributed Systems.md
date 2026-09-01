---
title: "Distributed Systems"
type: "concept"
area: "Solution Architecture"
level: 5
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Microservices]]"
  - "[[System Integration]]"
related:
  - "[[Scalability]]"
  - "[[Resilience]]"
  - "[[Cloud Architecture]]"
  - "[[Messaging]]"
tags:
  - solution-architecture
  - distribuido
---

# Distributed Systems

## ¿Qué es?
Un sistema distribuido es aquel cuyas partes viven en varias máquinas conectadas por una red y colaboran para funcionar como un solo sistema. La mayoría de aplicaciones modernas a escala (banca, streaming, redes sociales) son sistemas distribuidos.

**Definición técnica:** conjunto de componentes independientes ubicados en nodos conectados por red que se coordinan mediante paso de mensajes para presentar al usuario un servicio coherente, enfrentando fallos parciales, latencia y ausencia de reloj global.

---

## ¿Por qué existe?
Una sola máquina tiene límites de capacidad y es un punto único de fallo. Distribuir el trabajo permite escalar más allá de una máquina y seguir funcionando aunque algunas fallen. Existe para lograr escala y tolerancia a fallos.

---

## ¿Qué problema resuelve?
- Superar el límite de capacidad de una sola máquina ([[Scalability]]).
- Evitar que un único fallo tumbe todo el sistema ([[Resilience]]).
- Servir a usuarios en distintas regiones con menor latencia.

---

## ¿Cómo funciona?
Los nodos se comunican por red, lo que introduce retos que no existen en un solo proceso: la red puede fallar, los mensajes se pierden o llegan desordenados, y no hay un reloj compartido. Conceptos clave son el **teorema CAP** (consistencia, disponibilidad y tolerancia a particiones: no se pueden garantizar las tres a la vez ante una partición) y la **consistencia eventual**. La [[Observability]] y la mensajería ([[Messaging]]) son esenciales.

---

## Ejemplo sencillo
Es como organizar un evento con equipos en varias ciudades comunicándose solo por mensajes. Si una ciudad se queda sin señal (partición de red), debes decidir: ¿esperas a que responda (consistencia) o sigues sin ella (disponibilidad)? No puedes tener ambas perfectas a la vez.

---

## Conceptos relacionados
- [[Microservices]] — un caso concreto de sistema distribuido.
- [[Scalability]] — la distribución es un medio clave para escalar.
- [[Resilience]] — los sistemas distribuidos deben tolerar fallos parciales.
- [[Cloud Architecture]] — la nube es el entorno natural para construirlos.

---

## Antes de estudiar esto
- [[Microservices]]
- [[System Integration]]

---

## Después de estudiar esto
- [[Cloud Architecture]]
- [[Resilience]]

---

## Preguntas de comprobación
1. ¿Qué hace "distribuido" a un sistema?
2. ¿Qué afirma el teorema CAP y por qué obliga a hacer trade-offs?
3. ¿Qué es un "fallo parcial" y por qué es tan difícil de manejar?
4. ¿Qué significa consistencia eventual?

---

## Errores comunes
- Asumir que la red es fiable, instantánea y sin límites (las "falacias de la computación distribuida").
- Querer consistencia fuerte y disponibilidad total a la vez sin entender el CAP.
- Distribuir un sistema que un monolito resolvería mejor.

---

## Resumen
- Sus partes viven en varias máquinas conectadas por red.
- Existen para escalar y tolerar fallos.
- Enfrentan fallos parciales, latencia y falta de reloj global.
- El teorema CAP impone trade-offs entre consistencia y disponibilidad.
- Son la base de las aplicaciones modernas a gran escala.

---

## Fuentes
- Martin Kleppmann — *Designing Data-Intensive Applications* (O'Reilly, 2017), ISBN 978-1449373320.
- Google — *SRE Book*: https://sre.google/sre-book/table-of-contents/
- Microsoft — *Azure Architecture Center: Distributed systems*: https://learn.microsoft.com/en-us/azure/architecture/guide/
