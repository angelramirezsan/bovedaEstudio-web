---
title: "RAG"
aliases:
  - "Retrieval-Augmented Generation"
type: "pattern"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Large Language Models]]"
  - "[[Embeddings]]"
  - "[[Vector Databases]]"
related:
  - "[[Prompt Engineering]]"
  - "[[AI Agents]]"
  - "[[AI Architecture]]"
tags:
  - ai
  - genai
---

# RAG

## ¿Qué es?
RAG (Generación Aumentada por Recuperación) es una técnica para que un [[Large Language Models]] responda usando información específica que no tenía en su entrenamiento (documentos de tu empresa, datos actuales). Primero *recupera* información relevante y luego el modelo *genera* la respuesta con ese contexto.

**Definición técnica:** patrón arquitectónico que combina recuperación de información (búsqueda de fragmentos relevantes en una fuente externa, típicamente vía [[Embeddings]] y [[Vector Databases]]) con generación por un LLM, inyectando el contexto recuperado en el prompt para fundamentar la respuesta.

---

## ¿Por qué existe?
Los LLM tienen conocimiento limitado a su fecha de entrenamiento, no conocen tus datos privados y pueden alucinar. RAG existe para darles información fresca, específica y verificable en el momento de responder, sin tener que reentrenarlos (algo caro y lento).

---

## ¿Qué problema resuelve?
- El desconocimiento del modelo sobre datos privados o actuales.
- Las alucinaciones, al fundamentar la respuesta en fuentes reales.
- El alto costo de reentrenar el modelo cada vez que cambian los datos.

---

## ¿Cómo funciona?
Dos fases:
1. **Recuperación**: la pregunta se convierte en un [[Embeddings]] y se buscan los fragmentos más relevantes en una [[Vector Databases]].
2. **Generación**: esos fragmentos se añaden al prompt ([[Prompt Engineering]]) y el LLM redacta la respuesta basándose en ellos, idealmente citando la fuente.

Así la respuesta se apoya en datos concretos en lugar de solo en la "memoria" del modelo.

---

## Ejemplo sencillo
Es como un examen a libro abierto. En vez de responder solo de memoria (y arriesgarse a inventar), primero buscas en los apuntes el fragmento relevante y luego redactas la respuesta basándote en él. RAG le da al modelo esos "apuntes" en el momento justo.

---

## Conceptos relacionados
- [[Large Language Models]] — el componente que genera la respuesta.
- [[Embeddings]] y [[Vector Databases]] — hacen posible la recuperación semántica.
- [[Prompt Engineering]] — el contexto recuperado se inyecta en el prompt.
- [[AI Agents]] — la recuperación puede ser una de las herramientas de un agente.

---

## Antes de estudiar esto
- [[Large Language Models]]
- [[Vector Databases]]

---

## Después de estudiar esto
- [[AI Agents]]
- [[AI Architecture]]

---

## Preguntas de comprobación
1. ¿Qué dos fases componen RAG?
2. ¿Por qué RAG reduce (aunque no elimina) las alucinaciones?
3. ¿Qué ventaja tiene frente a reentrenar el modelo con tus datos?
4. ¿Qué papel juegan los embeddings y la base vectorial?

---

## Errores comunes
- Creer que RAG elimina por completo las alucinaciones (las reduce).
- Recuperar fragmentos irrelevantes por mala calidad de los embeddings o el troceado.
- No citar la fuente, perdiendo la verificabilidad que RAG habilita.

---

## Resumen
- RAG combina recuperación de información con generación por un LLM.
- Aporta datos privados o actuales sin reentrenar el modelo.
- Fundamenta las respuestas y reduce alucinaciones.
- Se apoya en embeddings y bases de datos vectoriales.
- Es uno de los patrones más usados para IA en la empresa.

---

## Fuentes
- Lewis et al. — *Retrieval-Augmented Generation* (2020): https://arxiv.org/abs/2005.11401
- AWS — *What is RAG?*: https://aws.amazon.com/what-is/retrieval-augmented-generation/
- Microsoft — *Learn: RAG*: https://learn.microsoft.com/en-us/azure/search/retrieval-augmented-generation-overview
