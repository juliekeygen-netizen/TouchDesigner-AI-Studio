# TouchDesigner AI Studio Architecture

## Components

### 1. AI Client

Examples:

- MCP-compatible AI assistants
- coding agents
- future custom interfaces

Responsible for reasoning and deciding actions.

### 2. MCP Server

Provides structured tools:

- inspect nodes
- create operators
- delete operators
- connect networks
- edit parameters
- execute TouchDesigner Python
- capture previews

### 3. TouchDesigner Bridge

A TouchDesigner component that exposes project control through the WebServer DAT and Python API.

Responsibilities:

- receive commands
- validate actions
- execute changes
- return results

### 4. Project Intelligence Layer

Creates AI-friendly descriptions of projects:

```
project_state/
  nodes.json
  parameters.json
  connections.json
  preview.png
```

This allows the AI to understand existing patches instead of blindly creating new ones.

### 5. Recipe System

Reusable creative building blocks:

```
recipes/
  crt_broadcast/
  vhs_damage/
  alien_environment/
  audio_reactive/
```

Recipes describe proven networks and parameter groups.

## Safety Model

AI actions should flow through:

```
Request
  |
Validation
  |
Backup
  |
Apply
  |
Report result
```

Large destructive operations should require confirmation.
