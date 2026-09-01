---
title: "Containers"
type: "technology"
area: "Solution Architecture"
level: 5
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Microservices]]"
related:
  - "[[Deployment]]"
  - "[[CI-CD]]"
  - "[[Cloud Architecture]]"
tags:
  - solution-architecture
  - devops
---

# Containers

## ¿Qué es?
Un contenedor empaqueta una aplicación junto con todo lo que necesita para ejecutarse (librerías, dependencias, configuración), de forma que corra igual en cualquier máquina. Resuelve el clásico "en mi máquina funciona".

**Definición técnica:** un contenedor es una unidad de software estandarizada que aísla una aplicación y sus dependencias a nivel de sistema operativo, compartiendo el kernel del host. Docker popularizó el formato; Kubernetes orquesta contenedores a escala.

---

## ¿Por qué existe?
El software se comportaba distinto según el entorno (desarrollo, pruebas, producción) por diferencias de dependencias. Los contenedores existen para empaquetar todo junto y garantizar ejecución reproducible en cualquier lugar.

---

## ¿Qué problema resuelve?
- El "en mi máquina funciona" por diferencias de entorno.
- Despliegues inconsistentes entre desarrollo y producción.
- Aprovechar mejor los recursos que una máquina virtual completa.

---

## ¿Cómo funciona?
A partir de una **imagen** (plantilla inmutable con la app y sus dependencias) se crean **contenedores** en ejecución. A diferencia de una máquina virtual, no incluyen un sistema operativo completo: comparten el kernel del host, por lo que son ligeros y rápidos. A gran escala se **orquestan** (Kubernetes) para desplegarlos, escalarlos y recuperarlos automáticamente. Son la unidad natural de despliegue de [[Microservices]] y encajan en [[CI-CD]].

---

## Ejemplo sencillo
Es como un contenedor marítimo estandarizado: no importa qué lleve dentro, encaja igual en cualquier barco, camión o grúa del mundo. Antes, cada carga necesitaba manejo especial; el estándar lo simplificó todo. Los contenedores de software hacen lo mismo con las aplicaciones.

---

## Conceptos relacionados
- [[Microservices]] — se empaquetan y despliegan naturalmente como contenedores.
- [[Deployment]] — los contenedores son la unidad de despliegue moderna.
- [[CI-CD]] — los pipelines construyen imágenes de contenedor.
- [[Cloud Architecture]] — la nube ofrece servicios gestionados de contenedores.

---

## Antes de estudiar esto
- [[Microservices]]

---

## Después de estudiar esto
- [[Deployment]]
- [[Cloud Architecture]]

---

## Preguntas de comprobación
1. ¿Qué problema resuelve un contenedor respecto a los entornos?
2. ¿En qué se diferencia un contenedor de una máquina virtual?
3. ¿Qué diferencia hay entre una imagen y un contenedor?
4. ¿Para qué sirve un orquestador como Kubernetes?

---

## Errores comunes
- Confundir contenedores con máquinas virtuales (los contenedores comparten kernel).
- Meter demasiadas responsabilidades en un solo contenedor.
- Guardar datos importantes dentro del contenedor, que es efímero por diseño.

---

## Resumen
- Empaquetan la app con sus dependencias para ejecución reproducible.
- Más ligeros que las máquinas virtuales: comparten kernel.
- De una imagen se crean contenedores en ejecución.
- Se orquestan a escala con Kubernetes.
- Son la unidad de despliegue de los microservicios.

---

## Fuentes
- Docker — *Docker Documentation*: https://docs.docker.com/
- CNCF — *Kubernetes Documentation*: https://kubernetes.io/docs/home/
