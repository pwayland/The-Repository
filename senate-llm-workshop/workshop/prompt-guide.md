---
title: "Prompt Guide — From Formula to Context"
source: manual
owner: Paul Wayland
last-updated: 2026-04-07
---

# Prompt Guide

How to move from generic LLM interactions to institutional intelligence.

---

## The Starting Formula

Most prompt guidance begins here:

```
TASK + CONTEXT + OUTPUT FORMAT
```

- **Task:** What you need done.
- **Context:** Information the LLM needs to do it well.
- **Output format:** How you need the results delivered.

This formula works. It is the difference between "analyze our enrollment" (vague, generic response) and a prompt that produces something you can act on. But it is not enough.

---

## Beyond the Formula

The formula gets you from bad to adequate. To get from adequate to genuinely useful, add two elements:

```
TASK + CONTEXT + OUTPUT FORMAT + CONSTRAINTS + ROLE
```

**Constraints** — what the LLM should *not* do:

- "Do not suggest strategies requiring budget increases."
- "Focus only on programs with enrollment below 50 students."
- "Do not hedge. If the data says a program is failing, say so."

Constraints prevent the LLM from producing the diplomatic, everything-is-fine output that is its default. Without constraints, you get a consultant report. With them, you get analysis.

**Role** — who the LLM should be:

- "You are a skeptical accreditation reviewer."
- "You are a hiring manager screening accounting graduates."
- "You are a grant reviewer looking for reasons to reject this proposal."

Role shifts the LLM's perspective. The same data, analyzed by a "supportive advisor" versus a "skeptical reviewer," produces very different — and complementarily useful — outputs.

---

## Context Is Intelligence

This is the central idea of this workshop.

The prompt tells the LLM what to do. Context tells it who you are and what you know. A brilliant prompt with no context produces generic output. A simple prompt with rich context produces institutional intelligence.

There are three types of context:

### 1. Inline Context

Information written directly into the prompt.

```markdown
TASK: Analyze retention strategies for our campus.
CONTEXT: Private university in Puerto Rico. Enrollment declined 40% from
2020 to 2024. 49% of students are working adults (25-64). 70% are
Pell-eligible. Top withdrawal reason is work schedule conflicts.
```

Inline context is fast and sufficient for one-off questions. Its limit: you retype it every time, and you are constrained by what you remember to include.

### 2. File-Based Context

A document — a report, a dataset, a writing sample — provided to the LLM as an attachment or pasted into the conversation.

In the workshop demonstration, a recommendation letter prompt with no context produces generic academic language. The same prompt with a single previous letter as a style sample produces output matching the author's voice, tone, and rhetorical patterns. The LLM did not become a better writer. It received better context.

File-based context is powerful for tasks where the LLM needs to work with specific documents: analyzing reports, matching a writing style, auditing a curriculum against job market data.

### 3. Knowledge-Base Context

A collection of structured files that represent institutional knowledge. This repository is an example. The `catalog/`, `institutional/`, and `data/` folders contain program structures, enrollment trends, and labor market data — all formatted for LLM consumption.

Knowledge-base context is the most powerful type because it scales. One person structures the data; everyone in the institution can use it. The LLM does not need to guess about your programs, your enrollment, or your market. It has the data.

---

## Anatomy of a Strong Institutional Prompt

Here is one prompt, fully annotated:

```markdown
ROLE: You are a workforce analyst evaluating whether a university
program prepares graduates for actual employer requirements.
Do not be diplomatic.

TASK: Compare our Accounting BBA curriculum against real job
posting requirements from Puerto Rico's accounting labor market.
Identify critical gaps where the curriculum fails to prepare
graduates for what employers actually demand.

CONTEXT:
- [Attach: programs-business-1.md — the Accounting BBA structure]
- [Attach: accounting-positions-1-2026.md — job market data]
- The program has a single 3-credit technology course (ACCT 3030)
  covering all software competencies.
- 70%+ of job postings require QuickBooks proficiency.
- 90%+ require advanced Excel (pivot tables, macros, VLOOKUPs).

OUTPUT FORMAT:
1. List of critical skill gaps (appearing in 50%+ of postings)
   with the curriculum's current coverage of each.
2. A "Market Readiness Score" (0-100) with justification.
3. A specific 2-course proposal (6 credits) to close the
   top gaps, with learning outcomes and tools taught.

CONSTRAINTS:
- Base analysis only on the attached data, not general knowledge.
- Do not recommend adding credit hours to the program.
- Do not suggest the CPA exam compensates for software gaps.
```

### What makes this work

- **Role** sets adversarial framing — the LLM will not soften findings.
- **Task** is specific: compare curriculum X against data Y, find gaps.
- **Context** includes both structured files and key facts the LLM should weight heavily.
- **Output** specifies exactly what deliverables are needed.
- **Constraints** prevent the three most common escape routes the LLM would otherwise take.

