---
title: "Resilience"
type: "concept"
area: "Solution Architecture"
level: 5
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Distributed Systems]]"
  - "[[Availability]]"
related:
  - "[[Reliability]]"
  - "[[Messaging]]"
  - "[[Cloud Architecture]]"
tags:
  - solution-architecture
  - atributo-calidad
---

# Resilience

## ¿Qué es?
La resiliencia es la capacidad de un sistema para seguir funcionando (aunque sea de forma degradada) y recuperarse cuando algo falla. No busca evitar todos los fallos (imposible), sino que el sistema los soporte con gracia.

**Definición técnica:** atributo de calidad que describe la capacidad de un sistema de anticipar, absorber, adaptarse y recuperarse ante fallos y condiciones adversas, manteniendo un nivel de servicio aceptable.

---

## ¿Por qué existe?
En [[Distributed Systems]] los fallos son inevitables: redes que caen, servicios lentos, picos de carga. Diseñar para que "nunca falle" es ilusorio. La resiliencia existe para asumir el fallo como algo normal y diseñar el sistema para sobrevivirlo.

---

## ¿Qué problema resuelve?
- Fallos en cascada donde un componente arrastra a todo el sistema.
- Caídas totales ante problemas que podrían haberse contenido.
- Recuperación lenta o manual tras un incidente.

---

## ¿Cómo funciona?
Usa patrones concretos:
- **Reintentos** con espera para fallos transitorios.
- **Circuit breaker**: dejar de llamar a un servicio que falla para no empeorar.
- **Timeouts** para no quedar esperando indefinidamente.
- **Bulkheads**: aislar recursos para que un fallo no contamine el resto.
- **Degradación elegante**: ofrecer funcionalidad reducida en lugar de caer del todo.

La [[Messaging]] asíncrona y la redundancia refuerzan la resiliencia.

---

## Ejemplo sencillo
Un barco resiliente tiene compartimentos estancos (bulkheads): si uno se inunda, el resto sigue a flote. No evita todas las fugas, pero evita que una hunda todo el barco.

---

## Conceptos relacionados
- [[Distributed Systems]] — donde los fallos parciales hacen la resiliencia indispensable.
- [[Availability]] — recuperarse rápido sostiene la disponibilidad.
- [[Reliability]] — tolerar fallos contribuye a un comportamiento fiable.
- [[Messaging]] — desacopla componentes y absorbe picos.

---

## Antes de estudiar esto
- [[Distributed Systems]]
- [[Availability]]

---

## Después de estudiar esto
- [[Cloud Architecture]]

---

## Preguntas de comprobación
1. ¿Por qué en sistemas distribuidos se asume que los fallos ocurrirán?
2. ¿Qué hace un patrón circuit breaker?
3. ¿Qué es la degradación elegante?
4. ¿Cómo ayuda la mensajería asíncrona a la resiliencia?

---

## Errores comunes
- Reintentar sin límite y provocar una "tormenta de reintentos" que empeora el fallo.
- No poner timeouts y quedar bloqueado esperando a un servicio caído.
- Diseñar como si la red y las dependencias nunca fallaran.

---

## Resumen
- Es la capacidad de soportar fallos y recuperarse.
- Asume el fallo como algo normal, no como excepción.
- Usa patrones: reintentos, circuit breaker, timeouts, bulkheads, degradación.
- Es esencial en sistemas distribuidos.
- Sostiene la disponibilidad y la fiabilidad.

---

## Fuentes
- Microsoft — *Azure Architecture Center: Resiliency patterns*: https://learn.microsoft.com/en-us/azure/architecture/patterns/category/resiliency
- AWS — *Well-Architected: Reliability Pillar*: https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/welcome.html
