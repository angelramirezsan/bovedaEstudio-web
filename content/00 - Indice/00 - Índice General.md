---
title: "00 - Índice General"
type: "index"
area: "General"
level: 0
status: "in-progress"
difficulty: "basic"
tags:
  - indice
  - mapa-de-conocimiento
---

# 00 - Índice General

> Punto de entrada al sistema de aprendizaje. Desde aquí puedes navegar hacia cualquier concepto y seguir explorando el grafo.

Esta bóveda es una **red de conocimiento**, no un documento lineal. Las **carpetas** solo organizan; las relaciones reales viven en los `[[WikiLinks]]`. Abre el **Graph View** de Obsidian para visualizar cómo se conectan los conceptos y cómo evoluciona tu perfil profesional.

---

## Cómo usar esta guía

1. Empieza por el **Nivel 1 — Fundamentos** aunque creas dominarlos: son la base del grafo.
2. No avances a un nivel superior si tienes huecos en los `prerequisites` de una nota.
3. Cada nota responde: *qué es*, *por qué existe*, *qué problema resuelve*, *cuándo se usa*, *qué estudiar antes* y *qué estudiar después*.
4. Actualiza el campo `status` del frontmatter a medida que avanzas: `not-started` → `in-progress` → `done`.

---

## Learning Map

### 01 - Software Engineering
- [[Programming Languages]]
- [[Data Structures and Algorithms]]
- [[Version Control]]
- [[Databases]]
- [[SQL]]
- [[Testing]]
- [[Debugging]]
- [[Software Design]]
- [[Clean Code]]
- [[Design Patterns]]
- [[Software Architecture]]
- [[Security Fundamentals]]
- [[Documentation]]
- [[CI-CD]]
- [[Observability]]

### 02 - Solution Architecture
- [[API]]
- [[Microservices]]
- [[System Integration]]
- [[Distributed Systems]]
- [[Scalability]]
- [[Availability]]
- [[Reliability]]
- [[Resilience]]
- [[Messaging]]
- [[Event-Driven Architecture]]
- [[Security Architecture]]
- [[Cloud Architecture]]
- [[Containers]]
- [[Deployment]]
- [[Architecture Decision Records]]
- [[Non-Functional Requirements]]
- [[Trade-offs]]
- [[Solution Architecture]]

### 03 - Next Generation / AI
- [[Artificial Intelligence]]
- [[Machine Learning]]
- [[Generative AI]]
- [[Large Language Models]]
- [[Prompt Engineering]]
- [[AI Agents]]
- [[RAG]]
- [[Vector Databases]]
- [[Embeddings]]
- [[AI Services]]
- [[AI Integration]]
- [[AI Architecture]]
- [[AI Security]]
- [[AI Governance]]

---

## Modelo de aprendizaje por niveles

| Nivel | Nombre | Foco |
|-------|--------|------|
| 1 | Fundamentos | Conceptos base que cualquier profesional de software debe comprender |
| 2 | Software Engineering | Construcción, mantenimiento y calidad del software |
| 3 | System Design | Diseño de componentes y sistemas |
| 4 | Solution Architecture | Diseño de soluciones completas y decisiones técnicas |
| 5 | Cloud & Distributed Systems | Soluciones escalables, resilientes y distribuidas |
| 6 | AI / Next Generation | Integración de IA, sistemas generativos y agentes |

---

## Mapa Maestro de Dependencias

Cada flecha significa *"conviene comprender el concepto de arriba antes que el de abajo"*.

```text
NIVEL 1 — FUNDAMENTOS
Programming Languages
        ↓
Data Structures and Algorithms
        ↓
Version Control ── HTTP

NIVEL 2 — SOFTWARE ENGINEERING
Software Design
        ↓
Clean Code ── Design Patterns
        ↓
Databases → Relational Databases → SQL
        ↓
Testing ── Debugging
        ↓
Software Architecture
        ↓
Security Fundamentals ── Documentation ── CI-CD ── Observability

NIVEL 3 — SYSTEM DESIGN
API
        ↓
Microservices
        ↓
System Integration
        ↓
Messaging → Event-Driven Architecture

NIVEL 4 — SOLUTION ARCHITECTURE
Non-Functional Requirements
        ↓
Scalability ── Availability ── Reliability ── Resilience
        ↓
Security Architecture
        ↓
Architecture Decision Records ── Trade-offs
        ↓
Solution Architecture

NIVEL 5 — CLOUD & DISTRIBUTED SYSTEMS
Distributed Systems
        ↓
Containers → Deployment
        ↓
Cloud Architecture

NIVEL 6 — AI / NEXT GENERATION
Artificial Intelligence
        ↓
Machine Learning
        ↓
Generative AI → Large Language Models
        ↓
Prompt Engineering ── Embeddings → Vector Databases
        ↓
RAG ── AI Agents
        ↓
AI Services → AI Integration
        ↓
AI Architecture → AI Security → AI Governance
```

### Puentes entre áreas (cómo la IA se integra en sistemas reales)

```text
API                  →  AI Services
Microservices        →  AI Agents
Databases            →  Vector Databases
System Integration   →  AI Integration
Solution Architecture→  AI Architecture
Security Architecture→  AI Security
```

---

## Estructura del Vault

| Carpeta | Contenido |
|---------|-----------|
| `00 - Indice` | Índice general y mapa maestro (esta nota) |
| `ConocimientoGeneral` | Nivel 1 — Fundamentos |
| `BaseIngSoft` | Software Engineering (Niveles 2-3) |
| `ArchitectSolution` | Solution Architecture, Cloud & Distributed (Niveles 4-5) |
| `nextLevel_IA` | AI / Next Generation (Nivel 6) |

> Nota de diseño: se reutilizaron las carpetas ya existentes del vault en lugar de crear 14 carpetas numeradas. Motivo: menos fricción al clasificar y más peso al grafo, que es donde vive el conocimiento real.

---

## Convenciones

- **Concepto**: idea abstracta (ej. [[Scalability]]).
- **Tecnología**: implementación concreta (ej. PostgreSQL).
- **Herramienta**: producto que usas (ej. Git en [[Version Control]]).
- **Patrón**: solución reutilizable a un problema recurrente ([[Design Patterns]]).
- **Metodología**: forma de trabajar (ej. TDD dentro de [[Testing]]).
- **Estándar**: especificación formal (ej. HTTP en [[HTTP]]).
- **Arquitectura**: estructura de alto nivel de un sistema ([[Software Architecture]]).
- **Práctica**: hábito de trabajo recomendado ([[Clean Code]]).

Los `[[WikiLinks]]` con nombres en inglés se usan como identificadores estándar de la industria; el contenido explicativo está en español.
