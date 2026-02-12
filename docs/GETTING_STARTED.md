# Getting Started with Artemonim's Agent Tools

Welcome to the Artemonim's Agent Tools ecosystem! This guide will help you get up and running with our suite of AI-assisted development tools.

## 🎯 What You'll Learn

By the end of this guide, you'll have:

-   ✅ Set up Agent Compass for consistent AI behavior
-   ✅ Configured your development environment for optimal AI assistance
-   ✅ Understood how Agent Enforcer 2 fits into a robust local CI workflow
-   ✅ Understanding of how all tools work together

## 🚀 Quick Start (5 minutes)

### Step 1: Choose Your Starting Point

**New to AI-assisted development?**
→ Start with [Agent Compass](#agent-compass-setup) to establish consistent AI behavior

**Have existing codebases?**
→ Start with [Agent Docstrings](#agent-docstrings-setup) to improve code comprehension

**Want comprehensive setup?**
→ Follow the [Complete Setup](#complete-setup) guide

### Step 2: Install Available Tools

```bash
# Agent Compass is configuration-based (no installation needed)
# Agent Enforcer 2 - Available (see repo)
# Agent Viewport - On Hold (future development uncertain)
```

## 📋 Agent Compass Setup

Agent Compass transforms your AI assistant into a disciplined, professional developer.

### Installation in Cursor IDE

1. **Open Cursor IDE**
2. **Access Settings**: Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
3. **Find Rules**: Type "Cursor: Configure User Rules" and select it
4. **Get Rules**: Visit [Agent Compass Repository](https://github.com/Artemonim/AgentCompass)
5. **Copy Content**: Copy the contents of `COMPASS.md`
6. **Paste Rules**: Paste into the rules editor
7. **Save**: Save and close the editor

### Verification

Test your setup with a simple request:

```
You: "Create a simple Python function to calculate factorial"
```

You should see:

-   ✅ Structured response with clear sections
-   ✅ Better Comments style (`# * Important`, `# ! Warning`, etc.)
-   ✅ Detailed report at the end with "Changes Made" section
-   ✅ Professional error handling and documentation

### Key Features You'll Notice

-   **Role-based interaction**: AI acts as your "Developer" while you're the "Architect"
-   **Structured reporting**: Every response ends with a detailed report
-   **Security-first**: No hardcoded secrets, proper placeholder usage
-   **Language-specific standards**: Follows best practices for each programming language

## 📝 Agent Docstrings Setup

Agent Docstrings helps AI agents understand your codebase structure instantly.

> This project is archived and is often unnecessary with modern LLMs in Cursor IDE. Consider it an optional, legacy workflow component.

### Installation

```bash
# Install from PyPI
pip install agent-docstrings

# Verify installation
agent-docstrings --version
```

### Basic Usage

```bash
# Process a single directory
agent-docstrings src/

# Process multiple paths
agent-docstrings src/ tests/ lib/utils.py

# Verbose output
agent-docstrings src/ --verbose
```

## 🤝 Integration Patterns

### Pattern 1: AI-First Development

1. **Start with Agent Compass** - Set behavior expectations
2. **Use AI to generate code** - Let AI create initial structure
3. **Run Agent Docstrings** - Generate structure documentation
4. **Iterate with AI** - AI can now understand your code structure

### Pattern 2: Existing Codebase Enhancement

1. **Run Agent Docstrings** - Document existing structure
2. **Configure Agent Compass** - Establish standards for new code
3. **Use AI for refactoring** - AI understands existing patterns
4. **Maintain with pre-commit hooks** - Keep documentation current

### Pattern 3: Team Collaboration

1. **Team-wide Agent Compass rules** - Consistent AI behavior
2. **Shared Agent Docstrings config** - Uniform documentation
3. **CI/CD integration** - Automated quality checks
4. **Regular updates** - Keep tools and configurations current

## 🧩 Other Tools in the Ecosystem

### Agent Enforcer 2 (Available)

-   **Purpose**: Local CI blueprint and reference architecture
-   **Integration**: Works with Agent Compass rules
-   **Setup**: Follow the repository docs and adapt the patterns to your stack

### Agent Viewport (On Hold / Uncertain)

-   **Purpose**: UI markup understanding for AI
-   **Integration**: Complements Agent Docstrings for UI code
-   **Setup**: Not started as of February 2026

## 🐛 Troubleshooting

### Common Issues

#### Agent Compass Not Working

-   **Check**: Rules are properly pasted in Cursor settings
-   **Verify**: Start a new chat session after configuration
-   **Test**: Try a simple coding request

#### Agent Docstrings Errors

-   **Check**: Python version compatibility (3.10+)
-   **Verify**: File permissions in target directories
-   **Test**: Run with `--verbose` flag for detailed output

#### Integration Issues

-   **Check**: Tool versions are compatible
-   **Verify**: Configuration files are in correct locations
-   **Test**: Run tools individually before combining

### Getting Help

1. **Check Documentation**: Individual tool repositories have detailed docs
2. **Search Issues**: Look for similar problems in GitHub issues
3. **Ask Community**: Use GitHub Discussions for questions
4. **Report Bugs**: Create detailed issue reports with examples

## 📚 Next Steps

### Learn More

-   [Agent Compass Documentation](https://github.com/Artemonim/AgentCompass)
-   [Agent Docstrings Documentation](https://github.com/Artemonim/AgentDocstrings)
-   [Ecosystem Roadmap](./ROADMAP.md)

### Get Involved

-   [Contributing Guidelines](../CONTRIBUTING.md)
-   [Community Discussions](https://github.com/Artemonim/AgentTools/discussions)
-   [Feature Requests](https://github.com/Artemonim/AgentTools/issues)

### Stay Updated

-   ⭐ Star the repositories you use
-   👁️ Watch repositories for updates
-   📧 Follow release notifications

---

**Happy coding with AI! 🚀**

_If you find this guide helpful, consider starring the repositories you use and supporting on [Sponsr](https://sponsr.ru/artemonim/)._
