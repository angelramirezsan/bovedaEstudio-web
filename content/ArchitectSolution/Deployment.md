---
title: "Deployment"
type: "practice"
area: "Solution Architecture"
level: 5
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Containers]]"
  - "[[CI-CD]]"
related:
  - "[[Cloud Architecture]]"
  - "[[Observability]]"
tags:
  - solution-architecture
  - devops
---

# Deployment

## ¿Qué es?
El despliegue (deployment) es el proceso de poner una versión del software en un entorno donde los usuarios (o pruebas) puedan usarlo. Es el paso de "el código está listo" a "el código está funcionando en producción".

**Definición técnica:** conjunto de actividades para instalar, configurar y activar una versión de software en un entorno objetivo, buscando hacerlo de forma repetible, segura y con mínimo impacto en el servicio.

---

## ¿Por qué existe?
Tener código que funciona no sirve si no llega a los usuarios de forma fiable. Desplegar a mano es lento y arriesgado. El despliegue como disciplina existe para llevar los cambios a producción de manera segura y repetible.

---

## ¿Qué problema resuelve?
- Llevar cambios a producción sin romper el servicio.
- Reducir el riesgo y el tiempo de inactividad durante una actualización.
- Poder revertir rápidamente si algo sale mal.

---

## ¿Cómo funciona?
Se automatiza mediante [[CI-CD]] y suele desplegar [[Containers]]. Existen estrategias para reducir el riesgo:
- **Blue-green**: dos entornos idénticos; se cambia el tráfico de uno a otro.
- **Canary**: liberar el cambio a un pequeño porcentaje de usuarios primero.
- **Rolling**: actualizar instancias gradualmente.

Tras desplegar, la [[Observability]] confirma que todo va bien y permite revertir (rollback) si no.

---

## Ejemplo sencillo
Es como abrir un puente nuevo. En lugar de desviar todo el tráfico de golpe (arriesgado), primero dejas pasar unos pocos coches (canary), compruebas que aguanta, y luego abres al resto. Si algo falla, cierras el puente nuevo y todos vuelven al antiguo (rollback).

---

## Conceptos relacionados
- [[CI-CD]] — automatiza y dispara el despliegue.
- [[Containers]] — la unidad que se despliega habitualmente.
- [[Cloud Architecture]] — provee la infraestructura donde se despliega.
- [[Observability]] — verifica que el despliegue fue exitoso.

---

## Antes de estudiar esto
- [[Containers]]
- [[CI-CD]]

---

## Después de estudiar esto
- [[Cloud Architecture]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre "código listo" y "código desplegado"?
2. ¿Qué ventaja tiene un despliegue canary frente a uno de golpe?
3. ¿Qué es un rollback y cuándo se usa?
4. ¿Cómo confirma la observabilidad que un despliegue fue bien?

---

## Errores comunes
- Desplegar de golpe a todos los usuarios sin plan de rollback.
- No monitorear tras el despliegue y enterarse tarde de los fallos.
- Procesos manuales imposibles de repetir de forma idéntica.

---

## Resumen
- Es poner una versión del software a funcionar en un entorno.
- Se automatiza con CI/CD y suele desplegar contenedores.
- Estrategias como blue-green, canary y rolling reducen el riesgo.
- La observabilidad valida el resultado y habilita rollback.
- Busca ser repetible, seguro y de bajo impacto.

---

## Fuentes
- Google — *SRE Book: Release Engineering*: https://sre.google/sre-book/release-engineering/
- Martin Fowler — *BlueGreenDeployment*: https://martinfowler.com/bliki/BlueGreenDeployment.html
- AWS — *Deployment strategies*: https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/introduction.html
