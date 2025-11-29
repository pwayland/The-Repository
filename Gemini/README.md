# Gemini Gems - The Blueprint

## What's in This Folder

- **blueprint-instructions.md** - Copy/paste-ready instructions for The Blueprint Gem
- **blueprint-builder-prompt.md** - Meta-template for creating your own customized Blueprint
- **README.md** - This file

## Quick Setup

### Creating The Blueprint Gem

1. Open Gemini and click **Gem manager** in the left sidebar (or click the gem icon ◆)
2. Click **New Gem** or **Create Gem**
3. Name your Gem "The Blueprint"
4. In the "Instructions" section, paste the contents of `blueprint-instructions.md`
5. (Optional) Click the magic wand icon if you want Gemini to help refine the instructions
6. (Optional) Add reference files to the "Knowledge" section
7. Click **Save**

### Verification Test

Start a new conversation with your Blueprint Gem and send:
```
I'm thinking about creating a project that helps me plan weekly meals 
based on what's in my fridge. Is this feasible? What should I think 
about first?
```

If The Blueprint responds by asking clarifying questions about your needs, considering constraints, or thinking through viability, you're set up correctly.

## Platform-Specific Features

**Google Workspace Integration:** Gems can access your Gmail, Google Drive, and Google Maps through @ mentions. This can be powerful for projects that need to interact with your existing Google ecosystem.

**Dynamic File Linking:** Files linked from Google Drive stay current automatically. If you update a reference document in Drive, the Gem sees the updated version without needing to re-upload.

**Magic Wand Refinement:** The magic wand feature can help refine instructions if you're struggling with wording. Use this judiciously - it's helpful for clarity but can sometimes change intent.

**Privacy Note:** Gems are private-only and cannot be shared publicly. Plan accordingly if you're building instruction sets you want to distribute to others.

**Instructions vs. Knowledge:**
- Instructions (where you pasted Blueprint content) define how the Gem behaves
- Knowledge section holds reference materials that inform instruction design
- Both persist across all conversations with this Gem

## What The Blueprint Does

The Blueprint guides you through creating specialized Gems by helping you:
- Translate fuzzy ideas into concrete requirements
- Decide what belongs in Gem instructions vs. conversation context
- Think through edge cases and architectural constraints
- Write instructions that provide context without scripting behavior
- Test and refine based on real usage
- Debug when things don't work as expected

See the root [README.md](../README.md) for philosophy and general guidance.

See [getting-started.md](../getting-started.md) for complete onboarding walkthrough.

## Using the Blueprint Builder

The `blueprint-builder-prompt.md` file contains a meta-template that helps you create your own customized Blueprint-equivalent from scratch. Use this if you want to understand the architecture deeply or build a Blueprint variant optimized for your specific use cases.

Start a new conversation with any Gem and paste the builder prompt to begin the collaborative creation process.

---

*Ready to build? Start a conversation with your Blueprint Gem and describe what you want to create.*