---
title: "Security Architecture"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Security Fundamentals]]"
  - "[[Software Architecture]]"
related:
  - "[[Cloud Architecture]]"
  - "[[Distributed Systems]]"
  - "[[AI Security]]"
tags:
  - solution-architecture
  - seguridad
---

# Security Architecture

## ¿Qué es?
La arquitectura de seguridad es el diseño de cómo se protege un sistema completo: qué controles hay, dónde están las fronteras de confianza y cómo se defiende la solución en su conjunto, no solo una pieza. Lleva los [[Security Fundamentals]] al nivel de sistema.

**Definición técnica:** disciplina que define la estructura de controles de seguridad de una solución, sus fronteras de confianza, flujos de datos y mecanismos de defensa, alineados con un modelo de amenazas y principios como defensa en profundidad y confianza cero.

---

## ¿Por qué existe?
Aplicar seguridad pieza por pieza deja huecos entre componentes. Un atacante busca el eslabón más débil de toda la solución. La arquitectura de seguridad existe para diseñar la defensa de forma integral y coherente.

---

## ¿Qué problema resuelve?
- Huecos de seguridad entre componentes que individualmente parecen seguros.
- Falta de una visión global de amenazas y controles.
- Confianza excesiva en la "red interna" como si fuera segura por defecto.

---

## ¿Cómo funciona?
Se apoya en principios de nivel de sistema:
- **Defensa en profundidad**: varias capas de protección, no una sola.
- **Confianza cero (Zero Trust)**: no confiar por defecto en nada, verificar siempre.
- **Modelado de amenazas**: analizar cómo podría atacarse el sistema antes de construirlo.
- **Mínimo privilegio** y segmentación de redes.

Es especialmente crítica en [[Cloud Architecture]] y [[Distributed Systems]], donde la superficie de ataque es amplia.

---

## Ejemplo sencillo
Proteger una casa no es solo poner una buena cerradura (un control). Es pensar en el conjunto: cerca, cámaras, alarma, iluminación, y no dar por seguro que "quien ya está dentro" es de confianza. La arquitectura de seguridad diseña todas esas capas juntas.

---

## Conceptos relacionados
- [[Security Fundamentals]] — la base que esta arquitectura lleva a escala de sistema.
- [[Cloud Architecture]] — introduce el modelo de responsabilidad compartida.
- [[Distributed Systems]] — amplían la superficie de ataque.
- [[AI Security]] — extiende estos principios a los riesgos propios de la IA.

---

## Antes de estudiar esto
- [[Security Fundamentals]]
- [[Software Architecture]]

---

## Después de estudiar esto
- [[Solution Architecture]]
- [[AI Security]]

---

## Preguntas de comprobación
1. ¿Qué es la defensa en profundidad?
2. ¿Qué propone el modelo de confianza cero (Zero Trust)?
3. ¿Para qué sirve el modelado de amenazas?
4. ¿Por qué confiar en la "red interna" es un riesgo?

---

## Errores comunes
- Confiar en un solo control (una sola capa de defensa).
- Asumir que el tráfico interno es seguro por estar "dentro".
- Diseñar la seguridad al final en lugar de desde la arquitectura.

---

## Resumen
- Diseña la defensa del sistema como un todo, no pieza por pieza.
- Se apoya en defensa en profundidad y confianza cero.
- Usa modelado de amenazas para anticipar ataques.
- Es crítica en la nube y en sistemas distribuidos.
- Extiende los fundamentos de seguridad a escala de solución.

---

## Fuentes
- NIST — *SP 800-207: Zero Trust Architecture*: https://csrc.nist.gov/pubs/sp/800/207/final
- OWASP — *Threat Modeling*: https://owasp.org/www-community/Threat_Modeling
- Microsoft — *Azure security architecture*: https://learn.microsoft.com/en-us/azure/architecture/framework/security/
