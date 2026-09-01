---
title: "Large Language Models"
aliases:
  - "LLM"
  - "LLMs"
type: "technology"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Generative AI]]"
related:
  - "[[Prompt Engineering]]"
  - "[[Embeddings]]"
  - "[[RAG]]"
  - "[[AI Agents]]"
tags:
  - ai
  - genai
---

# Large Language Models

## ¿Qué es?
Un modelo de lenguaje grande (LLM) es un tipo de IA generativa entrenada con enormes cantidades de texto para entender y producir lenguaje natural. Es la tecnología detrás de los asistentes conversacionales modernos.

**Definición técnica:** modelo de [[Generative AI]] basado en arquitecturas de red neuronal (típicamente Transformers) con gran cantidad de parámetros, entrenado sobre grandes corpus de texto para predecir la siguiente unidad de texto (token) y así generar lenguaje coherente.

---

## ¿Por qué existe?
Se necesitaban sistemas capaces de trabajar con lenguaje humano de forma flexible: responder preguntas, resumir, traducir, programar. Los LLM existen porque, entrenados a gran escala, generalizan a una enorme variedad de tareas de lenguaje sin programarse una por una.

---

## ¿Qué problema resuelve?
- Interactuar con sistemas usando lenguaje natural en lugar de comandos rígidos.
- Automatizar tareas de texto: redactar, resumir, clasificar, traducir, programar.
- Servir de "cerebro" de razonamiento para agentes y asistentes.

---

## ¿Cómo funciona?
Predicen el siguiente **token** (fragmento de texto) según el contexto previo. Ese contexto tiene un límite (la **ventana de contexto**). No "saben" hechos: reproducen patrones de su entrenamiento, por lo que pueden **alucinar** (inventar con seguridad). Su conocimiento está limitado a la fecha de entrenamiento; para datos actuales o privados se combinan con [[RAG]]. Se les instruye mediante [[Prompt Engineering]].

---

## Ejemplo sencillo
Es como un autocompletado extraordinariamente sofisticado: dado lo que llevas escrito, propone lo más probable a continuación, pero con tal riqueza que puede sostener una conversación o redactar un texto. Aun así, no consulta una verdad: continúa un patrón.

---

## Conceptos relacionados
- [[Generative AI]] — los LLM son su exponente para texto.
- [[Prompt Engineering]] — cómo se les dan instrucciones eficaces.
- [[Embeddings]] — cómo representan el significado del texto.
- [[RAG]] — les aporta información externa y actualizada.
- [[AI Agents]] — usan un LLM como motor de razonamiento.

---

## Antes de estudiar esto
- [[Generative AI]]

---

## Después de estudiar esto
- [[Prompt Engineering]]
- [[RAG]]
- [[AI Agents]]

---

## Preguntas de comprobación
1. ¿Qué predice realmente un LLM?
2. ¿Qué es la ventana de contexto y por qué importa?
3. ¿Por qué un LLM puede alucinar?
4. ¿Cómo se le puede dar información actual o privada que no vio en su entrenamiento?

---

## Errores comunes
- Creer que "sabe" o "consulta hechos"; genera texto probable.
- Confiar en sus respuestas sin verificarlas.
- Meter demasiada información y superar la ventana de contexto.

---

## Resumen
- Un LLM genera lenguaje prediciendo el siguiente token.
- Es el motor de la IA generativa de texto.
- Tiene una ventana de contexto limitada.
- Puede alucinar y su conocimiento tiene fecha de corte.
- Se combina con RAG y prompt engineering para ser útil y fiable.

---

## Fuentes
- Vaswani et al. — *Attention Is All You Need* (2017): https://arxiv.org/abs/1706.03762
- Google — *Machine Learning: LLMs*: https://developers.google.com/machine-learning/resources/intro-llms
- Microsoft — *Learn: How large language models work*: https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/
