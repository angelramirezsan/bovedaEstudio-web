---
title: "Observability"
type: "concept"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Debugging]]"
related:
  - "[[CI-CD]]"
  - "[[Reliability]]"
  - "[[Distributed Systems]]"
tags:
  - software-engineering
  - devops
  - operacion
---

# Observability

## ¿Qué es?
La observabilidad es la capacidad de entender qué está pasando dentro de un sistema en ejecución mirando lo que produce hacia afuera: registros, métricas y trazas. Es "ponerle sensores" al software para saber cómo se comporta en producción.

**Definición técnica:** la observabilidad es una propiedad de un sistema que permite inferir su estado interno a partir de sus salidas externas. Se sustenta en tres señales principales (los "tres pilares"): logs, métricas y trazas distribuidas.

---

## ¿Por qué existe?
En sistemas reales, y especialmente en [[Distributed Systems]], los fallos son complejos y no reproducibles en local. La observabilidad existe para diagnosticar problemas en producción y entender el comportamiento real bajo carga.

---

## ¿Qué problema resuelve?
- Fallos que solo ocurren en producción y no se pueden reproducir.
- No saber si el sistema está sano hasta que un usuario se queja.
- Diagnóstico lento en sistemas con muchas piezas interconectadas.

---

## ¿Cómo funciona?
Se apoya en tres señales:
- **Logs**: registros de eventos concretos ("el pago X falló a las 10:03").
- **Métricas**: valores numéricos agregados en el tiempo (latencia, tasa de errores, uso de CPU).
- **Trazas**: el recorrido de una petición a través de varios servicios.

Con esto se construyen tableros y **alertas** que avisan antes de que el problema escale. Es un insumo clave del [[Debugging]] en producción.

---

## Ejemplo sencillo
Es como el tablero de un coche: velocímetro, temperatura, nivel de gasolina y luces de advertencia. No necesitas abrir el motor para saber que algo va mal; los indicadores te lo dicen a tiempo.

---

## Conceptos relacionados
- [[Debugging]] — la observabilidad aporta los datos para diagnosticar en producción.
- [[Reliability]] — medir es el primer paso para mejorar la fiabilidad.
- [[Distributed Systems]] — las trazas son esenciales cuando una petición cruza muchos servicios.

---

## Antes de estudiar esto
- [[Debugging]]

---

## Después de estudiar esto
- [[Reliability]]
- [[Distributed Systems]]

---

## Preguntas de comprobación
1. ¿Cuáles son los tres pilares de la observabilidad?
2. ¿Qué diferencia hay entre un log y una métrica?
3. ¿Por qué las trazas son especialmente útiles en sistemas distribuidos?
4. ¿En qué se diferencia "monitoreo" de "observabilidad"?

---

## Errores comunes
- Registrar todo sin criterio y luego no encontrar nada útil.
- Confiar solo en logs y no tener métricas ni trazas.
- Poner alertas para todo, generando ruido que el equipo termina ignorando.

---

## Resumen
- La observabilidad permite entender el estado interno de un sistema desde sus salidas.
- Se apoya en logs, métricas y trazas.
- Es clave para diagnosticar fallos en producción.
- Habilita alertas tempranas y mejora la fiabilidad.
- Cobra especial importancia en sistemas distribuidos.

---

## Fuentes
- CNCF — *OpenTelemetry Documentation*: https://opentelemetry.io/docs/
- Google — *SRE Book: Monitoring Distributed Systems*: https://sre.google/sre-book/monitoring-distributed-systems/
