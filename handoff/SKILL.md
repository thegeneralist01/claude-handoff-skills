---
name: handoff
description: Prepare a context handoff for continuing work in a new thread. Use when asked to /handoff, create a handoff, or prepare context for continuation.
disable-model-invocation: true
context: fork
agent: Explore
---

# Handoff Skill

## Purpose
Extract relevant context from the current conversation so the user can continue work seamlessly in a new thread. Focus on extraction, not generation — pull concrete facts from the conversation rather than inventing instructions.

## Goal for the new thread
$ARGUMENTS

If no goal was provided, state clearly at the top of the output: "No goal was specified. Please describe what you want to work on in the new thread."

## Your task

Scan the entire conversation and produce a ready-to-paste handoff message using the structure below. Be specific: include actual file names, method names, commands, and concrete details. Prioritize recent decisions and discoveries over early exploratory discussion. Keep it dense with signal — no filler.

---

## Context from previous thread

### Relevant files
<!-- List each file path that is directly related to the goal, contains reference code or patterns to follow, needs to be read/edited/created, or provides important constraints. One per line. -->

### What was done
<!-- 2–5 bullet points summarizing key work completed in this thread -->

### Key decisions & constraints
<!-- Decisions made and why, coding patterns to follow, libraries in use, style preferences, constraints stated by the user -->

### Technical details
<!-- Important APIs, methods, data structures, commands run and their outcomes, gotchas discovered -->

### Open questions / known issues
<!-- Anything unresolved, limitations found, or edge cases to watch out for -->

---

**Goal for this thread:** $ARGUMENTS
