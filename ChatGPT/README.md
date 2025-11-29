# ChatGPT Projects - The Blueprint

## What's in This Folder

- **blueprint-instructions.md** - Copy/paste-ready instructions for The Blueprint project
- **blueprint-builder-prompt.md** - Meta-template for creating your own customized Blueprint
- **README.md** - This file

## Quick Setup

### Creating The Blueprint Project

1. Open ChatGPT and click **Projects** in the left sidebar (or click your profile icon → Projects)
2. Click the **+** button to create a new project
3. Name your project "The Blueprint"
4. Click **Customize** in the project header
5. Under "Instructions," paste the contents of `blueprint-instructions.md`
6. Click **Update** to save
7. (Optional) Upload any reference materials to the "Files" section

### Verification Test

Start a new chat in your Blueprint project and send:
```
I'm thinking about creating a project that helps me plan weekly meals 
based on what's in my fridge. Is this feasible? What should I think 
about first?
```

If The Blueprint responds by asking clarifying questions about your needs, considering constraints, or thinking through viability, you're set up correctly.

## Platform-Specific Features

**Model Flexibility:** ChatGPT Projects let you switch between models (GPT-4o, o1, o1-mini) within the same project. Use GPT-4o for general Blueprint conversations and switch to o1 for particularly complex instruction design if needed.

**Canvas Integration:** Take advantage of Canvas when drafting instruction documents. The collaborative editing environment can be helpful for iterative instruction refinement.

**Cross-Chat Persistence:** Project instructions and files are available across all chats within that project (not just a single thread like Claude). This makes it easy to return to instruction design work across multiple sessions.

**Files vs. Instructions:**
- Instructions (where you pasted Blueprint content) apply to every conversation in this project
- Files provide reference materials that inform instruction design
- Both persist across all chats in the project

## What The Blueprint Does

The Blueprint guides you through creating specialized projects by helping you:
- Translate fuzzy ideas into concrete requirements
- Decide what belongs in project instructions vs. conversation context
- Think through edge cases and architectural constraints
- Write instructions that provide context without scripting behavior
- Test and refine based on real usage
- Debug when things don't work as expected

See the root [README.md](../README.md) for philosophy and general guidance.

See [getting-started.md](../getting-started.md) for complete onboarding walkthrough.

## Using the Blueprint Builder

The `blueprint-builder-prompt.md` file contains a meta-template that helps you create your own customized Blueprint-equivalent from scratch. Use this if you want to understand the architecture deeply or build a Blueprint variant optimized for your specific use cases.

Start a new chat in any ChatGPT project and paste the builder prompt to begin the collaborative creation process.

---

*Ready to build? Start a chat in your Blueprint project and describe what you want to create.*