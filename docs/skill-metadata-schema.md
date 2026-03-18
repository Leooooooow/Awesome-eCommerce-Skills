# Skill Metadata Schema

This document defines the recommended metadata schema for Awesome eCommerce Skills.

## Core identity
- `name`
- `slug`
- `category`
- `status`
- `priority`

## Workflow understanding
- `problem`
- `best_for`
- `stage`
- `input`
- `output`
- `handoff`
- `use_when`
- `not_for`

## Capability / execution requirements
- `delivery_mode`
  - `prompt-only`
  - `tool-assisted`
  - `script-backed`
  - `browser-assisted`
  - `hybrid`
- `requires_api`
- `recommended_api`
- `requires_browser`
- `browser_mode`
  - `openclaw-managed`
  - `browser-relay`
  - `none`
- `requires_script`
- `script_runtime`
  - `python`
  - `node`
  - `shell`
  - `mixed`
  - `none`

## Installation / visibility
- `install_methods`
- `visibility`
  - `public-showcase`
  - `clawhub-only`
  - `internal`

## Why this schema matters

It helps:
- websites generate better catalogs
- AI agents select the right skill
- registries standardize install paths
- maintainers classify skills by capability and risk

## Immediate recommendation

At minimum, standardize these fields first:
- `name`
- `slug`
- `category`
- `best_for`
- `stage`
- `input`
- `output`
- `handoff`
- `delivery_mode`
- `requires_api`
- `requires_browser`
- `requires_script`
