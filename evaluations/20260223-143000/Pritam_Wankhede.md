# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Pritam Wankhede
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-23

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 2 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 2 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 1 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 1 |
| S7. Reflection | Reflective Thinking | — | 1 |
| Global. Communication | Clear Articulation | — | 2 |
| **Total Score** |  |  | **13/32** |

**Final Band:** Weak — not recommended

**Minimum Thresholds:**
* Foundation traits (S1=2, S4=2): PASS (both 2+)
* Change Governance (S5.5): PASS (barely, score=2)
* No section scores 1: **FAIL** (S3=1, S6=1, S7=1)

**AI-determined Band:** Weak

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 2 | Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

**Entities (1.1):** Lists ~7 items: Number of guests, Food, Guest count, Menu, Price estimation, Diary, Dishes. "Number of guests" and "Guest count" overlap. Only explicit entities, no implicit ones.

**Events (1.2):** 4 compressed events: customer calls → inquires for booking → calls back for updates → preparation/delivery/payment. Misses many intermediate steps (availability check, menu planning, shopping list creation).

**Dependency (1.3):** Doesn't state a dependency rule. Instead discusses consequences: "If food is not enough, customers can cancel orders. Can order from outside for increased 50 people." Lists 3 downstream effects: preparation time, food items, more helpers needed. The effects are reasonable but the rule is missing.

> "If order is not fulfilled, customer may not order again in future." — Thinks about customer relationship, which shows some business awareness but doesn't address the structural dependency.

**Shopping List (1.4):** Customer name, categories of dishes, delivery day, items required. Basic information but no linking mechanism to source order.

**Why 2:** Entities are adequate (~7) but overlapping. Events are very compressed (missing key steps). No dependency rule articulated. Some reasonable downstream effects. Basic shopping list information without linking.

### **S2. Information Synthesis**
**Score: 2 | Traits:** Modeling from Narrative (primary), Prioritization (secondary)

**Agreements (2.1):** Real-time tracking, evening demand, routing plan. Somewhat correct but "real-time tracking" is not an agreement — students want it, admin dropped it, drivers say devices didn't work.

**Disagreements (2.1):** "Routes are confirmed so no need for more buses" and "budget cannot be increased." Partially captures the contradiction.

**Contradiction (2.2):** "Provide real-time tracking to save time. Morning buses are empty, so schedule proper time." Mentions redistribution idea but very briefly. Uses "student survey percentage to decide" — unclear how.

**Solution (2.3):** "Real-time tracking and routing plan." Very brief, essentially one idea.

**Missing Information (2.4):** "Interacting with students to create rules. WhatsApp group so if anyone is absent driver can change route." These are proposed actions, not missing information.

**Why 2:** Some synthesis present but superficial. Solution is brief and favors one approach (tracking). 2.4 misunderstands the question.

### **S3. Finding Patterns**
**Score: 1 | Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

**Pattern (3.1):** "Crowd increases at particular times, mainly closing or ending time." Partially captures the idea but focuses on "ending time" rather than peak demand generally.

**General Description (3.2):** "Scheduling time is important. Start working from start, not at end point." This is time management advice, not the resource contention pattern. Fundamentally misses the abstraction.

**Cafeteria (3.3):** "Give chairs only when needed; otherwise people who need them most may not get them on time." This doesn't apply the peak demand pattern. It's about allocation priority, not temporal concentration.

**Fest (3.4):** "Give importance to time. Do not wait till the end; otherwise preparation time may not be available." Completely misses the information gap between Sponsorship and Logistics heads. This is generic advice about time management.

**Why 1:** Partially grasps the pattern in 3.1 but cannot abstract it (3.2 becomes time management advice). Cannot transfer to new situations correctly (3.3 and 3.4 both miss the point). The fest answer shows no understanding of the information flow problem.

### **S4. Diagnostic Reasoning**
**Score: 2 | Traits:** Diagnostic Reasoning

**Hypotheses (4.1):** 4 hypotheses: time interval issue, rendering of component, running multiple times when called, variable redeclaration. All software-focused (component rendering suggests React/frontend thinking).

**Tests (4.2):** "Test proper implementation of setInterval. It works after the time set. Do not call the method with different times." One vague test instruction rather than isolated tests per hypothesis.

**Root Cause (4.3):** "Main issue is where timer interval happens; check rendering after that." Presumes a root cause rather than describing an isolation process.

**Why 2:** 4 hypotheses (adequate count) but all narrow to frontend software. Tests are vague and not isolated per hypothesis. Root cause strategy presumes rather than eliminates.

### **S5. Prioritization & Change Governance**
**Score: 2 | Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)

**Feasibility (5.1):** Mobile and top questions are easy; text + voice is difficult; beginners need time to learn. Reasonable.

