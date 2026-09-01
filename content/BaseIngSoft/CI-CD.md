---
title: "CI-CD"
aliases:
  - "CI/CD"
  - "Continuous Integration"
  - "Continuous Delivery"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Version Control]]"
  - "[[Testing]]"
related:
  - "[[Deployment]]"
  - "[[Observability]]"
  - "[[Containers]]"
tags:
  - software-engineering
  - devops
---

# CI-CD

> Nota de nomenclatura: el término estándar es **CI/CD**, pero se usa el título `CI-CD` porque la barra `/` en un nombre de nota rompe los `[[WikiLinks]]` en Obsidian (la interpreta como carpeta). El alias `CI/CD` está declarado en el frontmatter.

## ¿Qué es?
CI/CD es la práctica de automatizar la integración, prueba y entrega del software. Cada vez que alguien cambia el código, un proceso automático lo compila, lo prueba y (opcionalmente) lo despliega, sin pasos manuales.

**Definición técnica:** CI (Integración Continua) integra y valida cambios de código de forma frecuente y automática. CD puede significar Entrega Continua (Continuous Delivery: siempre listo para desplegar) o Despliegue Continuo (Continuous Deployment: se despliega automáticamente). Se implementa mediante *pipelines*.

---

## ¿Por qué existe?
Integrar y desplegar a mano es lento, propenso a errores y desalienta hacer cambios pequeños y frecuentes. CI/CD existe para que entregar software sea rápido, repetible y confiable.

---

## ¿Qué problema resuelve?
- El "funciona en mi máquina" y los errores de integración tardíos.
- Despliegues manuales lentos, arriesgados y difíciles de repetir.
- Ciclos de entrega largos que retrasan el valor al usuario.

---

## ¿Cómo funciona?
Un **pipeline** define etapas automáticas que se disparan con cada cambio en el [[Version Control]]: compilar → ejecutar [[Testing]] → construir artefactos (a menudo [[Containers]]) → desplegar a un entorno. Si una etapa falla, el pipeline se detiene y avisa. Esto permite integrar muchas veces al día con confianza.

---

## Ejemplo sencillo
Es como una cadena de montaje automatizada: cada pieza que entra pasa por controles y ensamblaje sin intervención manual. Si una pieza no pasa el control de calidad, la línea se detiene antes de que el defecto llegue al cliente.

---

## Conceptos relacionados
- [[Version Control]] — los cambios en el repositorio disparan el pipeline.
- [[Testing]] — las pruebas automáticas son el corazón de CI.
- [[Deployment]] — CD automatiza la entrega a los entornos.
- [[Containers]] — empaquetan el software de forma reproducible para desplegar.

---

## Antes de estudiar esto
- [[Version Control]]
- [[Testing]]

---

## Después de estudiar esto
- [[Deployment]]
- [[Observability]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre Entrega Continua y Despliegue Continuo?
2. ¿Por qué las pruebas automáticas son esenciales en un pipeline de CI?
3. ¿Qué ventaja tiene integrar cambios pequeños y frecuentes?
4. ¿Qué debe pasar cuando una etapa del pipeline falla?

---

## Errores comunes
- Tener CI sin pruebas reales: automatiza compilar pero no valida nada.
- Confundir Continuous Delivery con Continuous Deployment.
- Pipelines lentos que el equipo empieza a ignorar o saltar.

---

## Resumen
- CI/CD automatiza integración, prueba y entrega del software.
- Se implementa con pipelines disparados por cada cambio.
- Reduce errores de integración y acelera la entrega.
- CD puede ser entrega o despliegue continuo.
- Se apoya en control de versiones, testing y contenedores.

---

## Fuentes
- Martin Fowler — *Continuous Integration*: https://martinfowler.com/articles/continuousIntegration.html
- GitLab — *CI/CD concepts*: https://docs.gitlab.com/ee/ci/
- AWS — *What is CI/CD?*: https://aws.amazon.com/devops/continuous-integration/
