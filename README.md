# TouchDesigner AI Studio

An experimental AI assistant framework for TouchDesigner.

The goal is to combine MCP-based TouchDesigner control with project understanding, versioned workflows, and creative AI assistance.

## Vision

TouchDesigner AI Studio is intended to become a system where an AI agent can:

- understand an existing TouchDesigner project
- inspect node networks and parameters
- create and modify visual systems
- suggest improvements
- build reusable creative recipes
- safely evolve projects over time

## Current Foundation

This project builds on the idea of connecting AI agents with TouchDesigner through MCP (Model Context Protocol).

The original MCP layer provides communication between AI tools and TouchDesigner, including:

- creating nodes
- modifying nodes
- querying project information
- executing TouchDesigner Python
- capturing outputs

## Planned Features

### Project Intelligence

Export AI-readable project context:

- node graph
- connections
- parameters
- errors
- previews

### Creative Assistant Layer

Higher-level commands:

- add VHS corruption system
- create CRT pipeline
- improve composition
- generate audio reactive networks
- build procedural environments

### Versioned AI Workflow

Use Git history for:

- snapshots
- experiments
- rollback
- comparing AI changes

## Development Docs

- [Project Plan](docs/PROJECT_PLAN.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Implementation Status](docs/IMPLEMENTATION_STATUS.md)

## Status

Early development / architecture phase.

The first milestone is creating a reliable bridge between AI tools and TouchDesigner, then adding project understanding and creative workflows on top.
