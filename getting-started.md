# Getting Started with The Blueprint

## Introduction

This guide will walk you through setting up and using The Blueprint to create your first AI project. By the end, you'll understand how to collaborate with The Blueprint to design effective instructions for specialized AI assistants.

**Expected time commitment:**
- Initial setup: 5-10 minutes
- First project build: 20-60 minutes depending on complexity
- Ongoing refinement: As needed when you discover edge cases

**Prerequisites:**
- Access to at least one AI platform (Claude Pro/Team, ChatGPT Plus/Team, or Gemini Advanced/Business)
- A project idea or problem you want to solve (even a fuzzy one is fine)

## Choosing Your Platform

### Claude Projects

**When to use:**
- You have Claude Pro ($20/month) or Claude Team ($30/user/month, 5 user minimum)
- You need excellent context retention and document handling
- Your project involves complex, multi-turn interactions
- You value privacy and don't need public sharing

**How to create a new project:**
1. Open Claude and click "Projects" in the left sidebar
2. Click "Create Project"
3. Name your project "The Blueprint" (or whatever you prefer)
4. In the project settings, add the Blueprint instructions to "Project knowledge"

**Platform-specific tips:**
- Claude's 200K token context window handles large instruction sets well
- Use project knowledge for reference materials that inform instruction design
- Projects maintain context across conversations within the same thread
- Consider using folders to organize multiple Blueprint-created projects

### ChatGPT Projects

**When to use:**
- You have ChatGPT Plus ($20/month) or ChatGPT Team ($25-30/user/month)
- You want flexibility to switch between models (GPT-4o, o1, o1-mini)
- You need Canvas for collaborative document editing
- You work primarily within the ChatGPT ecosystem

**How to create a new project:**
1. Open ChatGPT and look for "Projects" in the left sidebar
2. Click the "+" to create a new project
3. Name it "The Blueprint"
4. Click "Customize" and add the Blueprint instructions to "Instructions"
5. Optionally upload any reference materials to "Files"

**Platform-specific tips:**
- Use GPT-4o for general Blueprint conversations
- Switch to o1 if you're designing particularly complex instruction sets
- Projects keep files and instructions persistent across all chats within that project
- Take advantage of Canvas when drafting instruction documents

### Gemini Gems

