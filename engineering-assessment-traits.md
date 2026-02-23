# R&D Engineering Assessment: Trait Evaluation Framework

## Context

Foundry builds AI-native platform generating ERP systems from business conversations. Engineers must **master problems manually first** — extract structure from narratives, trace change ripples, design experiences backward from needs. Only then build agents automating this work.

Selection criteria: **see structure in chaos**, **trace consequences through systems**, **think in governed reversible changes**.

---

## Traits

### Foundation (Hard to Teach)

Weakness predicts struggle with core work.

| Trait | Definition | Strong Signal | Weak Signal |
|-------|------------|---------------|-------------|
| **Modeling from Narrative** | Extract entities, relationships, rules from unstructured descriptions; impose structure on ambiguity | Identifies implicit entities/dependencies; organizes messy info into clear categories; structural questions | Retains as narrative; misses implied relationships; surface-level categories |
| **Dependency & Ripple Reasoning** | Trace change propagation — "if X changes, what else?" | Spontaneous second-order effects; traces info flows between actors; recognizes dependency violations | Only direct effects; misses cross-actor impacts; treats changes as isolated |
| **Diagnostic Reasoning** | Generate multiple hypotheses; design discriminating tests | Multiple plausible causes across categories; single-variable isolation tests; root cause narrowing | One/two obvious hypotheses; non-discriminating tests; jumps to conclusions |

> **Scoring:** Modeling = entities, relationships, static structure. Ripple = second-order change effects. Score separately.

### Execution (Baseline Required)

Can sharpen with practice.

| Trait | Definition | Strong Signal | Weak Signal |
|-------|------------|---------------|-------------|
| **Prioritization Under Constraints** | Choose what matters when everything can't be done; defensible trade-offs | Must-have vs nice-to-have with reasoning; task dependencies; adjusts when constraints change | All requirements equal; no sequencing rationale; rigid under change |
| **Rapid Domain Learning** | Acquire working knowledge quickly; explain new ideas clearly | Accurate simple paraphrase; practical applications; articulates knowledge gaps; proposes deepening | Parrots definitions; superficial/wrong applications; no gap awareness |

### Growth (Trajectory Predictors)

Signal for technical leadership and automation design capability.

| Trait | Definition | Strong Signal | Weak Signal |
|-------|------------|---------------|-------------|
| **Pattern Recognition** | Notice common structure across contexts; abstract general principles | Domain-independent pattern articulation; correct novel application | Surface similarity only; abstraction too narrow/vague to transfer |
| **Reflective Thinking** | Awareness of own reasoning; what worked, what didn't, why | Describes problem-solving approach; identifies difficulty sources; adaptation suggestions | No process insight; external attribution only; no adaptation |
| **Change Governance Mindset** | Think traceability, reversibility, impact boundaries | Spontaneous "how to undo?"; identifies recording needs; recognizes blast radius | Happy path only; no reversal consideration; changes treated as permanent |

### Global Dimension

Applied across all sections, not standalone score.

| Dimension | Definition | Strong Signal | Weak Signal |
|-----------|------------|---------------|-------------|
| **Clear Articulation** | Express complex ideas simply and precisely | Organized, concise, logical flow; concrete examples; appropriate detail | Rambling/disorganized; over/under-simplified; missing key points |

---

## Assessed Elsewhere

| Trait | Method | Rationale |
|-------|--------|-----------|
| **Comfort with Ambiguity** | F2F interview, trial task | Requires live interaction, real-time decisions with incomplete info |
| **Collaboration Under Pressure** | F2F, pair programming | Requires interpersonal dynamics |
| **Domain Expertise** | Not selection criterion | Acquirable via rapid learning; hire for velocity not knowledge |

---

## Test Section Mapping

| Section | Primary Traits | Secondary |
|---------|----------------|-----------|
| S1 (business narrative)* | Modeling from Narrative | Dependency & Ripple |
| S2 (Bus System) | Modeling, Prioritization | — |
| S3 (Patterns) | Pattern Recognition | Dependency & Ripple |
| S4 (Timer) | Diagnostic Reasoning | — |
| S5 (Chatbot) | Prioritization | Change Governance (if 5.5 added) |
| S6 (domain concept)* | Rapid Domain Learning | Reflective Thinking |
| S7 (Reflection) | Reflective Thinking | — |

*Question design pending — framework applies once finalized.*

---

## Target Profile

Engineer who:
- **Perceives structure** in messy narratives
- **Traces ripples** through systems
- **Reasons through multiple hypotheses** systematically
- **Prioritizes under constraints**, learns domains rapidly
- **Recognizes patterns**, reflects on reasoning
- **Thinks reversibility and traceability** instinctively

Foundation for manual mastery today, automation design tomorrow.

---

## Implementation

| Item | Status |
|------|--------|
| S1 replacement (business narrative) | Pending |
| S6 replacement (domain concept) | Pending |
| S5.5 addition (governance question) | Pending |
| Candidate-facing simplified version | Pending |
| 0-3 rubric with sample answers | Recommended |
| Grader calibration session | Recommended |
