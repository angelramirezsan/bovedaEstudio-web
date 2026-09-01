---
title: "Prompt Engineering"
type: "practice"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Large Language Models]]"
related:
  - "[[Generative AI]]"
  - "[[RAG]]"
  - "[[AI Agents]]"
tags:
  - ai
  - genai
---

# Prompt Engineering

## ¿Qué es?
El prompt engineering es la práctica de escribir buenas instrucciones (*prompts*) para obtener mejores respuestas de un modelo de IA generativa. Cómo pides algo influye enormemente en lo que recibes.

**Definición técnica:** conjunto de técnicas para diseñar y estructurar las entradas a un modelo de lenguaje (contexto, instrucciones, ejemplos, formato de salida) con el fin de guiar su comportamiento y mejorar la calidad, precisión y consistencia de sus respuestas.

---

## ¿Por qué existe?
Un [[Large Language Models]] responde según lo que le pides y cómo se lo pides. Instrucciones vagas dan resultados pobres; instrucciones claras y con contexto dan resultados útiles. El prompt engineering existe para aprovechar bien estos modelos sin reentrenarlos.

---

## ¿Qué problema resuelve?
- Respuestas vagas, incorrectas o con formato inutilizable.
- Falta de control sobre el estilo, el detalle o la estructura de la salida.
- Obtener resultados consistentes para tareas repetibles.

---

## ¿Cómo funciona?
Se apoya en técnicas: dar **contexto** y **rol** claros, especificar el **formato de salida**, dividir tareas complejas en pasos, y aportar **ejemplos** (*few-shot*) o pedir que razone paso a paso (*chain-of-thought*). Cuando el modelo necesita datos externos o actuales, el prompt se combina con [[RAG]]. Es una práctica basada en iteración y experimentación, no una ciencia exacta.

---

## Ejemplo sencillo
Es como delegar una tarea a un asistente muy capaz pero literal. "Hazme algo de un informe" da un resultado impredecible. "Redacta un resumen de 5 puntos de este texto, en tono formal, para directivos" da justo lo que necesitas. La claridad de la instrucción define el resultado.

---

## Conceptos relacionados
- [[Large Language Models]] — el destinatario de los prompts.
- [[Generative AI]] — el prompt es la interfaz principal para dirigirla.
- [[RAG]] — enriquece el prompt con información externa.
- [[AI Agents]] — usan prompts estructurados para planificar y actuar.

---

## Antes de estudiar esto
- [[Large Language Models]]

---

## Después de estudiar esto
- [[RAG]]
- [[AI Agents]]

---

## Preguntas de comprobación
1. ¿Por qué la forma de pedir algo cambia tanto el resultado?
2. ¿Qué aporta dar contexto y un formato de salida esperado?
3. ¿Qué es un prompt "few-shot"?
4. ¿Cuándo conviene combinar el prompt con RAG?

---

## Errores comunes
- Dar instrucciones vagas y culpar al modelo del mal resultado.
- No especificar el formato de salida que se necesita.
- Asumir que un buen prompt garantiza veracidad (sigue pudiendo alucinar).

---

## Resumen
- Es la práctica de escribir instrucciones eficaces para IA generativa.
- La claridad, el contexto y los ejemplos mejoran el resultado.
- Técnicas: rol, formato, few-shot, razonamiento por pasos.
- Se combina con RAG cuando hacen falta datos externos.
- Es iterativo y experimental, no una ciencia exacta.

---

## Fuentes
- Google — *Prompting guidance*: https://developers.google.com/machine-learning/resources/prompt-eng
- Microsoft — *Learn: Prompt engineering*: https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering
- OpenAI — *Prompt engineering guide*: https://platform.openai.com/docs/guides/prompt-engineering
