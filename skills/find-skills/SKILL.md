---
name: find-skills
description: Help users discover, evaluate, and install relevant agent skills when they ask how to do something, want a specialized workflow, or ask whether a skill exists for a task. Use when the user is looking for installable skills, productivity extensions, tooling help, or domain-specific workflows.
---

# Find Skills

## What this skill solves

Use this skill to quickly locate the best matching skill for a task, then give the user the exact install command and a short decision summary.

## Use when

- The user asks: “how do I do X?” and X may have an existing skill
- The user asks: “find a skill for X” or “is there a skill for X?”
- The user wants help extending agent capabilities
- The user needs a specialized workflow, template, or tool bundle

## Do not use when

- The task is simple general reasoning and does not need an installable skill
- The user asks for direct help with a one-off task and no skill discovery is needed
- The request is about unrelated file editing, coding, or browsing

## Inputs to ask for

Ask only for the minimum needed:
1. The task domain, if unclear
2. The exact job to be done
3. Any preferred ecosystem or platform, if relevant

## Workflow

1. Identify the domain and task.
2. Search for matching skills using the Skills CLI.
3. Compare the top candidates by trigger fit and scope.
4. Recommend the best match and explain why it fits.
5. Give the install command and a skills.sh link when available.
6. If no match exists, say so plainly and offer a direct workaround.

## Output requirements

Always respond with:
- The best-matching skill name
- One-line reason it fits
- The install command
- A link to learn more, if available
- A fallback option if no skill is found

## Quality standards

- Prefer the most specific skill, not the broadest one
- Keep search results short and decision-ready
- Avoid overexplaining the Skills CLI
- Do not recommend a skill unless the trigger is a clear match

## Safety / constraints

- Do not claim a skill exists unless you have verified it
- Do not install anything without user consent
- If no skill matches, be explicit and offer direct help instead
- Prefer simple commands over multi-step installation instructions

## Reference commands

```bash
npx skills find <query>
npx skills add <owner/repo@skill>
npx skills add <owner/repo@skill> -g -y
npx skills check
npx skills update
```
