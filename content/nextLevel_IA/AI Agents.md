---
title: "AI Agents"
type: "concept"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Large Language Models]]"
  - "[[Prompt Engineering]]"
related:
  - "[[RAG]]"
  - "[[Microservices]]"
  - "[[AI Integration]]"
  - "[[AI Security]]"
tags:
  - ai
  - genai
---

# AI Agents

## ¿Qué es?
Un agente de IA es un sistema que usa un modelo de IA para no solo responder, sino *actuar*: decidir qué pasos dar, usar herramientas (buscar, llamar a una [[API]], ejecutar código) y perseguir un objetivo con varios pasos, no solo una respuesta.

**Definición técnica:** sistema que emplea un [[Large Language Models]] como motor de razonamiento para planificar y ejecutar acciones de forma autónoma, invocando herramientas externas y observando resultados en un ciclo de percepción-decisión-acción hasta alcanzar un objetivo.

---

## ¿Por qué existe?
Un LLM por sí solo solo genera texto: no puede consultar datos actuales ni ejecutar tareas. Los agentes existen para conectar el razonamiento del modelo con acciones reales, permitiendo automatizar tareas de varios pasos.

---

## ¿Qué problema resuelve?
- La limitación de un LLM que solo "habla" pero no actúa.
- Automatizar tareas que requieren varios pasos y decisiones intermedias.
- Integrar el razonamiento de IA con sistemas y datos reales.

---

## ¿Cómo funciona?
El agente recibe un objetivo, el LLM **planifica** los pasos, elige y usa **herramientas** (buscar en [[RAG]], llamar a una [[API]], ejecutar código), **observa** los resultados y decide el siguiente paso, repitiendo hasta terminar. Conceptualmente se parece a un [[Microservices]] autónomo con capacidad de decisión. Requiere controles de [[AI Security]] estrictos: un agente con permisos amplios puede causar daño real si se desvía o es manipulado.

---

## Ejemplo sencillo
Es la diferencia entre preguntarle a alguien "¿cómo reservo un vuelo?" (te explica) y darle una tarjeta y pedirle "resérvame el vuelo más barato el viernes" (busca, compara, decide y ejecuta). El agente hace lo segundo: actúa hacia un objetivo, no solo informa.

---

## Conceptos relacionados
- [[Large Language Models]] — el motor de razonamiento del agente.
- [[RAG]] — una de las herramientas típicas para recuperar información.
- [[Microservices]] — analogía arquitectónica: componentes autónomos que colaboran.
- [[AI Integration]] — cómo se conectan los agentes con los sistemas existentes.
- [[AI Security]] — crítica, por su capacidad de actuar con permisos reales.

---

## Antes de estudiar esto
- [[Large Language Models]]
- [[Prompt Engineering]]

---

## Después de estudiar esto
- [[AI Integration]]
- [[AI Architecture]]

---

## Preguntas de comprobación
1. ¿Qué diferencia a un agente de un simple chatbot?
2. ¿Qué es una "herramienta" en el contexto de un agente?
3. ¿Por qué la seguridad es especialmente crítica en agentes?
4. ¿Qué analogía existe entre un agente y un microservicio?

---

## Errores comunes
- Dar a un agente permisos amplios sin controles ni supervisión.
- Asumir que planifica sin errores; puede desviarse o quedar en bucles.
- Confiar acciones críticas e irreversibles a un agente sin validación humana.

---

## Resumen
- Un agente usa IA para planificar y ejecutar acciones, no solo responder.
- Combina razonamiento (LLM) con herramientas externas.
- Opera en un ciclo de decisión-acción-observación.
- Se parece a un componente autónomo (microservicio con decisión).
- Exige controles de seguridad estrictos por su capacidad de actuar.

---

## Fuentes
- Microsoft — *Learn: AI agents*: https://learn.microsoft.com/en-us/azure/ai-services/agents/overview
- Google Cloud — *AI agents*: https://cloud.google.com/discover/what-are-ai-agents
- OWASP — *Top 10 for LLM Applications*: https://owasp.org/www-project-top-10-for-large-language-model-applications/
