---
marp: true
theme: ssc
paginate: true
title: Agentic Test-Driven Development
description: SSC Compact Course
---

<!-- _class: title -->
<!-- _paginate: false -->
<!-- _footer: "Last updated: 2026-05-26" -->

# Agentic Test-Driven Development

## Liam Keegan, SSC

---

# Tenative Outline

- Classical tests intro
- Coding with LLMs intro
- Classical TDD intro
- Agentic TDD: what changes, what stays the same
- Common failure modes
- Best practices
- Hands on
  - Could be fully hands on
    - But hard to coordinate, each student will rapidly diverge
  - Could be just me coding
    - Students interacting with me as we discuss what to do next, pros/cons of different approaches

---

# Failure modes

- local reasoning
  - LLMs only have a local view of the code
  - this makes them (relatively) bad at architecture / API decisions
  - making changes that are consistent with / take into account conventions/ preserve invariants from a large codebase
  - note they are bad at this relative to their ability to implement code, they can still be pretty good!
- code bloat
  - defensive coding
  - backwards compatibility
  - unnecessary complexity
  - "enterprise" coding style
- cheating
  - in particular when writing tests

---

# Older failure modes

These failure modes used to be very common but seem to have been largely fixed in recent models:

- incorrect code
  - code that doesn't compile
  - code that contains syntax errors
- hallucinations
  - uses an invented API call that doesn't exist
  - or invents a language feature
- convincing "at a distance" code
  - looks good at first glance
  - but lots of small details are wrong

---

# Getting what you ask for

LLMs are amazingly good at giving you what you ask for. But not always at giving you what you need.

---

# 