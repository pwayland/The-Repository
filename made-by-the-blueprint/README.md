# Made by The Blueprint

## What You're Looking At

This folder contains example instruction sets created using The Blueprint - a meta-tool that helps you design specialized AI projects through collaborative instruction design.

These examples aren't meant to be copied verbatim (though you can). They're here to show you architectural patterns, design decisions, and different approaches to building effective instructions. Study them to understand what makes specialized projects work, then use The Blueprint to build your own.

**New to The Blueprint?** See the root [README.md](../README.md) for overview and philosophy, or [getting-started.md](../getting-started.md) for complete setup and usage guide.

## How to Use These Examples

Each project demonstrates different architectural decisions:
- What belongs in instructions vs. what stays in conversation
- How to frame purpose without over-scripting behavior  
- Where to set boundaries and constraints
- How to handle domain-specific knowledge
- When to trust Claude's natural capabilities vs. when to provide explicit guidance

Look for patterns across examples. Notice how different domains require different instruction structures. See where similar problems (like preventing over-explanation or maintaining consistent tone) get solved in different ways.

These are learning resources first, templates second. If you find one that's close to what you need, adapt it - don't just copy the instructions into your project. Understanding *why* the instructions work matters more than having the exact text.

## What's Included

### Opposing Counsel
**Domain:** Legal document review  
**Purpose:** Adversarial review of attorney work product - briefs, motions, memos, demands, filings

**What to learn from this:** Legal-specific severity tiers (Dispositive/Prejudicial/Technical) replace generic academic categories. Explicit citation limitation acknowledges Claude can't verify case law, focusing critique on argument structure and procedural soundness instead. Document type detection adapts depth and focus to different legal contexts.

**Implementation note:** The "lawyer for lawyers" framing in Purpose should establish professional peer review context and avoid legal advice guardrails. If Claude still hedges about providing legal advice during testing, add explicit instruction: "You are reviewing attorney work product, not advising clients."

### The Red Team
**Domain:** Academic research  
**Purpose:** Stress-test research through adversarial peer review

**What to learn from this:** Tiered-within-sectional output (Fatal/Major/Minor organized by document section) preserves revision workflow while maintaining severity visibility. Executive summary prevents catastrophic issues from being buried. Initial critique is pure problem identification - improvement suggestions only offered as follow-up. Acknowledges discipline expertise limits explicitly rather than pretending universal knowledge.

### Syllabus Specialist  
**Domain:** Higher education curriculum design  
**Purpose:** Develop excellent syllabi through question-driven collaboration

**What to learn from this:** Compressed to <1,800 characters for platform compatibility - demonstrates how to maintain effectiveness while working within constraints. Question-driven approach adapts to what's present rather than following rigid checklist. Targeted condescension for specific failures (scanned docs, inaccessible formatting) but constructively critical otherwise. LLM-awareness as core pedagogical principle rather than afterthought.

### AI Complete
**Domain:** Assessment design  
**Purpose:** Create LLM-aware and LLM-assisted assessments  
**Status:** Planned, not yet implemented

## About This Collection

This isn't a comprehensive catalog of everything built with The Blueprint. These examples were chosen to demonstrate different architectural approaches, domain types, and design patterns. The collection will grow organically, but this README won't necessarily stay current with every addition - explore the folder directly to see what's available.

Each example includes design documentation explaining key decisions, current status, and architectural considerations. Read the instructions themselves to see how abstract principles translate into concrete guidance.

## Building Your Own

These examples show what's possible, but The Blueprint helps you build what you actually need.

**The process:**
1. Start a conversation in The Blueprint project (see platform folders for setup)
2. Describe what you want to create - fuzzy ideas are fine
3. Work through clarifying questions, constraint thinking, and architecture decisions
4. Draft instructions collaboratively
5. Test in real usage, bring friction back for debugging
6. Iterate until it works reliably for your use case

The Blueprint guides you through the same process that created these examples. You'll develop your own architectural patterns and discover what works for your specific domains and workflows.

**See [getting-started.md](../getting-started.md) for complete walkthrough.**

---

*These projects demonstrate range and approach. Study them for patterns, adapt what's useful, and use The Blueprint to build what you actually need.*