# Artemonim's Agent Tools

**A comprehensive ecosystem of AI-assisted development tools for modern software engineering**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Cross--Platform-black.svg)
![Artemonim](https://img.shields.io/badge/Artemonim's-Agent%20Tools-purple.svg)


## 🚀 Overview

Welcome to **Artemonim's Agent Tools** - a growing ecosystem of specialized tools designed to enhance AI-assisted development workflows. Each tool in this collection addresses specific challenges developers face when working with AI coding assistants, from code comprehension to quality assurance.

## 🛠️ Tools in the Ecosystem

### 📋 [Agent Compass](https://github.com/Artemonim/AgentCompass)

**Status: 🟢 Available**

A comprehensive policy framework for AI-assisted development in Cursor IDE. Transform your AI assistant from a simple code generator into a disciplined, professional developer.

-   **Role-based interaction model** (Architect-Developer)
-   **Structured reporting** with detailed change logs
-   **Security-first approach** with built-in guidelines
-   **Language-specific standards** for Python, JavaScript, TypeScript, C#, C++, PowerShell
-   **Professional documentation** with Better Comments style

**Installation:** Copy rules to Cursor IDE's user rules configuration.

### 📝 [Agent Docstrings](https://github.com/Artemonim/AgentDocstrings)

**Status: 🔴 Archived**

Automatic code structure documentation that helps AI agents understand your codebase instantly. Generates "Table of Contents" summaries at the top of source files.

> This project is archived because, with modern LLMs and Cursor IDE, it provides little practical value for most workflows. The last released version remains available for legacy setups.

-   **Multi-language support** (Python, Java, Kotlin, Go, C/C++, C#, JavaScript, TypeScript, PowerShell, Delphi)
-   **Smart AST parsing** for accurate code analysis
-   **Gitignore integration** with custom filtering
-   **CI/CD ready** with pre-commit hooks
-   **150+ tests** ensuring reliability with **~90% code coverage**

**Installation:** `pip install agent-docstrings`

### 🔧 [Agent Enforcer 2](https://github.com/Artemonim/AgentEnforcer2)

**Status: 🟢 Available**

Local CI blueprint and reference architecture for building robust, language-agnostic code quality pipelines in your projects.

-   **Three-tier architecture**: thin entrypoint → orchestrator → language-specific tooling
-   **Stage-based pipeline**: fmt/lint/typecheck/tests/coverage/security
-   **Caching and idempotency**: skip redundant work safely
-   **Hang detection** and observable execution patterns
-   **Unified reporting** with structured outputs

### 🖼️ Agent Viewport

**Status: ⚪ On Hold (Uncertain)**

UI markup understanding tool for AI-assisted-developers. Helps AI agents comprehend and work with user interface code across different frameworks.

-   **Interactive markup preview** for various UI frameworks
-   **Cross-platform support**
-   **AI-friendly structure analysis**

> Not started as of February 2026. Future development is uncertain.

## 🎯 Why This Ecosystem?

### The Problem

AI coding assistants are powerful but often lack context about:

-   Your project's coding standards and architecture
-   The structure and relationships in your codebase
-   Quality requirements and best practices
-   Their GUI work leaves much to be desired.

### The Solution

Each tool in the Artemonim's Agent Tools ecosystem addresses a specific aspect of this challenge:

1. **Agent Compass** → Establishes consistent behavior and standards
2. **Agent Docstrings (Archived)** → Optional file-level structure summaries
3. **Agent Enforcer 2** → Provides a local CI blueprint for quality and compliance
4. **Agent Viewport** → Enables UI-aware development

Together, they create a comprehensive framework for professional AI-assisted development.

## 🚀 Getting Started

### Quick Start Guide

1. **Start with Agent Compass** - Set up your&AI behavior patterns
2. **Adopt Agent Enforcer 2** - Build a robust local CI pipeline

### Integration Examples

```bash
# Install available tools
pip install agent-docstrings

# Add Agent Compass rules to your IDE
# Adopt Agent Enforcer 2 blueprint (see repo)
```

## Support the Project

Artemonim's Agent Tools is an independent open-source ecosystem. If you find it useful and want to support my work, thank you!

You can support my work in two ways:

-   **Give a Star:** Star the repositories you use on GitHub.
-   **Support on Sponsr:** Support me on [Sponsr](https://sponsr.ru/artemonim/).

Thank you for your support!

### Contributing

We welcome contributions to any tool in the ecosystem! Each repository has its own contribution guidelines:

-   [Agent Compass Contributing](https://github.com/Artemonim/AgentCompass/blob/main/CONTRIBUTING.md)
-   [Agent Docstrings Contributing](https://github.com/Artemonim/AgentDocstrings/blob/main/CONTRIBUTING.md)

---

**Made with ❤️ by [Artemonim](https://github.com/Artemonim)**

_Building the future of AI-assisted development, one tool at a time._
