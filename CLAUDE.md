# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a comprehensive n8n workflow automation repository containing 2000+ workflows with an automated documentation system. The primary purpose is to share, document, and enable discovery of n8n automation workflows.

## Key Commands

### Generate Documentation
```bash
cd n8n
python3 generate_documentation.py
```
This creates `workflow-documentation.html` with interactive browsing, search, and analysis of all workflows.

### Import All Workflows
```bash
cd n8n
./import-workflows.sh
```
Bulk imports all workflows into an n8n instance using `npx n8n import:workflow`.

## Architecture

### Directory Structure
- `/n8n/workflows/` - Contains 2000+ n8n workflow JSON files
- `/n8n/generate_documentation.py` - Static analyzer that generates HTML documentation
- `/AI Workflow Blueprints(n8n)/` - Educational resources and templates organized by category

### Workflow JSON Structure
Each workflow file contains:
- `name`: Workflow identifier
- `nodes`: Array of operations (triggers, integrations, logic, data processing)
- `connections`: Node connectivity definitions
- `settings`: Workflow configuration
- `tags`: Categorization metadata

### Documentation System
The Python documentation generator:
- Performs static analysis on all JSON workflows
- Extracts metadata, integrations, and complexity metrics
- Categorizes workflows by trigger type (Manual, Webhook, Scheduled, Complex)
- Generates self-contained HTML with embedded JavaScript for interactivity
- No external dependencies - uses only Python standard library

## Working with Workflows

### Common Node Types
- **Triggers**: webhook, cron, manual trigger
- **Integrations**: HTTP Request, database connectors, API integrations (100+ services)
- **Logic**: IF, Switch, Merge, Loop, Set, Function
- **AI Services**: OpenAI, Google Gemini, Claude, Mistral nodes

### When Analyzing Workflows
1. Parse JSON to understand node chains and business logic
2. Identify trigger mechanisms and external dependencies
3. Check for error handling and retry mechanisms
4. Consider modular design patterns (sub-workflows)

### When Modifying Workflows
1. Preserve JSON structure and required fields
2. Maintain unique node IDs
3. Update connections when adding/removing nodes
4. Remove sensitive data (credentials, API keys, URLs)

## Security Considerations
- Workflows may contain webhook URLs or API configurations
- Credentials are stored separately in n8n, not in workflow files
- Always sanitize workflows before sharing or committing