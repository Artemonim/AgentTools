# Contributing to Artemonim's Agent Tools

Thank you for your interest in contributing to the Artemonim's Agent Tools ecosystem! This guide will help you understand how to contribute effectively to this project and its related tools.

## 🎯 How to Contribute

### Types of Contributions

We welcome several types of contributions:

1. **Bug Reports** - Help us identify and fix issues
2. **Feature Requests** - Suggest new tools or improvements to existing ones
3. **Documentation** - Improve guides, examples, and explanations
4. **Code Contributions** - Implement new features or fix bugs
5. **Community Support** - Help other users in discussions and issues

### Where to Contribute

This ecosystem consists of multiple repositories. Choose the appropriate one for your contribution:

- **[Agent Tools Hub](https://github.com/Artemonim/AgentTools)** (this repo) - Ecosystem documentation, roadmap, and general discussions
- **[Agent Compass](https://github.com/Artemonim/AgentCompass)** - AI assistant rules and guidelines
- **[Agent Docstrings](https://github.com/Artemonim/AgentDocstrings)** - Code structure documentation tool
- **Agent Enforcer** - Code quality verification (Coming July 2025)
- **Agent Viewport** - UI markup understanding (Coming summer 2025)

## 🚀 Getting Started

### 1. Choose Your Contribution Type

#### For Bug Reports or Feature Requests
- Go to the appropriate repository
- Check existing issues to avoid duplicates
- Create a new issue with detailed information

#### For Code Contributions
- Fork the relevant repository
- Create a feature branch
- Make your changes
- Submit a pull request

### 2. Development Setup

Each tool has its own development setup requirements. Refer to the individual repository's README and CONTRIBUTING files for specific instructions.

#### General Requirements
- Git for version control
- Appropriate language runtime (Python 3.10+, Go 1.22+, etc.)
- Code editor with linting support

## 📋 Contribution Guidelines

### Code Style and Standards

Each tool in the ecosystem follows specific coding standards:

#### Python Projects (Agent Docstrings)
- Follow PEP 8 style guide
- Use Black for code formatting
- Include type hints
- Write comprehensive docstrings
- Maintain test coverage above 90%

#### Documentation Projects (Agent Compass)
- Use clear, concise language
- Include practical examples
- Follow markdown best practices
- Test all code snippets

#### General Standards
- Write clear commit messages
- Include tests for new features
- Update documentation for changes
- Follow semantic versioning

### Commit Message Format

Use conventional commits format:

```
type(scope): description

[optional body]

[optional footer]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `test`: Test changes
- `chore`: Maintenance tasks

Examples:
```
feat(compass): add TypeScript-specific rules
fix(docstrings): handle multiline function definitions
docs(readme): update installation instructions
```

### Pull Request Process

1. **Fork and Clone**
   ```bash
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
   ```

2. **Create Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Changes**
   - Follow the coding standards
   - Add tests for new functionality
   - Update documentation

4. **Test Your Changes**
   - Run existing tests
   - Add new tests if needed
   - Ensure all tests pass

5. **Commit and Push**
   ```bash
   git add .
   git commit -m "feat: add new feature"
   git push origin feature/your-feature-name
   ```

6. **Create Pull Request**
   - Use a clear title and description
   - Reference related issues
   - Include screenshots if applicable
   - Wait for review and feedback

## 🐛 Reporting Issues

### Bug Reports

When reporting bugs, please include:

1. **Environment Information**
   - Operating system
   - Tool version
   - Programming language version
   - IDE/editor being used

2. **Steps to Reproduce**
   - Clear, step-by-step instructions
   - Minimal code example
   - Expected vs actual behavior

3. **Additional Context**
   - Error messages
   - Log files
   - Screenshots if helpful

### Feature Requests

For feature requests, please provide:

1. **Problem Description**
   - What problem does this solve?
   - Who would benefit from this feature?

2. **Proposed Solution**
   - How should this feature work?
   - Any implementation ideas?

3. **Alternatives Considered**
   - Other solutions you've considered
   - Why this approach is preferred

## 🤝 Community Guidelines

### Code of Conduct

We are committed to providing a welcoming and inclusive environment. Please:

- Be respectful and considerate
- Welcome newcomers and help them learn
- Focus on constructive feedback
- Respect different viewpoints and experiences

### Communication Channels

- **GitHub Issues** - Bug reports and feature requests
- **GitHub Discussions** - General questions and community chat
- **Pull Requests** - Code review and collaboration

## 📚 Resources

### Documentation
- [Agent Compass Documentation](https://github.com/Artemonim/AgentCompass)
- [Agent Docstrings Documentation](https://github.com/Artemonim/AgentDocstrings)

### Learning Resources
- [Conventional Commits](https://www.conventionalcommits.org/)
- [Semantic Versioning](https://semver.org/)
- [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)