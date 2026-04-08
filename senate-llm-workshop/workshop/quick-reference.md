---
title: "Quick Reference — Senate AI Workshop"
source: manual
owner: Paul Wayland
last-updated: 2026-04-07
---

# Quick Reference

Printable one-page card for the Senate AI Workshop.

---

## The Prompt Formula

| Component | What It Does | Example |
|-----------|-------------|---------|
| **Task** | What you need done | "Identify the 3 most vulnerable programs by enrollment and market demand" |
| **Context** | Information the LLM needs | Enrollment data, program structures, job market files |
| **Output** | How you need results | "Table with program name, enrollment trend, market score, and recommendation" |
| **Constraints** | What the LLM should NOT do | "Do not suggest adding budget. Do not hedge." |
| **Role** | Perspective for the analysis | "You are a skeptical accreditation reviewer" |

---

## Three Types of Context

- **Inline** — facts written directly in the prompt. Fast. Limited to what you remember.
- **File-based** — a document attached to the conversation. Writing samples, reports, datasets.
- **Knowledge base** — a structured collection of files representing institutional knowledge. Scales across people and conversations.

---

## Three Institutional Prompts

### 1. Grant Opportunity Research

```
ROLE: Grant reviewer who has rejected 80% of applications this cycle.
TASK: Identify 5 federal grant opportunities aligned with our priorities.
CONTEXT: [Attach enrollment-data.md] Priorities: STEM retention, faculty
  development, student mental health. Can manage grants up to $500K.
OUTPUT: Table (agency, program, max award, alignment, deadline,
  competitiveness). For top 3: why we fit, what is required, realistic odds.
CONSTRAINTS: Only opportunities where we have genuine competitive
  advantage. No aspirational long-shots.
```

### 2. Curriculum Gap Analysis

```
ROLE: Hiring manager screening graduates from our program.
TASK: Compare [program] curriculum against job market requirements.
CONTEXT: [Attach program file from catalog/] [Attach job market data]
OUTPUT: List of critical gaps (50%+ of postings), Market Readiness Score
  (0-100), and a specific course proposal to close the top 3 gaps.
CONSTRAINTS: Do not recommend adding credit hours. Do not suggest
  the professional exam compensates for skill gaps.
```

### 3. Enrollment Strategy

```
ROLE: Enrollment consultant who will not be renewed if enrollment
  does not increase by 5% next cycle.
TASK: Generate 5 recruitment strategies for [target population].
CONTEXT: [Attach enrollment-data.md] 40% decline over 4 years. 49%
  working adults. 99% from Puerto Rico. Budget: existing staff + $10K.
OUTPUT: For each strategy: specific actions, timeline (90 days),
  responsible party, success metric, and cost estimate.
CONSTRAINTS: Must be implementable with existing staff.
  No strategies requiring new hires or capital investment.
```

---

## Three Signs of a Bad Prompt

1. **Generic output** — you forgot to include context about your institution.
2. **Unusable output** — you forgot to specify constraints (budget, timeline, resources).
3. **Consultant-speak** — you asked for "best practices" instead of solving a specific problem.

---

## Ethics Checklist

- No confidential student data (FERPA)
- No personnel information
- No sensitive strategic plans in shared/public LLM platforms
- Use anonymized or representative data for practice
- Verify all LLM outputs against authoritative sources
- Cite LLM assistance in formal documents when appropriate

---

## AI Burnout Warning Signs

- Feeling dread about "falling behind" on AI developments — this is structural, not personal. You cannot keep up. Choose depth over breadth.
- Losing track of time during AI-assisted work sessions — strategic thinking is high-intensity cognitive work. Set time boundaries.
- Mental fatigue disproportionate to apparent activity — "just typing" can be as exhausting as any demanding professional task.
- Guilt about not learning fast enough — the field moves faster than any individual can track. Acceptance is the productive response.

---

## Referencia Rápida — En Español

### La Fórmula

| Componente | Qué Hace |
|------------|----------|
| **Tarea** | Qué necesitas que haga |
| **Contexto** | Información que el LLM necesita (en línea, archivos, base de conocimiento) |
| **Formato** | Cómo necesitas los resultados |
| **Restricciones** | Qué NO debe hacer |
| **Rol** | Perspectiva para el análisis |

### Tres Señales de un Mal Prompt

1. Respuesta genérica — falta contexto institucional.
2. Respuesta inutilizable — faltan restricciones de recursos.
3. Lenguaje de consultor — pediste "mejores prácticas" en vez de resolver un problema concreto.

### Lista de Ética

- Sin datos confidenciales de estudiantes (FERPA)
- Sin información de personal
- Verificar resultados contra fuentes autorizadas
- Citar asistencia de LLM en documentos formales

### Señales de Agotamiento por IA

- Ansiedad por "quedarse atrás" — es estructural, no personal.
- Perder noción del tiempo en sesiones con IA — establecer límites.
- Fatiga desproporcionada a la actividad aparente — el pensamiento estratégico es trabajo cognitivo intenso.
