# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ashwath Ravindra Bhat
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-23

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 3 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 3 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | — | 2 |
| Global. Communication | Clear Articulation | — | 3 |
| **Total Score** |  |  | **21/32** |

**Final Band:** Adequate — significant gaps, needs strong F2F performance

**Minimum Thresholds:**
* Foundation traits (S1=3, S4=2): PASS (both 2+)
* Change Governance (S5.5): PASS (2+)
* No section scores 1: PASS

**AI-determined Band:** Adequate (top end)

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 3 | Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

**Entities (1.1):** Exceptionally well-organized into categories: Core business objects, Planning & coordination, People, Execution, Payment, and Control. Lists 20+ entities including some implicit ones: Order ID, Final price (distinct from estimate), Ingredients, Change requests. This structural categorization shows systems thinking.

> Categories: "Core business objects," "Planning & coordination objects," "People," "Execution," "Payment," "Control"

**Events (1.2):** 15 events in correct sequence from inquiry to payment. Includes branching (customer requests changes → order updated → cook updates menu).

**Dependency (1.3):** "When guest contacts to change the order details at the last minute, menu and shopping list must be updated before shopping." Correct rule. Lists 4 downstream effects: food quantity, shopping list, estimated price, delivery quantity.

**Shopping List (1.4):** Lists Order ID, customer name, event date, guest count, quantity, total price. Proposes one-to-one mapping: "Each shopping list must represent a single order and every order generates its own shopping list."

**Why 3 not 4:** Excellent entity categorization and event flow. Dependency rule is correct. However, downstream effects don't span different actors (all about quantities), and implicit entities, while present, don't show deep "what must be true for this to work" thinking (e.g., no phone, vehicle, kitchen capacity).

### **S2. Information Synthesis**
**Score: 3 | Traits:** Modeling from Narrative (primary), Prioritization (secondary)

**Synthesis (2.1):** Correctly identifies agreements (delays, evening demand, system inefficiency) and disagreements (students want more buses vs budget constraints, GPS discontinued, driver complaints about traffic/scanning).

**Contradiction (2.2):** Good practical reframing: reallocate morning buses to evening, reschedule based on demand, improve boarding speed. The redistribution idea addresses the core contradiction without requiring budget increase.

**Solution (2.3):** Three-pronged approach using all sources: demand-based scheduling, operational improvements (less traffic routes, faster scanning), and estimated arrival times as alternative to real-time GPS tracking. The ETA-based approach shows creative thinking.

**Missing Information (2.4):** Provides only 2 items (question asks for 3) and these read more as solutions than missing information: "Use empty buses in morning routes" and "dashboards for drivers." This is the weakest part.

**Why 3 not 4:** Good synthesis and creative reframing (redistribution, ETA-based tracking), but 2.4 misunderstands the question (provides solutions instead of missing information) and only 2 items instead of 3.

### **S3. Finding Patterns**
**Score: 3 | Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

**Pattern (3.1-3.2):** "Usage is not evenly distributed. Sometimes same resources used at the same time." Correct but could be more crisply abstracted.

**Cafeteria (3.3):** Correctly identifies peak timing as the cause. Proposes practical solutions: extend serving hours, different lunch timings for departments. Both are appropriate.

**Fest (3.4):** "Communication issues due to lack of real-time information sharing." Correctly identifies the information gap but doesn't connect it to or distinguish it from the temporal demand pattern in 3.1-3.3.

**Why 3 not 4:** Pattern correct, application reasonable with practical solutions, information gap identified in 3.4. But pattern abstraction could be cleaner (domain-independent language), and 3.4 doesn't distinguish temporal vs informational contention.

### **S4. Diagnostic Reasoning**
**Score: 2 | Traits:** Diagnostic Reasoning

**Hypotheses (4.1):** 3 hypotheses: system clock dependency, app slowdown on heavy processing, app calculating seconds incorrectly. All software-focused, no hardware or environmental hypotheses.

**Tests (4.2):** Compare system clock with external stopwatch, check CPU load, use timestamps. Reasonable but don't cleanly isolate single variables.

**Root Cause (4.3):** "Run tests multiple times and compare results." — Repetition is not a root cause isolation strategy.

**Why 2:** Only 3 hypotheses (rubric wants 4+), all in one category (software), tests are reasonable but don't clearly discriminate, and root cause strategy is just "repeat."

### **S5. Prioritization & Change Governance**
**Score: 3 | Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)

**Feasibility (5.1):** Good realistic assessment. Notably reduces scope proactively: "Answer top 30 questions" (down from 50). Text & voice correctly identified as difficult.

**Features (5.2):** Mobile web, scope-controlled answers, text-based FAQ. Practical choices.

**Plan (5.3):** Realistic weekly plan: Week 1 collect Q&A + design, Week 2 implement + keyword matching, Week 3 exams + bug fixes, Week 4 feedback + deploy. Respects the exam constraint.

