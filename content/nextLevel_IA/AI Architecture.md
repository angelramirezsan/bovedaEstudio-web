---
title: "AI Architecture"
type: "architecture"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Solution Architecture]]"
  - "[[AI Integration]]"
related:
  - "[[RAG]]"
  - "[[AI Agents]]"
  - "[[AI Security]]"
  - "[[AI Governance]]"
  - "[[Cloud Architecture]]"
tags:
  - ai
  - arquitectura
---

# AI Architecture

## ¿Qué es?
La arquitectura de IA es el diseño de soluciones completas que incorporan inteligencia artificial: cómo encajan los modelos, los datos, la recuperación de información, la seguridad y el resto del sistema para resolver un problema de negocio. Es la [[Solution Architecture]] cuando la IA es un componente central.

**Definición técnica:** disciplina que diseña soluciones integrales basadas en IA, definiendo el flujo de datos, la selección y orquestación de modelos y patrones (como [[RAG]] y [[AI Agents]]), la infraestructura, la seguridad ([[AI Security]]) y el gobierno ([[AI Governance]]), gestionando trade-offs propios de la IA.

---

## ¿Por qué existe?
Añadir IA a un sistema introduce retos que la arquitectura clásica no cubre del todo: modelos que alucinan, datos de entrenamiento y calidad, costos variables, latencia, privacidad y sesgos. La arquitectura de IA existe para diseñar soluciones con IA de forma responsable, fiable y sostenible.

---

## ¿Qué problema resuelve?
- Soluciones con IA improvisadas que no escalan ni son fiables.
- Riesgos específicos de la IA sin tratamiento arquitectónico (alucinaciones, sesgos, fuga de datos).
- Falta de una visión integral que una modelo, datos, seguridad y negocio.

---

## ¿Cómo funciona?
Parte de los objetivos de negocio y decide: qué modelo o [[AI Services]] usar, cómo aportar contexto ([[RAG]]), si hacen falta [[AI Agents]], sobre qué [[Cloud Architecture]] correr, cómo asegurar la solución ([[AI Security]]) y cómo gobernarla ([[AI Governance]]). Reutiliza todo lo aprendido en [[Solution Architecture]] y suma los trade-offs propios de la IA (calidad vs. costo, latencia vs. precisión). Documenta decisiones en [[Architecture Decision Records]].

---

## Ejemplo sencillo
Diseñar un asistente de atención al cliente con IA no es solo "conectar un modelo". Es decidir de dónde saca la información (RAG sobre tus manuales), qué puede y no puede hacer (seguridad), cómo se revisa su calidad, cuánto cuesta cada respuesta y cómo encaja con el sistema de tickets existente. La arquitectura de IA orquesta todo eso.

---

## Conceptos relacionados
- [[Solution Architecture]] — la base que la arquitectura de IA extiende.
- [[RAG]] y [[AI Agents]] — patrones centrales que orquesta.
- [[AI Security]] y [[AI Governance]] — dimensiones inseparables del diseño.
- [[Cloud Architecture]] — infraestructura habitual de las soluciones de IA.

---

## Antes de estudiar esto
- [[Solution Architecture]]
- [[AI Integration]]

---

## Después de estudiar esto
- [[AI Security]]
- [[AI Governance]]

---

## Preguntas de comprobación
1. ¿Qué añade la arquitectura de IA respecto a la arquitectura de soluciones clásica?
2. ¿Qué riesgos propios de la IA debe tratar?
3. ¿Qué trade-offs específicos aparecen (ej. calidad vs. costo)?
4. ¿Por qué seguridad y gobierno son inseparables de su diseño?

---

## Errores comunes
- Diseñar "poniendo un modelo" sin pensar datos, seguridad ni costos.
- Ignorar alucinaciones y sesgos como problemas de arquitectura.
- Tratar la IA como magia y no como un componente con límites y trade-offs.

---

## Resumen
- Diseña soluciones completas donde la IA es un componente central.
- Extiende la arquitectura de soluciones con retos propios de la IA.
- Orquesta modelos, datos, RAG, agentes, seguridad y gobierno.
- Gestiona trade-offs como calidad vs. costo y latencia vs. precisión.
- Es la culminación del recorrido: software → arquitectura → IA.

---

## Fuentes
- Microsoft — *Azure Architecture Center: AI architecture design*: https://learn.microsoft.com/en-us/azure/architecture/ai-ml/
- AWS — *Well-Architected: Machine Learning Lens*: https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/machine-learning-lens.html
- NIST — *AI Risk Management Framework*: https://www.nist.gov/itl/ai-risk-management-framework
