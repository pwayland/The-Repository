# LLM Instruction Repository

## What This Is

A collection of instruction sets, templates, and meta-tools for building specialized LLM projects. These aren't just prompts—they're architectural frameworks that help you create purpose-built AI assistants that maintain context, develop expertise, and get better at specific tasks over time.

The centerpiece is **The Blueprint**: an instruction set that helps you build instruction sets. It's recursive tooling—using LLMs to help you build better LLM tools.

## Why This Exists

Most people learn to use AI tools by asking questions and hoping for good answers. That works for simple tasks, but it leaves capability on the table. 

This repository is built on a different philosophy: **Give people tools that make the tools teach them.**

Instead of creating dependence on experts or training programs, we're providing infrastructure. Download The Blueprint, and it will guide you through building whatever specialized LLM project you need. You're not learning *our* system—you're building *your* system, with an expert collaborator helping you think through every decision.

This is the bootstrap approach: minimal initial knowledge transfer, maximum long-term capability.

## What's Inside

### Core Instruction Sets

**The Blueprint** - Available for Claude Projects, ChatGPT Projects, and Google Gemini Gems. Each version is adapted to its platform's specific capabilities while maintaining the core architecture. The Blueprint helps you design and build specialized instruction sets for any purpose—teaching tools, research assistants, creative collaborators, domain-specific experts.

### Meta-Templates  

**Blueprint Builders** - Prompt templates that guide you through creating your own Blueprint-equivalent instruction builder, customized for your specific use cases and workflow. These help you understand not just *what* The Blueprint does, but *why* it works, so you can adapt the approach to your needs.

### Guides

**Getting Started** - Platform-specific quick starts and common use cases

**Philosophy** - The thinking behind the bootstrap approach and how to apply it

## How to Use This Repository

### Quick Start

1. **Choose your platform** - Choose your LLM (claude/, chatgpt/, or gemini/)
2. **Start with The Blueprint** - This is your instruction-builder. Copy the instructions into a new project/GPT/Gem
3. **Use The Blueprint to build what you need** - Tell it what you want to create, and it will guide you through designing the instruction set
4. **Iterate** - The Blueprint helps you refine and improve your instructions over time

### Going Deeper

If you want to understand the architecture and adapt it to your specific needs, start with the prompts. These will walk you through building your own Blueprint-equivalent from scratch, customized for your use cases.

See the [Getting Started Guide](getting-started.md) for detailed walkthroughs and the [Philosophy Guide](philosophy.md) to understand the principles behind the approach.

## Current Contents

### Claude Projects
- **The Blueprint - Claude** - Instruction builder for Claude Projects [`the-blueprint-claude.md`]

### ChatGPT Custom GPTs  
- **The Blueprint - ChatGPT** - Instruction builder for ChatGPT Custom GPTs [`the-blueprint-chatgpt.md`]

### Google Gemini Gems
- **The Blueprint - Gemini** - Instruction builder for Gemini Gems [`the-blueprint-gemini
.md`]

### Prompts
- **Claude Blueprint Builder** - Prompt for creating your own Blueprint [`prompts/claude-blueprint-builder.md`]
- **ChatGPT Blueprint Builder** - Prompt for creating your own Blueprint [`prompts/chatgpt-blueprint-builder.md`]
- **Gemini Blueprint Builder** - Prompt for creating your own Blueprint [`prompts/gemini-blueprint-builder.md`]

## Contributing

This repository is currently maintained by its creator, but is designed to eventually become a community resource. If you've built instruction sets that others might find useful, or have improved versions of existing tools, contributions will be welcome in the future.

For now, if you have suggestions or want to share what you've built, feel free to open an issue.

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines (coming soon).

## About

This repository emerged from workshop training on effective LLM use. The goal: not to teach people to depend on experts, but to give them tools that make them self-sufficient builders of their own AI infrastructure.

Built and maintained by Paul Wayland