**When to use:**
- You have Gemini Advanced ($20/month) or Gemini Business/Enterprise
- You're deeply integrated with Google Workspace (Gmail, Drive, Maps)
- You want dynamic file linking (Drive files stay updated automatically)
- Privacy is acceptable (Gems can't be shared publicly)

**How to create a Gem:**
1. Open Gemini and look for "Gem manager" in the left sidebar (or click the gem icon)
2. Click "New Gem" or "Create Gem"
3. Name it "The Blueprint"
4. Add the Blueprint instructions to the "Instructions" section
5. Optionally use the magic wand icon to let Gemini refine your instructions
6. Add any reference files to the "Knowledge" section

**Platform-specific tips:**
- Use @ mentions (Gmail, Drive, Maps) when relevant to your project design
- Link Google Drive files if you want your knowledge to stay current automatically
- The magic wand feature can help refine instructions if you're struggling
- Gems are private-only; plan accordingly if collaboration matters

### Multiple Platforms

**Why you might want The Blueprint on multiple platforms:**
- Different platforms have different strengths for different project types
- You may use different platforms for work vs. personal projects
- Testing the same project design across platforms can reveal what works universally
- Platform-specific features might inspire different approaches

**Differences between platform versions:**
- Core principles and constraint-thinking are identical across all three
- Platform-specific sections address different architectural realities
- Terminology varies slightly (Project Knowledge vs. Files vs. Knowledge)
- Capability assumptions differ (e.g., Gems mention Google Workspace integration)

**Choosing your "primary" platform:**
Start with whichever platform you use most frequently. The Blueprint will feel more natural when it's in your daily workflow. You can always expand to other platforms later.

## Your First Blueprint Session

### Setting Up

1. **Copy the instructions** from your chosen platform folder (look for the file that matches your platform)
2. **Create a new project/GPT/Gem** following the platform-specific steps above
3. **Paste the instructions** into the appropriate location (Project Knowledge, Instructions, or Instructions section)
4. **Verify it's working** with a simple test:

**Test prompt:**
```
I'm thinking about creating a project that helps me plan weekly meals based on what's in my fridge. Is this feasible? What should I think about first?
```

If The Blueprint responds by asking clarifying questions about your needs, considering constraints, or thinking through viability, you're set up correctly.

### Starting Your First Build

**What to tell The Blueprint first:**

Be clear about what problem you're trying to solve, but don't worry about having everything figured out. The Blueprint works well with both "I have a clear vision" and "I have a fuzzy idea."

**Example opening:**
```
I want to build a teaching assistant for my high school biology course. 
Students struggle with genetics problems, and I'd like something that can 
walk them through problems step-by-step without just giving them answers. 
I'm not sure exactly how to structure the instructions yet.
```

**What The Blueprint will ask you:**

The Blueprint will explore your idea through questions like:
- What specifically should this do? What should it avoid doing?
- Who will use it and in what context?
- What information needs to persist between conversations?
- Where might this hit architectural constraints?
- Have you thought about edge cases like [specific example]?

**How the iterative process works:**

1. You describe your concept
2. The Blueprint asks clarifying questions and surfaces constraints
3. Together you refine the concept into concrete requirements
4. The Blueprint helps you translate requirements into instructions
5. You test the instructions
6. You bring back friction points for debugging
7. Repeat as needed

### Working Through the Build

**Expect multiple conversation rounds:**
Most projects take 3-7 rounds of discussion before you have working instructions. Complex projects may take more. This is normal and expected.

**How to give good feedback:**
- Describe what happened vs. what you expected
- Share specific examples of failures
- Explain the context where problems occurred
- Don't just say "it didn't work" - show the actual interaction

**When to test interim versions:**
Test frequently. As soon as The Blueprint helps you draft initial instructions, try them in a separate thread. Real usage reveals problems that theoretical discussion misses.

**How to know when you're "done" (for now):**
You're done when the project handles your primary use case reliably. Don't aim for perfection - aim for "good enough to be useful." You can always refine later when you discover edge cases.

## Common Use Cases

### Teaching Tools

**Subject-specific tutors:**
Projects that help students learn specific subjects through Socratic questioning, adaptive difficulty, or conceptual explanation. The Blueprint helps you think through how much scaffolding to provide vs. letting students struggle productively.

**Assignment feedback systems:**
Projects that provide structured feedback on student work. The Blueprint helps you balance specificity with maintaining your voice, and decide what rubric information to include.

**Curriculum planning assistants:**
Projects that help you develop lesson plans, unit sequences, or assessment strategies. The Blueprint helps you articulate your teaching philosophy as instructions.

### Research Assistants

**Literature review helpers:**
Projects that synthesize research papers, identify themes, or suggest connections. The Blueprint helps you think through citation handling, summarization depth, and how to avoid just regurgitating sources.

**Note synthesis systems:**
Projects that organize and connect disparate notes into coherent insights. The Blueprint helps you balance structure with emergence.

**Research question developers:**
Projects that help refine vague interests into specific, answerable research questions. The Blueprint helps you articulate what makes a "good" research question in your domain.

### Creative Collaborators

**Writing partners:**
Projects that help with drafting, editing, or brainstorming narrative work. The Blueprint helps you preserve your voice while getting useful feedback.

**Brainstorming tools:**
Projects optimized for expansive, exploratory thinking. The Blueprint helps you distinguish between "brainstorming instructions" and "production instructions."

**Project development assistants:**
Projects that help take rough creative ideas and develop them into actionable plans. The Blueprint helps you think through when to expand vs. when to constrain.

### Domain Experts

**Technical consultants:**
Projects with deep knowledge in specific technical domains (programming languages, scientific fields, etc.). The Blueprint helps you think through what domain knowledge to include vs. trust the base model to know.

**Process guides:**
Projects that walk users through complex procedures or workflows. The Blueprint helps you sequence steps and handle decision points.

**Specialized knowledge bases:**
Projects that become go-to references for niche information. The Blueprint helps you think through what to include, how to organize it, and how to keep it current.

## Tips for Success

**Start with one clear purpose:**
"Help me with biology" is too broad. "Help my students work through genetics Punnett square problems step-by-step" is focused enough to build good instructions around.

**Iterate in small steps:**
Don't try to design perfect instructions in one session. Build something minimal, test it, then add one feature at a time based on real friction.

**Test frequently:**
Every time The Blueprint helps you draft or revise instructions, test them immediately in a separate conversation. Real usage reveals assumptions.

**Keep instructions in version control:**
Save your instruction iterations somewhere (a doc, a notes app, wherever). When you make changes, keep the old version. This helps when you need to roll back or understand why you made certain choices.

**Don't over-specify early:**
Resist the urge to write instructions for every possible edge case before you've tested the basics. Let real usage guide what needs to be specified.

**Let The Blueprint guide the structure:**
If The Blueprint suggests thinking about something you haven't considered, follow that thread. The constraint-thinking framework exists because those patterns matter.

## Troubleshooting

### The Blueprint isn't asking good questions

**Possible causes:**
- You gave too much detail too fast, and The Blueprint is just confirming rather than exploring
- Your initial description was too vague, and The Blueprint needs more to work with
- The conversation has drifted away from instruction-design into implementation details

**Fixes:**
- If you front-loaded everything: Ask "What have I not thought about that matters here?"
- If you were too vague: Provide a concrete example of what you want the project to do
- If you've drifted: Explicitly redirect: "Let's get back to the instruction design - what should we focus on?"

### My instructions aren't working as expected

**How to debug with The Blueprint:**
Bring the failure back to The Blueprint with specifics:
```
I tested the instructions we created. Here's what happened:

[paste actual interaction showing the problem]

What I expected instead was [describe expected behavior].

Can you help me figure out what's wrong with the instructions?
```

The Blueprint will help you distinguish between:
- Instructions that are unclear or contradictory
- Approaches that fight against how the AI naturally works
- Architectural limits you can't instruction your way around

**Common instruction pitfalls:**
- Over-scripting behavior instead of providing context and goals
- Conflicting instructions that pull in different directions
- Assuming the AI will interpret vague language the way you do
- Missing edge case handling because you only tested the happy path
- Instructions that are too long and get ignored

### I want to change direction mid-build

**How to pivot:**
Just tell The Blueprint directly:
```
I've been thinking about this differently now. Instead of [original approach], 
I want to try [new approach]. Can we rethink the instructions with this new 
direction in mind?
```

The Blueprint will help you evaluate whether the pivot is substantial enough to start fresh or if you can modify what you have.

**When to create a new project vs. modify existing:**
- Create new: If the purpose fundamentally changed (teaching assistant → research assistant)
- Modify existing: If you're refining the same goal with a different approach (Socratic method → worked examples)

## Next Steps

**Building multiple specialized tools:**
Once you're comfortable with The Blueprint process, you'll find it faster to create new projects. Each build teaches you patterns that transfer to future builds.

**Exploring meta-templates:**
After creating several projects, you might notice patterns in your instruction structures. The Blueprint can help you create reusable templates for common project types you build.

**Understanding the philosophy:**
See `philosophy.md` (if available in your folder) for deeper exploration of why The Blueprint works the way it does, and the principles behind effective instruction design.

**Contributing your own instruction sets:**
If you create particularly useful projects with The Blueprint, consider documenting your approach. The AI instruction design space is still young, and there's much to learn from diverse use cases.

---

## Quick Start Checklist

- [ ] Choose your platform (Claude, ChatGPT, or Gemini)
- [ ] Create new project/GPT/Gem called "The Blueprint"
- [ ] Copy and paste the appropriate instructions
- [ ] Test with simple prompt to verify setup
- [ ] Start your first build with a clear, focused problem
- [ ] Expect multiple rounds of refinement
- [ ] Test instructions frequently in separate conversations
- [ ] Bring friction back to The Blueprint for debugging
- [ ] Iterate until it works reliably for your core use case

Welcome to The Blueprint. Let's build something useful.