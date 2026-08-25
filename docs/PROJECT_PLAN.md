# TouchDesigner AI Studio - Project Plan

## Vision

TouchDesigner AI Studio aims to become an AI creative assistant for TouchDesigner projects.

The goal is not just generating random node graphs, but allowing an AI agent to understand existing visual systems, inspect networks, suggest improvements, and safely modify projects.

## Core Architecture

```
AI Agent
   |
   | MCP
   v
TouchDesigner AI Bridge
   |
   v
TouchDesigner Python API
   |
   v
Live Project
```

Additional Git-based state/versioning layer:

```
TouchDesigner
      |
      v
Project State Export
      |
      v
Git Repository
      |
      v
AI Context + Commands
      |
      v
TouchDesigner Apply System
```

## Development Phases

### Phase 1 - MCP Foundation

- Keep existing TouchDesigner MCP functionality
- Verify communication between AI client and TouchDesigner
- Document setup

### Phase 2 - Project Intelligence

Create AI-readable project snapshots:

- node tree
- operator types
- parameters
- connections
- errors
- screenshots/previews

### Phase 3 - Safe Modification Layer

Instead of raw arbitrary edits, use structured commands:

- add effect
- modify parameter
- insert pipeline
- create component
- connect nodes

### Phase 4 - Creative Assistant Features

Add higher-level abilities:

- analyze current patch
- suggest improvements
- apply visual styles
- build reusable effect recipes
- generate documentation

### Phase 5 - Versioning + Collaboration

Use Git history for:

- snapshots
- rollback
- experiments
- AI-generated variations

## Design Principles

- Never destroy user work without backup
- Prefer modifying existing systems over replacing them
- Make every AI action explainable
- Keep projects reproducible
- Treat visual networks as evolving creative systems
