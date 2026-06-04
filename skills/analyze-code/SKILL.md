---
name: analyze-code
description: Analyze code quality, performance, and security issues in your project
tags:
  - analysis
  - code-quality
  - security
author: Rodrigo Huaranga
version: 1.0.0
required_context:
  - project_root
---

# Analyze Code Skill

## Description
This skill performs comprehensive analysis of your codebase, including:
- Code quality metrics
- Performance bottlenecks
- Security vulnerabilities
- Best practices violations

## Usage
```
copilot skill run analyze-code
```

## Parameters
- `path` (optional): Specific path to analyze (defaults to project root)
- `type` (optional): Type of analysis (quality, security, performance, all)
- `strict` (optional): Enable strict mode for enhanced checking

## Examples
- `copilot skill run analyze-code`
- `copilot skill run analyze-code --type security`
- `copilot skill run analyze-code --path src/ --strict`

## Analysis Includes
- Linting results
- Type checking
- Dependency vulnerabilities
- Code complexity metrics
- Performance warnings
- Security scan results

## Output
Detailed analysis report with:
- Issues found
- Severity levels
- Recommended fixes
- Performance metrics

## Notes
- Results are cached for performance
- Use `--force` to bypass cache
