---
title: "Machine Learning"
type: "concept"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Artificial Intelligence]]"
  - "[[Data Structures and Algorithms]]"
related:
  - "[[Generative AI]]"
  - "[[Embeddings]]"
  - "[[Databases]]"
tags:
  - ai
---

# Machine Learning

## ¿Qué es?
El aprendizaje automático (Machine Learning, ML) es la rama de la IA en la que un sistema aprende patrones a partir de datos, en lugar de seguir reglas escritas por una persona. Le muestras muchos ejemplos y aprende a generalizar.

**Definición técnica:** subcampo de la [[Artificial Intelligence]] que estudia algoritmos capaces de mejorar su desempeño en una tarea a partir de la experiencia (datos), construyendo modelos estadísticos que generalizan a datos nuevos.

---

## ¿Por qué existe?
Para muchas tareas (predecir demanda, detectar fraude, reconocer voz) es imposible escribir todas las reglas a mano. El ML existe para que el sistema descubra esas reglas por sí mismo a partir de ejemplos.

---

## ¿Qué problema resuelve?
- Tareas donde las reglas son demasiadas o desconocidas.
- Hacer predicciones a partir de datos históricos.
- Adaptarse cuando los patrones cambian, reentrenando con nuevos datos.

---

## ¿Cómo funciona?
Se entrena un **modelo** con datos. Enfoques principales:
- **Supervisado**: aprende de ejemplos etiquetados (correo = spam/no spam).
- **No supervisado**: encuentra estructura sin etiquetas (agrupar clientes similares).
- **Por refuerzo**: aprende por ensayo y error con recompensas.

El objetivo es **generalizar** a datos nuevos, evitando el **sobreajuste** (memorizar en vez de aprender). La calidad de los datos es determinante: "basura entra, basura sale".

---

## Ejemplo sencillo
Es como enseñar a un niño a distinguir perros de gatos: no le das una definición exacta, le muestras muchas fotos etiquetadas hasta que aprende a reconocer uno nuevo que nunca vio. El modelo hace algo análogo con datos.

---

## Conceptos relacionados
- [[Artificial Intelligence]] — el ML es su subcampo dominante hoy.
- [[Generative AI]] — se apoya en técnicas avanzadas de ML (redes neuronales profundas).
- [[Embeddings]] — representaciones numéricas aprendidas por modelos de ML.
- [[Databases]] — los datos de entrenamiento suelen venir de bases de datos.

---

## Antes de estudiar esto
- [[Artificial Intelligence]]

---

## Después de estudiar esto
- [[Generative AI]]
- [[Embeddings]]

---

## Preguntas de comprobación
1. ¿Qué diferencia el ML de programar reglas explícitas?
2. ¿Qué distingue el aprendizaje supervisado del no supervisado?
3. ¿Qué es el sobreajuste (overfitting)?
4. ¿Por qué la calidad de los datos es tan determinante?

---

## Errores comunes
- Creer que más datos siempre es mejor, sin cuidar su calidad.
- Confundir memorizar los datos de entrenamiento (sobreajuste) con aprender.
- Asumir que un modelo es objetivo: puede heredar sesgos de sus datos.

---

## Resumen
- El ML aprende patrones a partir de datos en lugar de reglas fijas.
- Enfoques: supervisado, no supervisado y por refuerzo.
- Busca generalizar a datos nuevos evitando el sobreajuste.
- La calidad de los datos es determinante.
- Es la base técnica de la IA moderna, incluida la generativa.

---

## Fuentes
- Google — *Machine Learning Crash Course*: https://developers.google.com/machine-learning/crash-course
- Microsoft — *Learn: Machine learning*: https://learn.microsoft.com/en-us/training/paths/introduction-to-machine-learning/
- NIST — *AI Risk Management Framework*: https://www.nist.gov/itl/ai-risk-management-framework
