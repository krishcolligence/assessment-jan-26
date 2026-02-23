# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ashwath Ravindra Bhat
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-06

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 4 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 2 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 2 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | — | 1 |
| Global. Communication | Clear Articulation | — | 2 |
| **Total Score** |  |  | **17/32** |

**Final Band:** 16–21 → *Adequate — significant gaps, needs strong F2F performance*

**Minimum Thresholds:**
* Foundation traits (S1, S4): 4, 2 ✓
* Change Governance (S5.5): 2 (borderline) ✓
* No section scores 1: **FAILS — S7 = 1** ✗

**AI-determined Band:** Adequate (with threshold violation)

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)
**Score: 4**

Exceptional structural thinking. Entities are organized into clear categories — Core business objects, Planning & coordination, People, Execution, Payment, Control — demonstrating system-level thinking rather than narrative retelling. Identifies 20+ entities including implicit ones: Order ID, Change requests, Final price (distinct from estimate), Menu plan (distinct from menu), Ingredients (distinct from shopping list). The categorical organization itself reveals understanding of how the system is structured.

Process flow lists 15 events in correct sequence, closely matching the model answer. Includes branching (order accepted/rejected, customer changes). Dependency rule clearly stated: *"When guest contacts to change the order details at the last minute, menu and shopping list must be updated before shopping."* Four downstream effects identified: food quantity, shopping list, estimated price, delivery quantity.

Traceability thinking in 1.4 is strong: lists Order ID, Customer name, Event date, Guest count, Quantity, Total price on each shopping list, and states the structural rule: *"Each shopping list must represent a single order and every order generates its own shopping list."*

### **S2. Information Synthesis**
**Traits:** Modeling from Narrative (primary), Prioritization (secondary)
**Score: 2**

Agreements and disagreements are listed but not truly synthesized — more of a per-source summary. The core contradiction (students want more buses vs. budget constraint) is handled with a reasonable redistribution idea but without the creative reframing seen in stronger answers.

Solution (2.3) has reasonable elements: demand-based scheduling, operational improvements, estimated arrival time as GPS alternative. However, answers are very brief with no elaboration on implementation or stakeholder balance.

2.4 misunderstands the question — provides solution suggestions (*"Use empty buses in morning routes"*, *"Use dashboards for drivers"*) instead of identifying missing information that would improve recommendations. Only two items listed instead of three.

### **S3. Finding Patterns**
**Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)
**Score: 2**

Pattern identified (*"Usage is not evenly distributed"*, *"same resources used at same time"*) but stated too briefly to demonstrate deep abstraction. 3.2 is a single sentence that barely qualifies as domain-independent language.

Cafeteria application (3.3) is correct — identifies peak-time concentration and proposes reasonable solutions (extend hours, stagger timings). However, lacks the quantitative reasoning or detailed explanation that would demonstrate full understanding.

3.4 correctly identifies *"Communication issues due to lack of real-time information sharing"* but this is a single sentence with no comparison to the temporal patterns in 3.1-3.3 and no articulation of how the fest stall problem differs from demand concentration.

### **S4. Diagnostic Reasoning**
**Traits:** Diagnostic Reasoning
**Score: 2**

Only 3 hypotheses listed: (1) system depends on device clock, (2) app slowdown on heavy processing, (3) app calculating seconds incorrectly. All are software-related — no hardware hypotheses (speaker, battery), no environmental factors (multitasking, sleep mode, battery saver), no user behavior considerations.

Tests are reasonable but brief: compare with external stopwatch, check CPU load, use timestamps. Each checks one thing, which is correct methodology.

Root cause isolation (4.3) is entirely generic: *"Run tests multiple times and compare results."* No description of systematic variable isolation, no mention of controlled testing or changing one variable at a time.

### **S5. Prioritization & Change Governance**
**Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)
**Score: 2**

**5.1-5.4:** Reasonable prioritization — reduces scope to 30 questions (realistic given constraints), identifies voice as unrealistic. 4-week plan is practical and respects exam constraints. However, everything is stated at headline level without supporting rationale. Backup plan (*"stability over completeness, remove features if needed"*) is too vague — doesn't specify which features would be cut or what the minimum viable product looks like.

**5.5:** Answers are combined into a single undifferentiated block rather than addressing (a), (b), (c) separately. Appears to choose option (iii) — *"Answer only when confident"* — which is a strong governance choice, but provides no trade-off reasoning for why this is better than the alternatives. Mentions tracking questions, keywords, and answers (relevant to tracing) and reviewing/flagging wrong answers (relevant to fix), but doesn't address the three specific fix requirements: (i) stopping wrong answers immediately, (ii) identifying affected students, (iii) preventing future errors. Each is only vaguely touched upon without specific mechanisms.