**Backup (5.4):** "Stability over completeness. Remove features if needed." Clear principle-based approach.

**Governance (5.5):** Mixes approaches — "answer only when confident" (option iii) combined with "track questions, keywords, answers" and "review & flag wrong answers." Shows governance thinking but not structured around the three specific requirements (stop harm, identify affected, prevent recurrence).

> "Answer only when confident... Track questions, keywords, answers... Review & flag wrong answers... Maintain history"

**Why 3 not 4:** Good prioritization with proactive scope reduction, practical plan. Governance shows awareness of tracking/confidence but doesn't explicitly address all three requirements in 5.5(c) and doesn't trace through a specific incident path in 5.5(b).

### **S6. Rapid Domain Learning**
**Score: 2 | Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

**Explanation (6.1):** "To-do list approach instead of instructions." Very brief and the analogy is unclear — a to-do list doesn't clearly map to event sourcing.

**Applications (6.2):** Online food order flow and college attendance flow. Both plausible but presented without reasoning about *why* event sourcing would be beneficial in these cases.

**Unclear Parts (6.3):** "Decide how long history should be stored." One legitimate question about storage lifecycle, showing some engagement.

**S1 Connection (6.4):** Lists appropriate events: event created, guest updated, menu updated, shopping list created, shopping complete. Correct event decomposition for the catering business, showing understanding of how to apply the concept.

**Why 2 not 3:** Analogy in 6.1 is weak and unclear. Applications lack reasoning. One good question in 6.3. The S1 connection (6.4) is a positive signal, but overall the section shows surface-level understanding rather than genuine grasping of the concept.

### **S7. Reflection**
**Score: 2 | Traits:** Reflective Thinking

**Easiest (7.1):** "Section 3 was easiest." No reasoning for why.

**Hardest (7.2):** "Sections 5 & 6 were hardest." No reasoning for why.

**Method (7.3):** "Broke business into parts — People, Events, Information, Changes." This is an actual method — a categorization framework for decomposing a business narrative. This is the strongest part of the reflection.

**Improvement (7.4):** "With more time, would improve understanding and efficiency." Generic.

**Why 2:** 7.3 reveals a genuine analytical method (categorical decomposition), which is a positive signal. But 7.1/7.2 are labels without reasoning, and 7.4 is generic. The method in 7.3 elevates this above a 1 but the surrounding weakness keeps it at 2.

### **Global. Clear Articulation**
**Score: 3 | Traits:** Clear Articulation (applied across entire test)

Ashwath's answers are consistently well-structured:
- S1.1 uses meaningful categories (Core objects, Planning, People, etc.)
- Uses numbered lists and clear formatting throughout
- Answers are organized logically within sections
- Minor clarity issues: some answers are too brief (S6, S7), and 2.4 misunderstands the question
- Overall: mostly clear and organized with some gaps

---

## **Strengths**

- Strong structural thinking in S1 — categorizing entities into functional groups shows analytical instinct
- Practical, constraint-aware planning in S5 — proactively reduces scope from 50 to 30 questions
- Consistent 3-level performance across S1, S2, S3, S5 — shows broad competence
- Well-organized communication with clear formatting and logical flow
- Good pattern recognition with practical solutions (staggered times, redistribution)

**Exceptional Candidate Markers (if applicable):**
- S1 score of 4: NOT MET (S1=3)
- Connections between sections: PARTIAL — 6.4 connects to S1 with appropriate events
- Spontaneous governance thinking before S5.5: NOT MET

---

## **Concerns / Weaknesses**

- Diagnostic reasoning is weak (S4=2) — only 3 hypotheses, all software-focused, no isolation strategy
- Rapid domain learning shows surface understanding (S6=2) — analogy is unclear, applications lack reasoning
- Reflection lacks depth — can articulate a method (7.3) but doesn't reason about why sections were easy/hard
- 2.4 misunderstands the question (provides solutions instead of missing information)
- Several answers are too brief, especially in S6 and S7

**Red Flags to Note:**
- None critical. S4 weakness is the primary concern — diagnostic reasoning is a foundation trait.

---

## **Final Recommendation (AI Generated)**

* **Adequate** (top end) — Ashwath demonstrates solid analytical skills across most sections, with particular strength in structural thinking (S1) and practical planning (S5). His consistent 3-level performance in S1/S2/S3/S5 shows broad competence. However, weak diagnostic reasoning (S4=2) is a concern for an R&D role, and his domain learning (S6) and reflection (S7) suggest he may struggle with unfamiliar concepts and self-improvement. F2F should probe: (1) diagnostic reasoning depth — can he generate diverse hypotheses and design discriminating tests? (2) learning approach when encountering genuinely new concepts, and (3) depth of self-awareness about his thinking patterns.
