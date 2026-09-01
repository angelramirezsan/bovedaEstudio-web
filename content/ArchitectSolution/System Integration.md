---
title: "System Integration"
type: "concept"
area: "Solution Architecture"
level: 3
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[API]]"
  - "[[Microservices]]"
related:
  - "[[Messaging]]"
  - "[[Event-Driven Architecture]]"
  - "[[AI Integration]]"
tags:
  - solution-architecture
  - integracion
---

# System Integration

## ¿Qué es?
La integración de sistemas es hacer que aplicaciones distintas trabajen juntas e intercambien información, aunque hayan sido creadas por separado, con tecnologías diferentes y en momentos distintos.

**Definición técnica:** disciplina que conecta sistemas heterogéneos para que compartan datos y procesos, mediante mecanismos como APIs, mensajería, eventos o archivos, resolviendo diferencias de formato, protocolo y semántica.

---

## ¿Por qué existe?
Ninguna organización usa un solo sistema: hay CRM, facturación, inventario, etc., a menudo de distintos proveedores. Sin integración, los datos quedan aislados en silos y los procesos se rompen. La integración existe para conectar ese ecosistema.

---

## ¿Qué problema resuelve?
- Silos de información que no se comunican entre sí.
- Procesos manuales de copiar datos de un sistema a otro.
- Inconsistencias entre sistemas que deberían tener la misma información.

---

## ¿Cómo funciona?
Existen varios estilos, catalogados en los **patrones de integración empresarial**:
- **Síncrono** vía [[API]]: un sistema llama a otro y espera respuesta.
- **Asíncrono** vía [[Messaging]] / [[Event-Driven Architecture]]: los sistemas se comunican por mensajes o eventos sin esperarse.
- **Por lotes**: intercambio periódico de archivos.

La elección depende de requisitos de tiempo real, acoplamiento y volumen.

---

## Ejemplo sencillo
Es como coordinar varias empresas en una cadena de suministro: la fábrica, el transportista y la tienda usan sistemas distintos, pero deben intercambiar pedidos y estados. La integración es el conjunto de acuerdos y canales que hace que fluyan sin errores.

---

## Conceptos relacionados
- [[API]] — mecanismo de integración síncrona más común.
- [[Messaging]] — habilita integración asíncrona y desacoplada.
- [[Event-Driven Architecture]] — estilo de integración basado en eventos.
- [[AI Integration]] — aplica estos principios para incorporar IA a los sistemas existentes.

---

## Antes de estudiar esto
- [[API]]
- [[Microservices]]

---

## Después de estudiar esto
- [[Messaging]]
- [[Event-Driven Architecture]]
- [[Distributed Systems]]

---

## Preguntas de comprobación
1. ¿Qué es un silo de información y por qué es un problema?
2. ¿Qué diferencia hay entre integración síncrona y asíncrona?
3. ¿Cuándo preferirías mensajería frente a llamadas directas por API?
4. ¿Por qué la integración implica resolver diferencias de formato y semántica?

---

## Errores comunes
- Integrar todo de forma síncrona y crear dependencias frágiles.
- Ignorar las diferencias de significado de los datos entre sistemas.
- Copiar datos manualmente en lugar de automatizar la integración.

---

## Resumen
- Conecta sistemas heterogéneos para que compartan datos y procesos.
- Rompe silos de información y automatiza flujos.
- Puede ser síncrona (API), asíncrona (mensajería/eventos) o por lotes.
- La elección depende de tiempo real, acoplamiento y volumen.
- Es la antesala de los sistemas distribuidos y la arquitectura de soluciones.

---

## Fuentes
- Hohpe & Woolf — *Enterprise Integration Patterns*: https://www.enterpriseintegrationpatterns.com/
- Microsoft — *Azure Architecture Center: Integration*: https://learn.microsoft.com/en-us/azure/architecture/example-scenario/integration/
