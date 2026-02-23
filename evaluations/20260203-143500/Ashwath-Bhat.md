# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ashwath Ravindra Bhat
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-03

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 2 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 2 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | — | 2 |
| Global. Communication | Clear Articulation | — | 2 |
| **Total Score** |  |  | **17/32** |

**Final Band:** 16–21 → *Adequate — significant gaps, needs strong F2F performance*

**Minimum Thresholds:**
* Foundation traits (S1, S4): S1=3 ✓, S4=2 ✓
* Change Governance (S5.5): Present (minimally) ✓
* No section scores 1 ✓

**AI-determined Band:** Adequate

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 3 (Strong)**

**Entities (1.1):** Excellent systematic categorization into six groups:
- *Core business objects:* Customers, orders, event, guest count, menu, dishes, price estimate, final price
- *Planning & coordination:* Calendar, order record, menu plan, shopping list, ingredients
- *People:* Cook, helpers, delivery
- *Execution:* Prepared food, delivery, event date
- *Payment:* Payment, payment methods, payment record, payment book
- *Control:* Order ID, customer details, change requests

Identifies 25+ items including implicit ones (Order ID, change requests, final price vs estimate distinction). Shows strong structural thinking through categorization.

**Events (1.2):** Lists 15 events in clear sequence:
*"1. Customer calls to inquire → 2. Customer provides event details → 3. Owner checks availability → 4. Order accepted or rejected → ... → 14. Delivery → 15. Payment received"*

Includes branching (accepted/rejected, changes). Comprehensive coverage.

**Dependency (1.3):** States rule: *"When guest contacts to change the order details at the last minute, menu and shopping list must be updated before shopping."* Lists 4 downstream effects: food quantity, shopping list, estimated price, delivery quantity. Correct but effects don't fully span multiple actors (focused on quantities).

**Traceability (1.4):** Lists: Order ID, Customer name, Event date, Guest count, Quantity of items, Total price. States: *"Each shopping list must represent a single order and every order generates its own shopping list."* Good traceability concept.

### **S2. Information Synthesis**
**Score: 2 (Adequate)**

**Synthesis (2.1):** Lists agreements (delays, evening demand, inefficient system) and disagreements (students want buses vs budget; GPS discontinued; driver issues). However, this is a list format without true synthesis—doesn't identify the core tension or reconcile perspectives.

**Contradiction Handling (2.2):** *"Allocate buses from morning empty buses to evening demand. Reschedule buses based on demand pattern. Reduce delays by improving boarding speed."* Reasonable but stated without creative reframing of the contradiction.

**Solution (2.3):** Lists:
- *"1. Demand-based scheduling"*
- *"2. Operational improvement - Use routes with less traffic, Speed up ID scanning"*
- *"3. Instead of real-time tracking, use scale & time based approach to give estimated arrival time"*

Practical but brief and not well-developed. Doesn't fully address all stakeholder concerns.

**Missing Information (2.4):** *"Use empty buses in morning routes to areas where students stay. Use dashboards and mobile checklist for drivers."* This doesn't answer the question—these are solutions, not missing information that would help make a better recommendation.

### **S3. Finding Patterns**
**Score: 2 (Adequate)**

**Pattern (3.1):** *"Usage is not evenly distributed. Sometimes same resources used at the same time."* Correct but stays concrete rather than abstracting.

**General Description (3.2):** *"When many people use shared resources at same time, it is a pattern."* Very brief and somewhat circular. Doesn't articulate the concept of peak demand vs average capacity.

**Application (3.3):** *"Students come at same time from different sections. Cafeteria looks empty otherwise."* Correct identification. Solutions: *"Extend serving hours. Different lunch timings for departments."* Reasonable but brief.

**Pattern Distinction (3.4):** *"Communication issues due to lack of real-time information sharing."* Identifies the information gap but doesn't compare or contrast with the temporal pattern from WiFi/gym/printer. No articulation of how the fest stall problem differs from or relates to the earlier examples.

### **S4. Diagnostic Reasoning**
**Score: 2 (Adequate)**

**Hypotheses (4.1):** Only 3 hypotheses listed:
- *"System depends on device clock"*
- *"App slowdown on heavy processing"*
- *"App calculating seconds incorrectly"*

Limited diversity—all software/system focused. Missing hardware hypotheses (speaker, battery), environment hypotheses (phone sleep mode, background apps, multitasking), and timing mechanism hypotheses (race conditions, UI vs actual timer).

**Tests (4.2):** Three tests:
- *"Compare system clock with external stopwatch"*
- *"Check CPU load"*
- *"Use start & end timestamps"*

Reasonable but minimal. Tests don't clearly isolate single variables.

**Root Cause (4.3):** *"Run tests multiple times and compare results."* Very brief with no real isolation strategy. Doesn't describe how to narrow down from multiple possibilities.

### **S5. Prioritization & Change Governance**
**Score: 2 (Adequate)**

**Feasibility (5.1):** Easy: *"Answer top 30 questions"* (notably reduces from 50), static/well-defined, web-based. Difficult: text & voice input, speech recognition. Reasonable assessment.

**Priorities (5.2):** *"Mobile web based implementation. Scope-controlled answers. Text based FAQ."* Very basic list without clear rationale for why these matter most.

