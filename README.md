# LLM Instruction Repository

## What This Is

A collection of instruction sets and meta-tools for building specialized LLM projects. These aren't just prompts—they're architectural frameworks that help you create purpose-built AI assistants tailored to specific tasks, domains, or workflows.

The centerpiece is **The Blueprint**: an instruction set that helps you build instruction sets. It's recursive tooling—using LLMs to help you design better LLM tools.

## Why This Exists

Most people learn to use AI tools by asking questions and hoping for good answers. That works for simple tasks, but it leaves capability on the table.

This repository is built on a different philosophy: **Give people tools that make the tools teach them.**

Instead of creating dependence on experts or training programs, we're providing infrastructure. Use The Blueprint, and it will guide you through building whatever specialized LLM project you need. You're not learning *our* system—you're building *your* system, with an expert collaborator helping you think through every decision.

This is the bootstrap approach: minimal initial knowledge transfer, maximum long-term capability. See [philosophy.md](philosophy.md) for the full thinking behind this approach.

## Repository Structure

### Platform Folders

Choose the folder for your LLM platform:

- **[Claude/](Claude/)** - For Claude Projects (Claude Pro or Team)
- **[ChatGPT/](ChatGPT/)** - For ChatGPT Projects (ChatGPT Plus or Team)  
- **[Gemini/](Gemini/)** - For Gemini Gems (Gemini Advanced or Business)

Each folder contains:
- **The Blueprint** - Copy/paste-ready instructions for creating specialized projects
- **Blueprint Builder** - Meta-template for creating your own customized Blueprint
- **Platform README** - Setup instructions and file guide

Not sure which platform to use? See the platform comparison in [getting-started.md](getting-started.md).

### Examples & Inspiration

**[made-by-the-blueprint/](made-by-the-blueprint/)** - Real instruction sets created using The Blueprint, demonstrating different approaches and use cases. These serve as templates and learning resources, not production copies.

### Guides

**[getting-started.md](getting-started.md)** - Complete onboarding guide covering platform selection, setup, first build walkthrough, common use cases, and troubleshooting.

**[philosophy.md](philosophy.md)** - Deep dive into the bootstrap approach, meta-tooling concepts, and principles behind effective instruction design.

## Quick Start

1. **Choose your platform** - Navigate to Claude/, ChatGPT/, or Gemini/
2. **Follow the platform README** - Copy instructions, create new project, verify setup
3. **Start building** - Tell The Blueprint what you want to create
4. **Iterate** - Test, refine, bring friction back for debugging
5. **Use what you built** - Your specialized project is now available whenever you need it

Most first projects take 20-60 minutes of collaborative discussion to get working instructions. Complex projects may take longer. This is normal—you're building lasting capability, not just getting a quick answer.

## What You Can Build

The Blueprint helps you create specialized projects for:

- **Teaching tools** - Subject tutors, assignment feedback systems, curriculum planners
- **Research assistants** - Literature review helpers, note synthesis, research question development
- **Creative collaborators** - Writing partners, brainstorming tools, project development
- **Domain experts** - Technical consultants, process guides, specialized knowledge bases
- **Analysis tools** - Document reviewers, strategic planning, evaluation frameworks

If you find yourself having the same type of conversation with an LLM repeatedly, you probably need a specialized project. The Blueprint helps you build it.

## How This Works

The Blueprint guides you through:
- Translating fuzzy ideas into concrete requirements
- Deciding what belongs in instructions vs. conversation context
- Thinking through edge cases and constraints
- Writing instructions that provide context without scripting behavior
- Testing and refining based on real usage
- Debugging when things don't work as expected

You describe what you want. The Blueprint asks clarifying questions, surfaces constraints, helps you think through architecture. Together you develop instructions that work reliably for your use case.

The value compounds over time. Your first project teaches you patterns that transfer to future builds. Each project extends your capability in a persistent way. The meta-skill you develop—thinking effectively about instruction design—applies across all future work with LLMs.

## Contributing

This repository is currently maintained by its creator, but is designed to eventually become a community resource. 

If you've built instruction sets that others might find useful, have improved versions of existing tools, or have insights about patterns that work well, contributions will be welcome as the project matures.

For now, if you have suggestions or want to share what you've built, open an issue.

## About

This repository emerged from workshop training on effective LLM use. The goal: not to teach people to depend on experts, but to give them tools that make them self-sufficient builders of their own AI infrastructure.

The bootstrap philosophy—giving people tools that teach themselves rather than trying to transfer all knowledge directly—scales better and creates more lasting capability than traditional instruction.

Built and maintained by Paul Wayland

---

*New to instruction design? Start with [getting-started.md](getting-started.md)*  
*Want to understand the philosophy? See [philosophy.md](philosophy.md)*  
*Ready to build? Choose your platform folder above*