**Features (5.2):** Timestamp for questions, text input over voice, device accessibility. "Timestamp for questions to answer oldest first" is an odd prioritization that doesn't align with FAQ chatbot purpose.

**Plan (5.3):** Not a weekly plan — lists principles: "understand question meaning," "answer oldest first," "prefer text." Doesn't create a work breakdown.

**Backup (5.4):** "Answer common questions to save time. Create information about nearby colleges." Tangential.

**Governance (5.5):**
- (a) Hybrid: "System answers when confident; otherwise human review." Reasonable approach but no trade-off reasoning.
- (b) "Check whether system data is updated on time." Vague tracing.
- (c) "After updates, database should also be updated. Can identify from student login account." Brief, doesn't clearly address all three requirements.

**Why 2:** Some feasibility awareness. Plan is not a plan but a list of principles. Feature selection is oddly focused (timestamps). Governance shows basic awareness but lacks structured thinking.

### **S6. Rapid Domain Learning**
**Score: 1 | Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

**Explanation (6.1):** "Use time everyday with planning." This does not explain event sourcing. It appears to be general life advice completely unrelated to the concept.

**Applications (6.2):** "Waking up and exercising every day. Working on time." These are daily habits, not event sourcing applications. Fundamentally misunderstands the concept.

**Unclear Parts (6.3):** "Almost clear about things, but getting real-time example requires thinking." Claims near-understanding while demonstrating no understanding.

**S1 Connection (6.4):** "Helpful for planning as amount is fixed; can know what items are left and what to buy additionally." Doesn't connect to event sourcing or address the S1 problems (forgotten changes, mixed-up lists).

**Why 1:** Cannot explain the concept. Applications are completely wrong (daily habits, not data storage patterns). No connection made to S1 problems. The answer strongly suggests the candidate did not understand the event sourcing passage.

### **S7. Reflection**
**Score: 1 | Traits:** Reflective Thinking

**Easiest (7.1):** "Finding pattern is easiest as it shows meaning in different patterns related to coding." Vague reasoning that doesn't explain why it was easy for this person specifically.

**Hardest (7.2):** "Section 6 is small." Unclear what this means — possibly "the passage was short" or "the section was small"? No reasoning about difficulty.

**Method (7.3):** "Customer orders may get updated sometimes with less time to work; need to handle such situations." This describes a business scenario, not a thinking process for extracting structure.

**Improvement (7.4):** "Quick thinking helps to be more productive, save time, and add more things." Generic motivational statement, not an actionable improvement.

**Why 1:** No meaningful reflection on own cognition. Cannot articulate a thinking process (7.3 describes a business scenario instead). No actionable improvement. Answers suggest difficulty understanding what the questions are asking.

### **Global. Clear Articulation**
**Score: 2 | Traits:** Clear Articulation (applied across entire test)

- Uses numbered points and lettered sub-items for basic structure
- Many answers are tangential or miss the question's intent (S3.2-3.4, S6.1-6.2, S7.3)
- Some answers ramble or include irrelevant detail
- Understandable when on-topic but frequently off-topic
- Core ideas are present in some sections (S1, S4) but buried

---

## **Strengths**

- Attempts all sections — doesn't leave blanks
- Shows some business awareness in S1 (customer relationship thinking)
- Basic feasibility assessment in S5.1 (correctly identifies voice input as difficult)
- S5.5(a) chooses a reasonable hybrid approach

**Exceptional Candidate Markers (if applicable):**
- None triggered

---

## **Concerns / Weaknesses**

- Fundamental misunderstanding of event sourcing (S6) — explains it as daily routine planning
- Cannot abstract patterns (S3) — pattern becomes time management advice instead of resource contention
- Reflection (S7) shows inability to articulate own thinking process
- Frequently misunderstands what questions are asking (S3.4 as time management, S6.1 as life advice, S7.3 as business scenario)
- Three sections score 1 — fails minimum threshold check

**Red Flags to Note:**
- Complete conceptual misunderstanding in S6 (daily habits ≠ event sourcing)
- Inability to transfer patterns to new situations (S3)
- Answers to reflection questions suggest limited metacognitive awareness

---

## **Final Recommendation (AI Generated)**

* **Weak** — Pritam fails the minimum threshold check with three sections scoring 1 (S3, S6, S7). The most concerning patterns are: (1) fundamental conceptual misunderstanding — the event sourcing section reveals inability to grasp and apply a new concept from written material, (2) inability to abstract — Section 3 shows pattern recognition that cannot be transferred or generalized, and (3) weak metacognition — cannot articulate own thinking processes. While S1 and S4 meet minimum thresholds and show basic competence, the overall profile does not indicate readiness for R&D work that requires rapid learning, pattern abstraction, and reflective thinking. Not recommended for advancement.
