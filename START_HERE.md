# START HERE

If you are new to Awesome eCommerce Skills, use this order:

## 1) Understand what this GitHub repo is for

This repository is the **public catalog and documentation layer** for ecommerce skills.

Use GitHub to:
- understand what a skill does
- compare workflows
- inspect metadata and examples
- help humans and AI agents choose the right skill

Do **not** treat GitHub as the main download surface for production-ready skills.

## 2) Install real skills through SkillHub or ClawHub

Recommended install sources:
- **SkillHub** → preferred when available in your environment
- **ClawHub** → public fallback and distribution channel

The real install path should come from a registry, not from manually copying random files out of GitHub.

## 3) Use this repo as a routing layer

Start from:
- [`skills/manifest.json`](skills/manifest.json) for machine-readable metadata
- [`skills/INDEX.md`](skills/INDEX.md) for category navigation
- `skills/<slug>/SKILL.md` for deeper workflow detail

## Minimal mental model

- **Website** = fastest browse experience
- **GitHub** = catalog, docs, examples, trust
- **SkillHub / ClawHub** = install real skills

## How to prompt an agent with a skill

```text
Use <skill-slug> to <goal>.
Input: <source/data>
Constraints: <channel/risk/time>
Output: <format>
```

Example:

```text
Use ugc-variants-generator to generate 12 short-video variants.
Input: one base script + target audience + banned claims.
Output: 12 variants + hook + CTA + test order.
```

## Before you choose a skill

Check these fields first:
- problem
- best_for
- stage
- input
- output
- handoff

Then check execution requirements:
- does it need an API?
- does it need browser automation?
- does it need a script/runtime?

## Suggested next reading

- [What is a skill?](docs/what-is-a-skill.md)
- [Installing real skills](docs/installing-real-skills.md)
- [Skill metadata schema](docs/skill-metadata-schema.md)
