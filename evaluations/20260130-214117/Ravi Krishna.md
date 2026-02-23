# **R&D Engineering Aptitude Test - Evaluation Report**

**Candidate Name:** Ravi Krishna
**Application ID / Email:** N/A
**Date of Evaluation:** 2026-01-30

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1-4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 2 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | - | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | - | 2 |
| Global. Communication | Clear Articulation | - | 2 |
| **Total Score** |  |  | **18/32** |

**Final Band:** Adequate (16-21 -> Adequate - significant gaps, needs strong F2F performance)

**Minimum Thresholds Check:**
- S1 (>=2): Pass (3)
- S4 (>=2): Pass (2)
- S5.5 Change Governance (>=2): Pass (2)
- No section scored 1: Pass

**AI-determined Band:** Adequate

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

Rubric criteria: identify explicit + implicit entities, extract ordered process flow, express dependency as a rule with multiple ripple effects, and define clear traceability between list and source order.

Evidence: Mentions concrete entities like "events diary", "shopping list", and "payment notes book"; captures a rule: "When a change comes in, the neighbour MUST inform the chef"; and proposes traceability fields such as "Order No. on ALL pages" and "Event date on ALL pages."

Rationale: Good extraction of explicit items and a clear dependency rule. Some implicit system entities are missed (e.g., order, availability, ingredients), and ripple effects focus mostly on quantities rather than pricing/helper/driver impacts. Traceability is present but not fully specified (no order ID or creation date).
Score: 3
Section rank: 1/1

### **S2. Information Synthesis**
**Traits:** Modeling from Narrative (primary), Prioritization (secondary)

Rubric criteria: synthesize across sources, reframe contradictions, propose balanced solution covering all stakeholders, and request actionable missing information.

Evidence: States "All three stakeholders agree that GPS systems are needed" (overstates agreement). Handles the budget contradiction via reallocation: "Reduction in number of buses in the morning... apply those reduced buses... in the evening." Solution prioritizes GPS/app: "prioritize the mapping of buses to drivers via an app." Missing info includes "At what capacity buses run during the morning and evening."

Rationale: Some practical prioritization, but synthesis is flawed (GPS is not a full agreement) and the solution under-weights boarding delays and route planning. Missing info is partially actionable but incomplete.
Score: 2
Section rank: 1/1

### **S3. Finding Patterns**
**Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

Rubric criteria: abstract pattern in domain-independent language, apply correctly to new context, and distinguish temporal demand concentration from informational coordination in 3.4.

Evidence: Identifies "peak time crowd management" and explains "demand rises above available resources during peak hours." Applies it with "Staggered entry for lunch." For 3.4 suggests a "living document that tracks the availability of stalls."

Rationale: Pattern and application are correct. The 3.4 info-flow fix is good, but the underlying pattern is still framed as generic resource shortage rather than clearly distinguishing informational coordination vs temporal overload.
Score: 3
Section rank: 1/1

### **S4. Diagnostic Reasoning**
**Traits:** Diagnostic Reasoning

Rubric criteria: 5+ diverse hypotheses across categories, tests isolate single variables, and clear root-cause isolation strategy.

Evidence: Hypotheses include "conversion of time", "system clock might be slow", "check might be failing", and "speaker might be faulty." Tests include "write test cases for the isolated time conversion function," "check... every 1 second," and an "isolated speaker test." Root-cause step suggests "Implementing threading."

Rationale: Hypotheses are mostly software/hardware and tests are somewhat isolating, but the set is narrow and the root-cause method is a proposed fix rather than an isolation plan.
Score: 2
Section rank: 1/1

### **S5. Prioritization & Change Governance**
**Traits:** Prioritization Under Constraints (5.1-5.4), Change Governance Mindset (5.5)

Rubric criteria: realistic feasibility assessment, clear prioritization tied to constraints, practical plan and backup, and governance choice with trade-offs + traceability + full fix.

Evidence: Feasibility focuses on "Answering 50 top common questions" and "Fast responses," while noting "voice requires advanced TTS and STT." Top features are "clean UI", "Link to source truth", "Ability to upload images", and "Ability to save chats." Governance choice: "show answers quickly but let students flag wrong answers." Tracing is "need the information of why the student thinks the information given by the bot is wrong." Fix: "Correct the data and update the RAG database" and "send callback notifications."

Rationale: Prioritization misses core MVP elements (text Q&A, mobile-first, keyword search) and adds scope. Plan is structured but optimistic. Governance choice lacks trade-off reasoning, tracing is vague, and prevention is only partially addressed.
Score: 2
Section rank: 1/1

### **S6. Rapid Domain Learning**
**Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

Rubric criteria: novel analogy, non-obvious applications with reasoning, genuine unclear parts, and a specific Section 1 connection.

Evidence: Uses a "car service station" analogy and gives "parking garage" and "logistics warehouse" as applications. States "The idea is clear, No questions." For 6.4: "This would not help with mixed up lists."

Rationale: Analogy and applications show basic understanding, but there are no unclear parts, and the Section 1 connection is incomplete (does not show how event links prevent mixed-up lists).
Score: 2
Section rank: 1/1

### **S7. Reflection**
**Traits:** Reflective Thinking

Rubric criteria: specific insight into own cognition, explicit method for S1, and concrete improvement.

Evidence: "pattern finding section was the easiest" due to "prior experience with real world problems." Method is generic: "Any process involves getting information from a client... deliver results." Improvement: "code a simple timer."

Rationale: Reflection is experience-based rather than cognition-based, method is vague, and improvement focuses on tooling not approach.
Score: 2
Section rank: 1/1

### **Global. Clear Articulation**
**Traits:** Clear Articulation (applied across entire test)

Rubric criteria: structured answers, clear explanations, appropriate detail, concrete examples.

Rationale: There is some structure and bulleting, but several answers are incomplete or "text cut off," and reasoning occasionally drifts (assumptions and scope creep).
Score: 2

---

## **Strengths**

- Identifies core peak-demand pattern and applies it with a plausible operational fix (S3.1-3.3)
- Articulates a clear dependency rule and basic traceability fields for shopping lists (S1.3-1.4)
- Suggests a realistic capacity rebalancing tactic under budget constraints (S2.2)
- Provides a multi-week plan with explicit sequencing (S5.3)

**Exceptional Candidate Markers (if applicable):**
- None observed

---

## **Concerns / Weaknesses**

- Mis-synthesizes stakeholder inputs and over-weights GPS as a universal agreement (S2)
- Diagnostic reasoning is shallow with limited hypothesis diversity and weak isolation strategy (S4)
- Prioritization adds non-core features and governance lacks trade-off reasoning and traceability detail (S5)
- Limited reflective depth and weak method articulation for modeling tasks (S7)
- Event sourcing connection to mixed-up lists is incorrect or incomplete (S6.4)

---

## **Final Recommendation (AI Generated)**

**Adequate** - Shows baseline modeling and pattern recognition, but synthesis accuracy, diagnostic rigor, change governance, and reflective thinking are weak. Would require strong F2F evidence to mitigate these gaps.
