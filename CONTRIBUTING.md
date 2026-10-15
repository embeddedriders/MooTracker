# Contributing to MooTracker

Thank you for your interest in contributing to MooTracker! We welcome contributions from the community to make this AI-powered cattle health monitoring platform better.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Reporting Bugs](#reporting-bugs)
- [Feature Requests](#feature-requests)

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). Please treat all community members with respect.

## Getting Started

1. **Fork** the repository on GitHub
2. **Clone** your fork locally: `git clone https://github.com/YOUR-USERNAME/MooTracker.git`
3. **Add upstream remote**: `git remote add upstream https://github.com/embeddedriders/MooTracker.git`
4. **Create a branch** for your changes: `git checkout -b feature/your-feature-name`

## How to Contribute

### Types of Contributions

- 🐛 **Bug Fixes** — Fix issues reported in the issue tracker
- ✨ **New Features** — Add new functionality (discuss in an issue first)
- 📚 **Documentation** — Improve README, inline comments, or wiki pages
- 🧪 **Tests** — Add or improve test coverage
- 🔧 **Refactoring** — Improve code structure without changing behaviour
- 🌐 **Translations** — Add or improve language support (Hindi/English bilingual support)

## Development Setup

### Prerequisites

- Node.js >= 18.x
- Python >= 3.9 (for ML engine and build scripts)
- ESP32 toolchain (for firmware contribution)

### Running Locally

```bash
# Install dependencies
npm install

# Start the local server
node server.js
```

Open **http://localhost:3000** in your browser.

### Running the ML Engine

```bash
pip install -r requirements.txt
python build_release.py
```

## Pull Request Process

1. Ensure your changes are on a **feature branch** (not `main`)
2. Update the **README.md** if your change affects usage or setup
3. Add relevant **comments** to complex logic
4. Run the app locally and verify nothing is broken
5. Submit a PR with a **clear title** and description:
   - What problem does this solve?
   - How was it tested?
   - Screenshots (for UI changes)
6. Respond to review comments promptly

### PR Title Format

Use conventional commits format:
- `feat: add new signal dashboard widget`
- `fix: correct milk pattern threshold calculation`
- `docs: update ESP32 wiring diagram`
- `chore: upgrade supabase client version`

## Coding Standards

### JavaScript

- Use **ES6+** syntax (arrow functions, destructuring, template literals)
- Keep functions small and focused (single responsibility)
- Comment non-obvious logic with `//` inline comments
- Use `camelCase` for variables and functions
- Use `UPPER_CASE` for constants

### Python

- Follow **PEP 8** style guidelines
- Use type hints where possible
- Docstrings for all public functions

### HTML/CSS

- Use semantic HTML5 elements
- Keep CSS class names descriptive (BEM methodology encouraged)
- Ensure **mobile responsiveness** for all UI changes
- Test bilingual (EN/हिं) toggle still works after changes

## Reporting Bugs

Before reporting a bug:
1. Search [existing issues](https://github.com/embeddedriders/MooTracker/issues) to avoid duplicates
2. Test on the latest version

When reporting:
- Provide a **clear title** and description
- Include **steps to reproduce**
- Share **expected vs actual behaviour**
- Attach **screenshots** or **error logs** if possible
- Note your **browser**, **OS**, and **device**

## Feature Requests

We love ideas! Open a [Feature Request issue](https://github.com/embeddedriders/MooTracker/issues/new) with:
- The **problem** you're trying to solve
- Your **proposed solution**
- Any **alternative approaches** considered

## Questions?

Open a [Discussion](https://github.com/embeddedriders/MooTracker/discussions) or reach out via the issue tracker.

---

Happy contributing! 🐄📡