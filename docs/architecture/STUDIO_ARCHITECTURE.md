# STUDIO ARCHITECTURE
Version: 0.1
Status: Draft
Last Updated: 2026-07-27

---

# Purpose
This document defines the structural architecture of the AI Research & Development Studio —
how its layers are organized and how they relate to each other.
It does not describe workflow (see STUDIO_OPERATING_MODEL.md) or belief/purpose (see STUDIO_VISION.md).

---

# Current State
At present, the Studio is operated by a single person.
All roles defined in the Operating Model (Strategy, Research, Engineering, Validation, Product)
are performed by the same individual, in sequence or in parallel, as needed.

"Departments" in this document refer to functional stages of work, not organizational units.
No AI agents or additional personnel are currently assigned to any layer.

---

# Structural Layers

```
AI Research & Development Studio
│
├── Foundation
│
├── Operating System
│      ├── Strategy
│      ├── Research
│      ├── Engineering
│      ├── Validation
│      └── Product
│
├── Knowledge
│
└── Projects
       └── (to be defined as products emerge)
```

## Foundation
Defines identity and purpose. Contains README.md, STUDIO_VISION.md, STUDIO_OPERATING_MODEL.md, STUDIO_ARCHITECTURE.md.
This layer is stable and changes rarely.

## Operating System
Defines how work moves from signal to value (see STUDIO_OPERATING_MODEL.md for detail).
This layer is process, not people — it does not assume any particular team size.

## Knowledge
Stores what has been learned: research notes, decisions, validated and invalidated assumptions.
This layer grows continuously and is the Studio's long-term memory.

## Projects
Holds the actual products the Studio produces.
This layer is intentionally left open — no specific products are named at the architecture level.
Each product manages its own internal structure independently.

---

# Cross-Layer Relationships

```
Operating System  ──produces──▶  Projects
Projects          ──generates──▶  Knowledge (lessons, results)
Knowledge         ──informs────▶  Operating System (future decisions)
```

The Studio does not treat Projects as permanent. Projects may start, evolve, or end.
The Operating System and Knowledge layers persist independently of any single project's lifecycle.

---

# Extension Rule
When a new product is created, it is added under `projects/` without modifying the Operating System.
When a new capability is needed (e.g. a new department, a new AI agent role), it is added to the
Operating System only if it serves an active, validated need — not in anticipation of future scale.

---

# Scope
This document defines structure only. It does not define workflow steps (Operating Model)
or long-term intent (Vision). It does not assign specific people, AI models, or tools to any layer —
that responsibility belongs to a future document once real needs emerge.

---
End of Document
