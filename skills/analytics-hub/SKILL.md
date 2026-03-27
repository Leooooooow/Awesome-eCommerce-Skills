---
name: analytics-hub
description: Route ecommerce analytics requests to the right specialized analysis skill and provide a clear entry point for sales, creator, product, customer, advertising, logistics, or financial analysis. Use when the user asks for any ecommerce analytics and needs the assistant to pick the correct analysis path.
---

# Analytics Hub

## What this skill solves

Route the request to the right analytics path before doing the work.

## Use when

- The user asks for ecommerce analytics but the exact analysis type is unclear
- The user wants a single entry point for multiple data questions
- The user needs help choosing between sales, creator, product, customer, logistics, or financial analysis

## Do not use when

- The request already clearly matches a specialized analytics skill
- The user only wants a one-off raw file read
- The task is unrelated to ecommerce data

## Inputs to ask for

Ask only for the minimum needed:
1. What they want to know
2. Time period
3. Any focus area, if they already have one

## Workflow

1. Clarify the business question.
2. Identify the best matching sub-skill.
3. Pull the relevant source files.
4. Run the specialized analysis.
5. Return a concise decision summary.

## Output requirements

Always include:
- The selected analysis path
- The core result
- The most important supporting metrics
- The recommended next action

## Quality standards

- Choose the narrowest useful analysis path
- Avoid duplicate reporting across skills
- Keep the routing decision obvious

## Safety / constraints

- Do not force the user through unnecessary clarifying steps
- Do not invent a sub-skill result if the analysis was not run
