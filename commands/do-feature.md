---
description: |
  Execute feature with team of agents — waves, reviews, commits.

  Use when: "выполни фичу", "do feature", "execute feature", "запусти фичу"
---

# Do Feature

Execute a full feature using a team of agents.

## Step 1: Load Skill

When user runs `/do-feature {feature-name}`, follow these steps:

**Step 1:** Read the skill file: `skills/feature-execution/SKILL.md`

**Step 2:** Follow the instructions from that file.

## Step 2: Find Feature

1. User provides feature path or name
2. Read `work/{feature}/tech-spec.md` — verify exists and approved
3. Read `work/{feature}/tasks/` — verify task files exist
4. If tech-spec or tasks missing → stop, tell user what's needed

## Step 3: Execute

Follow the loaded feature-execution skill workflow.
The skill checks `checkpoint.yml` in Phase 1 and handles resume automatically.
