---
title: "Senate AI Workshop — Strategic LLM Applications for Institutional Transformation"
source: manual
owner: Paul Wayland
last-updated: 2026-04-07
---

# Senate AI Workshop

Strategic LLM applications for institutional transformation.

**Workshop Date:** 2026 (TBD)
**Facilitator:** Paul Wayland
**Institution:** Inter American University of Puerto Rico — Metro Campus

---

## What This Is

This repository serves two purposes:

1. **Workshop materials** for the Academic Senate AI Workshop — prompt guides, provocations, quick reference, and resources.
2. **Institutional knowledge base** — structured data about programs, enrollment, and labor markets, prepared for use as LLM context.

Everything here is public. The knowledge base files are designed to be copied directly into any LLM conversation as context for institutional analysis.

---

## Workshop Overview

A 2-hour, platform-agnostic, hands-on session for academic senate members and institutional leaders. Five phases:

| Phase | Topic | What Happens |
|-------|-------|--------------|
| 1 | The Ideal Prompt | From the basic formula to effective institutional prompts |
| 2 | Context in Action | Live demo: how a single context file transforms LLM output |
| 3 | Shared Context | Hands-on: using the knowledge base for institutional analysis |
| 4 | AI Burnout | The costs nobody mentions — two types of burnout facing adopters |
| 5 | Resources & Next Steps | Tools, references, and where to go from here |

The central thesis: **the prompt tells the LLM what to do; context tells it who you are and what you know.** Context is intelligence.

---

## Repository Structure

```
workshop/               Workshop delivery materials
  prompt-guide.md         Core guide: building effective prompts and context
  provocation.md          Honest challenges for institutional thinking
  quick-reference.md      Printable one-page reference card
  resources.md            External resources and tools

catalog/                Knowledge base: 146 academic programs (generated from YAML)
  gen-ed-requirements.md  General education requirements (bachelor + associate)
  programs-business-*.md  Business & Management (21 programs, 2 files)
  programs-education-*.md Education (19 programs, 2 files)
  programs-health-*.md    Health Sciences (17 programs, 2 files)
  programs-engineering-*  Engineering & Technology (17 programs, 2 files)
  programs-sciences-*.md  Natural Sciences & Math (20 programs, 2 files)
  programs-arts-media-*   Arts, Design & Media (17 programs, 2 files)
  programs-social-*.md    Social Sciences & Humanities (14 programs)
  programs-other.md       Criminal Justice, Hospitality, Agriculture, Sports, Other (18 programs)

institutional/          Knowledge base: institutional context (curated)
  enrollment-data.md      Enrollment trends 2020–2024 (IPEDS data)

data/                   Reference data
  CSV_182026-218.csv      IPEDS data export
  accounting-positions-1-2026  Job market compilation
```

---

## How to Use This Repository

### Workshop Participants

1. Browse `workshop/` for the prompt guide and reference materials.
2. Copy any file from `catalog/`, `institutional/`, or `data/` into an LLM conversation as context.
3. Use the prompt templates in the quick reference to run your own institutional analyses.

### Other Institutions

These materials are designed around Inter American University — Metro Campus, but the methods are transferable. To adapt:

- Replace the knowledge base files with your own institutional data.
- Modify prompt templates with your context (enrollment, programs, labor market).
- The workshop structure (ideal prompt → context demo → shared knowledge base → burnout) works for any audience learning to use LLMs strategically.

---

## The Knowledge Base

The `catalog/`, `institutional/`, and `data/` folders contain structured information about Inter Metro. These files follow a standard format:

- YAML frontmatter (title, source, owner, date)
- 200–400 lines each, independently useful
- Catalog data is in Spanish (from SmartCatalog source)
- Institutional data is in Spanish (IPEDS public data)

These files are not summaries or reports. They are **context files** — structured so that an LLM can use them as working knowledge when responding to institutional questions.

---

## Privacy and Ethics

- No confidential student information (FERPA compliance)
- No proprietary institutional data without authorization
- No personnel information or sensitive strategic plans
- All enrollment data is from public federal sources (IPEDS)
- Use representative examples or anonymized data for practice

LLM outputs should always be verified against authoritative sources before use in institutional decision-making.

---

## Contact

**Paul Wayland**
Email: pwayland@intermetro.edu
Office: 317

---

## En Español

Este repositorio contiene materiales para el Taller de IA del Senado Académico de la Universidad Interamericana — Recinto Metro. Incluye:

- **workshop/** — Guía de prompts, provocaciones, referencia rápida y recursos.
- **catalog/** — Base de conocimiento: programas académicos generados desde datos curriculares.
- **institutional/** — Base de conocimiento: datos institucionales curados (matrícula, tendencias).
- **data/** — Datos de referencia (IPEDS, mercado laboral).

Los archivos de la base de conocimiento están diseñados para copiarse directamente en cualquier conversación con un LLM como contexto para análisis institucional. Todos los datos de matrícula provienen de fuentes públicas federales (IPEDS).

**Tesis central del taller:** El prompt le dice al LLM qué hacer; el contexto le dice quién eres y qué sabes. El contexto es inteligencia.
