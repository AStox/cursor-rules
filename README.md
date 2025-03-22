# Cursor Rules

A collection of reusable Cursor AI rules for standardizing code style, development workflows, and best practices across projects.

## Overview

This repository contains a set of Cursor AI rules that can be imported into any project to provide consistent guidance on:

- Code style and quality
- Development workflows
- Git practices
- Problem-solving approaches
- Security considerations
- And more

## Usage

### Adding to a project

1. Clone this repository as a submodule in your project's `.cursor/rules/global` directory:

```bash
# If .cursor/rules directory doesn't exist yet
mkdir -p .cursor/rules

# Add as git submodule
git submodule add git@github.com:AStox/cursor-rules.git .cursor/rules/global
```

2. Commit the changes to your project repository:

```bash
git add .gitmodules .cursor
git commit -m "feat: add cursor rules as submodule"
```

### Updating rules across projects

1. Update the submodule from the main project:

```bash
git submodule update --remote --merge
git add .cursor/rules/global
git commit -m "chore: update cursor rules"
```
