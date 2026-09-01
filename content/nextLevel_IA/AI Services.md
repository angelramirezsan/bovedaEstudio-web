---
title: "AI Services"
type: "concept"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[API]]"
  - "[[Artificial Intelligence]]"
related:
  - "[[AI Integration]]"
  - "[[Cloud Architecture]]"
  - "[[Generative AI]]"
tags:
  - ai
  - integracion
---

# AI Services

## ¿Qué es?
Los servicios de IA son capacidades de inteligencia artificial que consumes a través de una [[API]], sin tener que construir ni entrenar el modelo tú mismo. Envías una petición (texto, imagen) y recibes un resultado (una respuesta, una transcripción, una clasificación).

**Definición técnica:** funcionalidades de IA expuestas como servicios accesibles vía API, normalmente alojadas en la [[Cloud Architecture]], que abstraen el modelo y su infraestructura bajo un contrato de uso (pago por consumo).

---

## ¿Por qué existe?
Entrenar y operar modelos de IA es costoso y complejo. La mayoría de organizaciones no necesita construir el modelo, sino usar la capacidad. Los servicios de IA existen para consumir IA como cualquier otra API, sin la carga de crearla.

---

## ¿Qué problema resuelve?
- La barrera de entrada de construir y entrenar modelos propios.
- El costo de operar la infraestructura de IA.
- La necesidad de incorporar IA rápidamente a aplicaciones existentes.

---

## ¿Cómo funciona?
El proveedor aloja el modelo y lo expone como una [[API]]. Tu aplicación envía una petición y recibe el resultado, igual que consume cualquier otro servicio. Este es el **puente directo entre la arquitectura de software clásica y la IA**: una [[API]] "normal" pasa a ser una [[API]] de IA. Se integra en los sistemas mediante [[AI Integration]].

---

## Ejemplo sencillo
Es como usar un servicio de mensajería en lugar de tener tu propia flota de camiones. No compras camiones ni contratas conductores: le entregas el paquete al servicio y él lo entrega. Con la IA igual: no construyes el modelo, solo consumes la capacidad vía API.

---

## Conceptos relacionados
- [[API]] — el mecanismo por el que se consumen (el puente clave).
- [[Artificial Intelligence]] — la capacidad que exponen.
- [[Cloud Architecture]] — dónde suelen alojarse.
- [[AI Integration]] — cómo se conectan a los sistemas existentes.

---

## Antes de estudiar esto
- [[API]]
- [[Artificial Intelligence]]

---

## Después de estudiar esto
- [[AI Integration]]
- [[AI Architecture]]

---

## Preguntas de comprobación
1. ¿Qué ventaja tiene consumir IA como servicio en lugar de construir el modelo?
2. ¿Por qué se dice que un servicio de IA es "una API más"?
3. ¿Qué relación tienen con la nube?
4. ¿Qué debes cuidar al enviar datos a un servicio de IA externo? (pista: privacidad)

---

## Errores comunes
- Enviar datos sensibles a un servicio externo sin revisar privacidad y cumplimiento.
- Asumir disponibilidad y costo constantes sin considerar límites de uso.
- Depender de un único proveedor sin plan de portabilidad.

---

## Resumen
- Son capacidades de IA consumibles vía API.
- Evitan tener que construir y operar el modelo.
- Suelen alojarse en la nube con pago por uso.
- Son el puente directo entre la arquitectura clásica y la IA.
- Requieren cuidar privacidad y dependencia del proveedor.

---

## Fuentes
- Microsoft — *Azure AI Services*: https://learn.microsoft.com/en-us/azure/ai-services/
- Google Cloud — *AI and Machine Learning products*: https://cloud.google.com/products/ai
- AWS — *Machine Learning Services*: https://aws.amazon.com/machine-learning/
