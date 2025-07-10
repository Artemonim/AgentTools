# Getting Started with Artemonim's Agent Tools

Welcome to the Artemonim's Agent Tools ecosystem! This guide will help you get up and running with our suite of AI-assisted development tools.

## 🎯 What You'll Learn

By the end of this guide, you'll have:

-   ✅ Set up Agent Compass for consistent AI behavior
-   ✅ Installed Agent Docstrings for code structure documentation
-   ✅ Configured your development environment for optimal AI assistance
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
# Install Agent Docstrings
pip install agent-docstrings

# Agent Compass is configuration-based (no installation needed)
# Agent Enforcer - Coming Q2 2025
# Agent Viewport - Coming Q3 2025
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

### Integration with Development Workflow

#### Pre-commit Hook

Add to `.pre-commit-config.yaml`:

```yaml
repos:
    - repo: local
      hooks:
          - id: agent-docstrings
            name: Generate docstrings
            entry: agent-docstrings
            language: system
            files: \.(py|java|kt|go|ps1|psm1|pas|js|jsx|ts|tsx|cs|cpp|cxx|cc|hpp|h|c)$
            pass_filenames: false
            args: [src/]
```

#### VS Code/Cursor Integration

Add to your project's tasks.json:

```json
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Update Docstrings",
            "type": "shell",
            "command": "agent-docstrings",
            "args": ["src/"],
            "group": "build",
            "presentation": {
                "echo": true,
                "reveal": "always",
                "focus": false,
                "panel": "shared"
            }
        }
    ]
}
```

### Configuration Options

#### Ignore Files (`.agent-docstrings-ignore`)

```
# Ignore test files
**/test_*.py
**/tests/

# Ignore generated files
**/generated/
**/__pycache__/
```

#### Include Only (`.agent-docstrings-include`)

```
# Only process main source code
src/**/*.py
lib/**/*.py
agent_docstrings/**/*.py
```

## 🔧 Complete Setup

### 1. Project Structure Preparation

```bash
# Create a new project or navigate to existing one
mkdir my-ai-project
cd my-ai-project

# Initialize git if not already done
git init

# Create basic structure
mkdir src tests docs
```

### 2. Agent Compass Configuration

Follow the [Agent Compass Setup](#agent-compass-setup) above.

### 3. Agent Docstrings Integration

```bash
# Install and run initial scan
pip install agent-docstrings
agent-docstrings src/ --verbose

# Set up pre-commit hooks
pip install pre-commit
pre-commit install
```

### 4. Development Environment Configuration

#### VS Code/Cursor Settings

Add to `.vscode/settings.json`:

```json
{
    "python.linting.enabled": true,
    "python.linting.pylintEnabled": true,
    "python.formatting.provider": "black",
    "editor.formatOnSave": true,
    "files.exclude": {
        "**/__pycache__": true,
        "**/*.pyc": true
    }
}
```

#### Git Configuration

Add to `.gitignore`:

```
# Python
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
*.egg-info/
.installed.cfg
*.egg

# IDE
.vscode/
.idea/
*.swp
*.swo
*~

# OS
.DS_Store
Thumbs.db
```

### 5. Testing the Setup

Create a test file `src/calculator.py`:

```python
def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

class Calculator:
    def __init__(self):
        self.history = []

    def calculate(self, operation, a, b):
        if operation == "add":
            result = add(a, b)
        elif operation == "multiply":
            result = multiply(a, b)
        else:
            raise ValueError("Unknown operation")

        self.history.append((operation, a, b, result))
        return result
```

Run Agent Docstrings:

```bash
agent-docstrings src/
```

The file should now have a table of contents at the top showing the structure.

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

## 🔮 Future Tools Preview

### Agent Enforcer (Coming Q2 2025)

-   **Purpose**: Automated code quality verification
-   **Integration**: Works with Agent Compass rules
-   **Setup**: Will integrate with existing linting workflows

### Agent Viewport (Coming Q3 2025)

-   **Purpose**: UI markup understanding for AI
-   **Integration**: Complements Agent Docstrings for UI code
-   **Setup**: Will support major UI frameworks

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

_If you find this guide helpful, consider [supporting the project](https://boosty.to/artemonim) or sharing it with your team._