---

## Three Signs You Are Asking the Wrong Question

### Sign 1: The output is generic

You asked:

```markdown
How can we improve student retention?
```

You got standard retention advice applicable to any institution anywhere.

**Why it failed:** No context about your students, your institution, your constraints.

Fix it:

```markdown
Analyze retention strategies specifically effective for working adult
students (avg age 28) at commuter campuses in Puerto Rico, where 70%
work full-time and cite "work schedule conflicts" as top withdrawal
reason. Focus on scheduling innovations and employer partnerships
that do not require new budget allocation.
```

### Sign 2: You cannot use the output tomorrow

You asked:

```markdown
Give me ideas for recruiting more students.
```

You got 20 recruitment ideas ranging from "improve website" to "build new dormitories."

**Why it failed:** No prioritization, no resource constraints, no timeline.

Fix it:

```markdown
Generate 5 recruitment strategies implementable with $10K budget
and existing staff within 90 days, targeting students within
25-mile radius who inquired but did not apply this cycle.
For each: specific action steps, responsible party, success metric.
```

### Sign 3: The output sounds like a consultant report

You asked:

```markdown
What are best practices for curriculum review?
```

You got a formal process description with committees, timelines, and stakeholder engagement frameworks.

**Why it failed:** You do not need a process manual. You need to solve a specific problem.

Fix it:

```markdown
Our Accounting BBA curriculum has not changed in 8 years. Faculty
resist changes citing "academic rigor." Employers say graduates
lack QuickBooks and advanced Excel skills. I need talking points
for the next curriculum committee meeting that acknowledge faculty
concerns while making the case for specific skill additions. Include
3 courses where software skills could be integrated without adding
credit hours.
```

---

## Common Mistakes

**Over-prompting.** Writing 500 words when 50 would do. If your prompt is longer than the output you want, something is wrong. Be specific, not verbose.

**Under-contexting.** Expecting the LLM to know your institution. It does not. It knows statistical patterns about institutions in general. Your specific enrollment data, program structures, and labor market — those require context files.

**Asking for consensus.** "What should we do about declining enrollment?" invites the LLM to give you safe, balanced, non-controversial recommendations. Instead, ask it to argue a position: "Make the strongest case that Program X should be discontinued based on enrollment and market data." You can always ask for the counter-argument next.

**Treating one conversation as the whole analysis.** A single prompt rarely produces a final answer. Use follow-up prompts to pressure-test, challenge, and refine. The first output is a draft, not a deliverable.

---

## Project Showcase: Context as Institutional Infrastructure

The knowledge base files in this repository were not assembled by hand. They were generated from a structured data project — the Curricular Sequence Visualizer — that models all 146 degree programs as machine-readable YAML data. The same data that powers a student-facing course planning tool also generates the LLM context files used in this workshop.

This illustrates the most durable lesson of this workshop: **context is an investment, not an expense.** Institutional data structured once in a machine-readable format can serve student advising, LLM analysis, accreditation reporting, and program review — all from the same source.

The live demonstration during the workshop walks through this project and shows how structured data becomes institutional intelligence.

---

## Guía de Prompts — En Español

### La Fórmula Expandida

```
TAREA + CONTEXTO + FORMATO DE SALIDA + RESTRICCIONES + ROL
```

- **Tarea:** Qué necesitas que haga.
- **Contexto:** La información que el LLM necesita. Tres tipos: en línea (escrito en el prompt), basado en archivos (documentos adjuntos), y base de conocimiento (colección estructurada de archivos).
- **Formato de salida:** Cómo necesitas los resultados.
- **Restricciones:** Qué NO debe hacer el LLM.
- **Rol:** Desde qué perspectiva debe analizar.

### Tesis Central

El prompt le dice al LLM qué hacer. El contexto le dice quién eres y qué sabes. Un prompt brillante sin contexto produce resultados genéricos. Un prompt simple con contexto rico produce inteligencia institucional.

### Tres Señales de una Mala Pregunta

1. **La respuesta es genérica** — falta contexto sobre tu institución.
2. **No puedes usar la respuesta mañana** — falta especificidad y restricciones de recursos.
3. **La respuesta suena a informe de consultor** — estás pidiendo mejores prácticas en vez de resolver un problema concreto.

### Errores Comunes

- **Sobre-prompting:** Escribir 500 palabras cuando 50 bastan.
- **Sub-contexting:** Esperar que el LLM conozca tu institución sin darle datos.
- **Pedir consenso:** Pedir recomendaciones "balanceadas" en vez de análisis directo.
- **Una conversación = todo el análisis:** El primer resultado es un borrador, no un entregable.
