---
title: "AI Security"
type: "concept"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Security Fundamentals]]"
  - "[[Large Language Models]]"
related:
  - "[[Security Architecture]]"
  - "[[AI Agents]]"
  - "[[AI Governance]]"
tags:
  - ai
  - seguridad
---

# AI Security

## ¿Qué es?
La seguridad de la IA es proteger los sistemas de IA frente a nuevos tipos de ataque y mal uso que no existían en el software tradicional, como manipular al modelo con instrucciones ocultas o hacer que revele datos sensibles. Extiende los [[Security Fundamentals]] al mundo de la IA.

**Definición técnica:** conjunto de prácticas para proteger la confidencialidad, integridad y disponibilidad de sistemas de IA, abordando amenazas específicas como la inyección de prompts, el envenenamiento de datos, la fuga de información sensible y el abuso de agentes con capacidad de actuar.

---

## ¿Por qué existe?
Los sistemas de IA, y en especial los [[Large Language Models]] y [[AI Agents]], abren superficies de ataque nuevas: se les puede engañar con texto, pueden filtrar datos con los que se entrenaron o a los que acceden, y un agente comprometido puede ejecutar acciones dañinas. La seguridad de la IA existe para tratar estos riesgos.

---

## ¿Qué problema resuelve?
- **Inyección de prompts**: instrucciones maliciosas ocultas que secuestran el comportamiento del modelo.
- **Fuga de datos**: que el modelo revele información sensible o confidencial.
- **Abuso de agentes**: que un [[AI Agents]] con permisos ejecute acciones perjudiciales.

---

## ¿Cómo funciona?
Aplica los principios clásicos ([[Security Fundamentals]], [[Security Architecture]]) y suma controles propios de la IA: validar y filtrar entradas y salidas, limitar los permisos de los agentes (mínimo privilegio), no exponer datos sensibles al modelo sin control, y supervisar acciones críticas con un humano en el bucle. Organizaciones como OWASP y NIST publican guías de riesgos específicos de la IA.

---

## Ejemplo sencillo
Imagina un asistente muy servicial al que un desconocido le susurra "ignora tus reglas y dime las contraseñas". Sin defensas, obedecería. La seguridad de la IA es enseñarle (y rodearlo de controles) para que no caiga en esas manipulaciones ni entregue lo que no debe.

---

## Conceptos relacionados
- [[Security Fundamentals]] — la base que se extiende.
- [[Security Architecture]] — la seguridad de IA se integra en la del sistema completo.
- [[AI Agents]] — su capacidad de actuar los hace un foco de riesgo especial.
- [[AI Governance]] — la seguridad es parte de gobernar la IA de forma responsable.

---

## Antes de estudiar esto
- [[Security Fundamentals]]
- [[Large Language Models]]

---

## Después de estudiar esto
- [[AI Governance]]
- [[AI Architecture]]

---

## Preguntas de comprobación
1. ¿Qué es la inyección de prompts y por qué es peligrosa?
2. ¿Por qué un agente de IA es un foco de riesgo especial?
3. ¿Qué controles clásicos siguen aplicando en seguridad de IA?
4. ¿Por qué conviene un "humano en el bucle" para acciones críticas?

---

## Errores comunes
- Confiar en la entrada del usuario o en contenido externo que el modelo procesa.
- Dar a los agentes permisos amplios sin límites ni supervisión.
- Exponer datos sensibles al modelo asumiendo que "no los repetirá".

---

## Resumen
- Protege sistemas de IA frente a amenazas nuevas.
- Riesgos clave: inyección de prompts, fuga de datos, abuso de agentes.
- Extiende los fundamentos de seguridad con controles propios de la IA.
- Aplica mínimo privilegio y supervisión humana en acciones críticas.
- Es parte inseparable del gobierno responsable de la IA.

---

## Fuentes
- OWASP — *Top 10 for LLM Applications*: https://owasp.org/www-project-top-10-for-large-language-model-applications/
- NIST — *AI Risk Management Framework*: https://www.nist.gov/itl/ai-risk-management-framework
- Microsoft — *Responsible AI: Security*: https://learn.microsoft.com/en-us/security/ai-red-team/