**Plan (5.3):**
- *"Week 1: Collect questions & answers, decide format & UI flow"*
- *"Week 2: Implement logic & interface, keyword matching"*
- *"Week 3: Exams ongoing, bug fixes"*
- *"Week 4: Improve based on feedback & deploy"*

Reasonable structure but minimal detail on who does what or how constraints are managed.

**Backup (5.4):** *"Focus only on core features. Stability over completeness. Remove features if needed."* Generic—doesn't specify which features would be cut.

**Change Governance (5.5):** Response is merged/unclear:
- *"Answer only when confident"* (option iii)
- *"Track questions, keywords, answers"*
- *"Check FAQ database. Review & flag wrong answers"* (option ii)
- *"Maintain history"*

Does not clearly:
- **(a)** Make a single choice with trade-off reasoning
- **(b)** Describe what specific data would be needed to trace a wrong answer
- **(c)** Address all three requirements (stop harm, identify affected students, prevent recurrence) with concrete mechanisms

### **S6. Rapid Domain Learning**
**Score: 2 (Adequate)**

**Explanation (6.1):** *"To-do list approach instead of instructions."* This is too vague to serve as an analogy. Doesn't explain what event sourcing means in concrete, accessible terms.

**Applications (6.2):** *"Online food order flow. College attendance flow."* Just example names without any explanation of why event sourcing would be useful or how it would work in these contexts.

**Unclear Parts (6.3):** *"Decide how long history should be stored."* Identifies one relevant unclear part, showing some engagement with limitations.

**S1 Connection (6.4):** Lists events:
- *"Event created"*
- *"Guest updated"*
- *"Menu updated"*
- *"Shopping list created"*
- *"Shopping complete"*

Connection to S1 present but superficial. Doesn't explain HOW this structure would help with the forgotten changes or mixed-up lists problems.

### **S7. Reflection**
**Score: 2 (Adequate)**

**Easy (7.1):** *"Section 3 was easiest."* No reasoning provided.

**Hard (7.2):** *"Sections 5 & 6 were hardest."* No reasoning provided.

**Method (7.3):** *"Broke business into parts - People, Events, Information, Changes."* Shows a categorization approach, which aligns with the strong S1 performance. However, brief.

**Improvement (7.4):** *"With more time, would improve understanding and efficiency."* Generic—not specific or actionable.

### **Global. Clear Articulation**
**Score: 2 (Adequate)**

- Uses structure (headers, bullet points, categories)
- Many answers are extremely brief—bullet lists without explanation
- Key reasoning often missing or implied rather than stated
- Under-explained in most sections, making it hard to assess depth of understanding
- Strong categorization in S1 not maintained consistently across other sections

---

## **Strengths**

* **Systematic categorization (S1):** Exceptional organization of entities into logical groups (Core, Planning, People, Execution, Payment, Control)
* **Comprehensive event listing:** 15 events in S1.2 with proper sequencing and branching
* **Practical thinking:** Solutions are generally practical and achievable
* **Structure awareness:** Uses headers and bullets consistently

**Exceptional Candidate Markers:**
- S1 score of 4: No (scored 3)
- Connections between sections: Superficial — 6.4 lists events but doesn't explain how they solve S1 problems
- Spontaneous governance thinking before S5.5: Not observed

---

## **Concerns / Weaknesses**

* **Consistent under-explanation:** Nearly every section lacks the reasoning behind answers. Bullet points without context make it difficult to assess depth of understanding.
* **Synthesis weakness (S2):** Lists information rather than truly synthesizing across sources. 2.4 answers with solutions instead of missing information.
* **Limited diagnostic breadth (S4):** Only 3 hypotheses, all software-focused. No isolation methodology described.
* **Incomplete governance response (S5.5):** Doesn't make a clear choice, doesn't specify tracing data, doesn't address all three fix requirements distinctly.
* **Vague learning transfer (S6):** Cannot explain event sourcing in accessible terms or articulate why applications would benefit from it.
* **No reflective depth (S7):** Identifies easy/hard sections without any reasoning about why or what about their cognition made it so.

**Red Flags to Note:**
- Retelling story instead of extracting structure (S1): No — excellent structure extraction
- Only thinks about happy path in governance (S5.5): Partial — mentions tracking and flagging but doesn't address affected student identification clearly
- No traceability thinking: Partial — present in S1.4 but weak in S5.5
- Labels without reasoning in reflection (S7): Yes — 7.1 and 7.2 are just labels

---

## **Final Recommendation (AI Generated)**

**Adequate**

Ashwath demonstrates strong structural thinking in S1 with excellent entity categorization, suggesting good analytical foundation. However, consistent under-explanation across other sections makes it difficult to assess reasoning depth. Key gaps include synthesis ability (S2), pattern abstraction (S3), diagnostic methodology (S4), and governance thinking (S5.5). The brief responses may indicate time pressure, surface-level engagement, or difficulty articulating reasoning. Recommended for F2F only if strong F2F performance is expected. In F2F, probe: (1) reasoning behind brief answers to assess depth vs. articulation gap, (2) ability to synthesize contradictory information verbally, (3) change governance scenarios to test proactive thinking about failure modes.