### **S6. Rapid Domain Learning**
**Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)
**Score: 2**

Explanation (6.1) uses *"To-do list approach instead of instructions"* — this is an inaccurate analogy. A to-do list is a list of tasks to complete, not a record of all events that derive current state. The core insight of event sourcing (replaying events to reconstruct state) is not captured.

Applications (6.2) list "Online food order flow" and "College attendance flow" without any explanation of why event sourcing applies or how it would work in these contexts. The rubric requires reasoning, not just labels.

6.3 identifies one question: *"Decide how long history should be stored"* — a genuine concern about storage/performance, showing minimal engagement.

6.4 lists relevant events (event created, guest updated, menu updated, shopping list created, shopping complete) but provides no explanation of how this event log would help solve the S1 problems (forgotten changes, mixed-up lists). The connection exists structurally but is not articulated.

### **S7. Reflection**
**Traits:** Reflective Thinking
**Score: 1**

7.1: *"Section 3 was easiest."* No explanation of why or what about their thinking made it easier. 7.2: *"Sections 5 & 6 were hardest."* No explanation of what specifically was difficult. Both are labels without reasoning.

7.3: *"Broke business into parts — People, Events, Information, Changes."* This decomposition is actually a reasonable method (and is reflected in the strong S1 answer), but it is stated without any elaboration on the thinking process — how they decided on these categories, how they connected the parts, what they looked for.

7.4: *"With more time, would improve understanding and efficiency."* Entirely generic — no specific change in approach, no awareness of cross-section connections.

This matches the rubric's Score 1 anchor: labels without reasoning, cannot articulate process, no meaningful improvement.

### **Global. Clear Articulation**
**Traits:** Clear Articulation (applied across entire test)
**Score: 2**

S1 is well-organized with clear category headers and structured lists — demonstrating the candidate can produce well-articulated answers. However, from S2 onward, answers become increasingly terse. Many responses are single sentences or bare bullet lists without supporting reasoning. S5.5 combines all sub-questions into one block. S7 is four lines total for four questions.

The disparity between S1's quality and subsequent sections suggests either time management issues (spent too long on S1) or difficulty articulating reasoning beyond structured enumeration. Key points are present but frequently lack the supporting logic that would demonstrate understanding.

---

## **Strengths**

- Exceptional structural thinking in S1 — categorized 20+ entities systematically, demonstrating system-level understanding
- Strong traceability instinct in S1.4 — proposes one-to-one order-shopping list mapping with structural rule
- Practical constraint awareness — reduces scope to 30 questions, respects exam weeks, chooses confident-only answers
- Correct governance instinct in S5.5 — chooses option (iii) which prioritizes preventing harm

**Exceptional Candidate Markers (if applicable):**
- S1 score of 4: **Yes** (strongest signal for Foundry fit)
- Connections between sections: No — S6.4 lists events but doesn't explain how they solve S1 problems
- Spontaneous governance thinking before S5.5: No

---

## **Concerns / Weaknesses**

- Severe brevity from S2 onward — answers lack reasoning, rationale, and elaboration
- S7 scores 1 — violates the "no section should score 1" minimum threshold
- S6.1: Inaccurate analogy ("to-do list") suggests incomplete understanding of event sourcing
- S2.4: Misunderstands the question — provides solutions instead of identifying missing information
- No cross-section connections demonstrated anywhere in the assessment
- Potential time management issue: S1 is exceptional but remaining sections are uniformly thin

**Red Flags to Note:**
- S7 = 1 is a threshold violation. Inability to reflect on own thinking is a concern for R&D roles requiring meta-cognition.
- The quality drop from S1 (4) to the rest (all 2s and a 1) is the sharpest in this cohort. May indicate that structured decomposition is a strength but sustained analytical reasoning across different problem types is a gap.
- S6.1 inaccuracy suggests the candidate may not fully grasp new concepts but lists reasonable surface-level responses.

---

## **Final Recommendation (AI Generated)**

* **Adequate** (with threshold violation)
  Ashwath demonstrates exceptional structural thinking in S1 — the strongest S1 in this cohort, which is the highest-signal section for Foundry fit. However, this strength is not sustained: all subsequent sections score 2 or below, and S7 scores 1, violating the minimum threshold. The pattern suggests strong decomposition/categorization skills but difficulty with synthesis, abstraction, articulation of reasoning, and reflective thinking. Recommend F2F only if S1 performance is weighted heavily. F2F should probe: (1) whether the brevity reflects time pressure or reasoning limits, (2) ability to synthesize and argue trade-offs verbally, (3) reflective thinking capacity in a conversational setting.
