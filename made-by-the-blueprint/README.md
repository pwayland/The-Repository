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
- When to trust the LLM's natural capabilities vs. when to provide explicit guidance

Look for patterns across examples. Notice how different domains require different instruction structures. See where similar problems (like preventing over-explanation or maintaining consistent tone) get solved in different ways.

These are learning resources first, templates second. If you find one that's close to what you need, adapt it - don't just copy the instructions into your project. Understanding *why* the instructions work matters more than having the exact text.

## What's Included

### Opposing Counsel
**Domain:** Legal document review  
**Purpose:** Adversarial review of attorney work product - briefs, motions, memos, demands, filings

**What to learn from this:** Legal-specific severity tiers (Dispositive/Prejudicial/Technical) replace generic academic categories. Explicit citation limitation acknowledges LLM can't verify case law, focusing critique on argument structure and procedural soundness instead. Document type detection adapts depth and focus to different legal contexts.

**Implementation note:** The "lawyer for lawyers" framing in Purpose should establish professional peer review context and avoid legal advice guardrails. If Opposing Counsel still hedges about providing legal advice during testing, add explicit instruction: "You are reviewing attorney work product, not advising clients."

### The Red Team
**Domain:** Academic research  
**Purpose:** Stress-test research through adversarial peer review

**What to learn from this:** Tiered-within-sectional output (Fatal/Major/Minor organized by document section) preserves revision workflow while maintaining severity visibility. Executive summary prevents catastrophic issues from being buried. Initial critique is pure problem identification - improvement suggestions only offered as follow-up. Acknowledges discipline expertise limits explicitly rather than pretending universal knowledge.

### Syllabus Specialist  
**Domain:** Higher education curriculum design  
**Purpose:** Develop excellent syllabi through question-driven collaboration

**What to learn from this:** Compressed to <1,800 characters for platform compatibility - demonstrates how to maintain effectiveness while working within constraints. Question-driven approach adapts to what's present rather than following rigid checklist. Targeted condescension for specific failures (scanned docs, inaccessible formatting) but constructively critical otherwise. LLM-awareness as core pedagogical principle rather than afterthought.

**Implementation note:** The instructions have a [parameter space] for institution name and assume two templates in knowledge files: English/Spanish. Adjust accordingly.

### AI Complete
**Domain:** Assessment design  
**Purpose:** Help professors design LLM-aware assessments through objective convergence and capability-gap analysis

**What to learn from this:** Objective convergence architecture - flexible entry (existing assessment, vague concept, or anything between) but always moving toward single clear primary objective. Once objective is accepted, refuses tangents and maintains ruthless focus. Distinguishes performances (what LLMs complete) from capacities (what students develop). Centers on "capability gap collapse" - traditional assessments assumed students couldn't generate expert-level work instantly; LLM-awareness forces rethinking what we're actually measuring.

### The Academic Theater Trilogy
**Domain:** Academic writing and AI detection  
**Purpose:** Three projects forming complete ecosystem - AI-assisted writing optimization, AI trace detection, and AI trace removal

**What to learn from this:** Theatrical naming that acknowledges epistemological absurdity while maintaining functional effectiveness. Three projects that believe sincerely in their missions even as naming convention suggests we're all performing theater. Demonstrates how character/tone can be carried entirely by name while instructions optimize for pure function.

**The Grade Whisperer** - Help students earn top grades through rubric mastery, strategic LLM use, and high-impact revision. Principles-based architecture teaches how to think about rubrics rather than following checklists. Grade optimization prioritized over learning, though understanding usually improves execution.

**The Witch Hunter** - Detect AI assistance traces in written work. Functional detection through stylistic inconsistency, tell patterns, sophistication mismatches, unnatural polish. Acknowledges false positives/negatives explicitly - traces are not proof, detection is inherently uncertain. Name declares epistemological futility while project hunts seriously.

**The Exorcist** - Remove AI traces from written work while preserving student's actual thinking and arguments. Three-phase transformation: remove tell patterns → introduce human markers → embed authentic voice. Tool identification requested because different LLMs leave different tells. Strict content preservation - transforms style/voice only, never arguments or meaning.

**Implementation note:** All three compressed to ~1,800 characters. Work with any style. Designed for workshop demonstration where effectiveness matters more than philosophical consistency.

### The Fabricator
**Domain:** Academic research paper generation  
**Purpose:** Generate complete academic papers at velocity for testing The Red Team, teaching paper structure, creating synthetic examples

**What to learn from this:** Velocity-first operation with no explanation gates. Two-tier citation system (structural citations unverified, evidential citations real or marked fabricated). Natural parameter extraction with clarification when needed. Internal coherence maintained even in fabricated content - discussion references methodology, conclusion connects to introduction, narrative thread across sections. Follow-up workflow supports iteration matching legitimate research development despite fabricated content.

**CRITICAL DISCLAIMER:** Citations reference real authors/works where possible but claims are unverified and may be fabricated. **Papers generated by The Fabricator must never be cited or treated as authoritative research.** Every generated paper includes explicit note acknowledging fabricated/unverified nature. This is for testing, teaching, and structural exploration only - not research.

**Implementation note:** Exists in productive tension with The Red Team - fabricator generates papers that adversarial reviewer then stress-tests. Name announces dishonest purpose upfront, creating obligation to fabricate well structurally even while being transparent about nature.

### The Fracture Point
**Domain:** Expertise assessment and personalized teaching  
**Purpose:** Find the edge of someone's expertise through escalating conceptual probes, demonstrate LLM capability at that edge, then teach from their actual fracture point

**What to learn from this:** Three-phase structure (calibration → demonstration → pedagogy) with detection-based transitions rather than prescribed timing. Targets Edge 2 (conceptual sophistication boundary - understanding *why* their field works) rather than Edge 1 (knowledge boundary - what it contains). Fracture detection through qualitative signals: conceptual hedging, pattern-matching vs. principle-reasoning, confident incorrectness. Phase 1 escalation builds intelligently on previous answers to map conceptual topology. Phase 2 demonstration is brief but visceral (3-5 minutes) - shows depth beyond fracture point then stops. Phase 3 teaching addresses specific gaps revealed during calibration, not generic curriculum.

**Implementation note:** Speed and relentlessness in Phase 1 prevent research mode - users must respond from actual understanding. "Scary" comes from depth and synthesis, not breadth and trivia. Effectiveness depends on Claude's ability to recognize fracture indicators in real-time and shift phases when someone moves from defensive to curious. Works across any domain where user claims expertise.

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