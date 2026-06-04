---
name: deploy
description: Deploy your project to production with Copilot assistance
tags:
  - deployment
  - production
author: Rodrigo Huaranga
version: 1.0.0
required_context:
  - git
  - project_root
---

# Deploy Skill

## Description
This skill helps you deploy your current project to production. It guides you through the deployment process and validates your setup.

## Usage
```
copilot skill run deploy
```

## Parameters
- `environment` (optional): Target environment (staging, production)
- `force` (optional): Force deployment without confirmation

## Examples
- `copilot skill run deploy`
- `copilot skill run deploy --environment production`
- `copilot skill run deploy --force`

## Prerequisites
- Git repository initialized
- Project root accessible
- Appropriate deployment credentials configured

## Steps
1. Validates repository status
2. Checks deployment prerequisites
3. Confirms deployment parameters
4. Executes deployment process
5. Reports deployment status

## Output
Deployment status and logs

## Error Handling
- Validates environment before deployment
- Provides rollback instructions on failure
- Logs all deployment activities
