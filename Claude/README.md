# Claude Projects - The Blueprint

## What's in This Folder

- **blueprint-instructions.md** - Copy/paste-ready instructions for The Blueprint project
- **blueprint-builder-prompt.md** - Meta-template for creating your own customized Blueprint
- **STYLES.md** - Guide to Claude styles (behavioral modes) and available style definitions
- **README.md** - This file

## Quick Setup

### Creating The Blueprint Project

1. Open Claude and click **Projects** in the left sidebar
2. Click **Create Project**
3. Name your project "The Blueprint" (or whatever you prefer)
4. Click into the project, then click the settings icon (⚙️)
5. Under "Project knowledge," click **Add content**
6. Copy the contents of `blueprint-instructions.md` and paste into the text editor
7. Click **Save**

### Verification Test

Start a new conversation in your Blueprint project and send:
```
I'm thinking about creating a project that helps me plan weekly meals 
based on what's in my fridge. Is this feasible? What should I think 
about first?
```

If The Blueprint responds by asking clarifying questions about your needs, considering constraints, or thinking through viability, you're set up correctly.

## About Styles

Claude Projects support **styles** (behavioral modes that change how Claude communicates and thinks without changing project context). 

**Projects vs. Styles:**
- **Projects** provide stable domain context - knowledge, role definitions, persistent state, constraints
- **Styles** provide dynamic behavioral modes - communication preferences, cognitive stance, interaction patterns

You can switch styles mid-conversation to change Claude's approach while maintaining all project context. This makes styles powerful for different phases of work or exploring problems from multiple angles.

The Blueprint helps you design both projects and styles. It can help you create custom styles, design style chains (sequential mode progressions), or build style roulette sets (alternative perspectives on the same problem).

**Available styles and detailed usage guidance:** See [STYLES.md](STYLES.md)

## Platform-Specific Features

**Context Window:** Claude Projects support up to 200K tokens of context, which handles large instruction sets and extensive project knowledge well.

**Project Knowledge vs. Files:** 
- Project knowledge (where you pasted Blueprint instructions) is available to Claude in every conversation within this project
- You can also upload files to projects for reference materials that inform instruction design

**Thread Persistence:** Projects maintain context across conversations within the same thread. Start new threads for distinct topics to avoid context pollution.

**Organization:** Use Claude's project folders to organize multiple Blueprint-created projects as your collection grows.

## What The Blueprint Does

The Blueprint guides you through creating specialized projects by helping you:
- Translate fuzzy ideas into concrete requirements
- Decide what belongs in project instructions vs. conversation context vs. styles
- Think through edge cases and architectural constraints
- Write instructions that provide context without scripting behavior
- Test and refine based on real usage
- Debug when things don't work as expected

See the root [README.md](../README.md) for philosophy and general guidance.

See [getting-started.md](../getting-started.md) for complete onboarding walkthrough.

## Using the Blueprint Builder

The `blueprint-builder-prompt.md` file contains a meta-template that helps you create your own customized Blueprint-equivalent from scratch. Use this if you want to understand the architecture deeply or build a Blueprint variant optimized for your specific use cases.

Start a new conversation in any Claude project and paste the builder prompt to begin the collaborative creation process.

---

*Ready to build? Start a conversation in your Blueprint project and describe what you want to create.*