# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Aryan Pramod Khaire
**Application ID / Email:** aryan.khaire001@gmail.com
**Date of Evaluation:** 2026-02-23

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 2 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 2 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 2 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | — | 2 |
| Global. Communication | Clear Articulation | — | 2 |
| **Total Score** |  |  | **16/32** |

**Final Band:** Adequate — significant gaps, needs strong F2F performance

**Minimum Thresholds:**
* Foundation traits (S1=2, S4=2): PASS (both 2+)
* Change Governance (S5.5): PASS (barely, score=2)
* No section scores 1: PASS

**AI-determined Band:** Adequate (low end)

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 2 | Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

**Entities (1.1):** Lists ~10 items including roles (Owner, Customers, Cook, Helper, Driver) and data (Event Date, No. of guests, Type of food, Estimated Price, shopping list). Mostly explicit entities. "Number of guests" listed both as a role/person and as customer data, showing some confusion. No implicit entities identified.

**Events (1.2):** Compressed flow: "Customer → Owner → Check availability → Give price estimate → Cook → Shopping list → Cook food → Deliver → Payment." About 7-8 events but in abbreviated form. Includes branching for payment status.

**Dependency (1.3):** States "Dependency is functional dependency. If X depends on Y, changes in X affect Y." This is an abstract definition, not the specific rule. Doesn't say "When guest count changes, cook must be informed before shopping." Lists 4 effects: shortage of food, wrong estimated price, wrong items, mixing of shopping lists.

**Shopping List (1.4):** Proposes unique order ID and customer ID linked to shopping list. Correct concept. Answered before 1.2 (answered out of order).

**Why 2:** Entities are adequate but only explicit. Flow is compressed. The dependency is described abstractly rather than stated as a specific rule — "functional dependency" is a term, not an articulation. Linking concept is present.

### **S2. Information Synthesis**
**Score: 2 | Traits:** Modeling from Narrative (primary), Prioritization (secondary)

**Synthesis (2.1):** "Buses are crowded. Need proper routing. Only 40% buses full daily. GPS tracking not real-time." Restates facts from sources without clearly separating agreements vs disagreements.

**Contradiction (2.2):** "Instead of new buses, re-route efficiently. All buses should handle equal number of students." Basic idea of redistribution but very brief, no reasoning.

**Solution (2.3):** "Balance routes. Restart GPS. Increase trips in evening." One sentence, no depth, doesn't draw from all three sources.

**Missing Information (2.4):** "Increase budget and use small buses. Maintain GPS. Do ID scanning at bus stops." These are proposed solutions, not missing information — misunderstands the question.

**Why 2:** Mostly restates information. Solution is superficial. 2.4 fundamentally misunderstands the question (proposes solutions instead of identifying information gaps).

### **S3. Finding Patterns**
**Score: 2 | Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

**Pattern (3.1):** "Systems become slow when many users use simultaneously." Correct but stays concrete (uses "systems" and "users").

**General Description (3.2):** "When many people need resource at same time → long waiting. Avoid with balancing techniques." Reasonable abstraction with a solution hint.

**Cafeteria (3.3):** Identifies: students occupy large tables, lunch rush, teachers/staff also occupy seats. "Large table" insight is interesting but doesn't clearly apply the peak demand pattern. No explicit solution proposed.

**Fest (3.4):** "Race condition: Both roles need same resource simultaneously." The "race condition" label is technically apt and shows some cross-domain thinking, but doesn't identify the information gap or distinguish patterns.

**Why 2:** Pattern partially correct but stays concrete. Cafeteria application is vague (doesn't clearly apply peak demand pattern). 3.4 uses an interesting analogy ("race condition") but doesn't address the information flow problem.

### **S4. Diagnostic Reasoning**
**Score: 2 | Traits:** Diagnostic Reasoning

**Hypotheses (4.1):** 4 hypotheses: improper state handling, lifecycle methods not executing, background tasks affecting logic, miscalculation in logs. All software-focused, specifically React/frontend jargon. No hardware, system, or environmental hypotheses.

**Tests (4.2):** Check timer reset, start time, interval, UI mounting/unmounting, performance tab, core logic math. Multiple things to check but not structured as isolated single-variable tests.

**Root Cause (4.3):** "Inspect each situation carefully." Not a strategy.

**Why 2:** Has 4 hypotheses (meets count) but they're all in one narrow category (React/frontend software). Tests are a checklist rather than isolated experiments. No root cause narrowing strategy.

### **S5. Prioritization & Change Governance**
**Score: 2 | Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)

**Feasibility (5.1):** "Exams in 3 weeks difficult. Can manage 2-3 hrs daily." Identifies a constraint but doesn't separate easy vs difficult features.

**Features (5.2):** FAQs, LLM, Good UI. Including "LLM" as a top feature is overly ambitious for a beginner team. No rationale for choices.

**Plan (5.3):** Week 1: Setup LLM + dependencies. Week 2: Train LLM. Week 3: Create UI. Week 4: Testing. "Train LLM" is unrealistic for beginners with no paid tools.

**Backup (5.4):** "Focus on minimal UI. Complete important backlog first." Brief but somewhat practical.

**Governance (5.5):** Chooses option (ii) — show and flag. "Admin can analyze wrong answers. Correct database if errors found." No trade-off reasoning, no tracing specifics, doesn't address identifying affected students or prevention.

**Why 2:** Plan is overly optimistic (training an LLM as beginners). Feature selection doesn't consider feasibility. Governance is basic — no trade-off analysis, no tracing, doesn't address all three requirements.

### **S6. Rapid Domain Learning**
**Score: 2 | Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

**Explanation (6.1):** Uses the bank account example — same as provided in the passage. Does not create an original analogy.

**Applications (6.2):** Crime scene (store event timestamps) and app crash (store error logs). Crime scene is somewhat creative but barely explained. App crash logs are a reasonable but conventional example.

**Unclear Parts (6.3):** "All parts of idea clear." Claims full understanding — red flag per rubric.

**S1 Connection (6.4):** Lists events as cost items: "Birthday: ₹1500, Marriage anniversary: ₹2500, Extra guests: ₹500..." This is a pricing breakdown, not event sourcing. Misapplies the concept — confuses event sourcing with cost tracking.

**Why 2:** Repeats the given bank example instead of creating original analogy. Claims full understanding (no genuine engagement with gaps). 6.4 misapplies event sourcing as cost tracking rather than recording state changes.

### **S7. Reflection**
**Score: 2 | Traits:** Reflective Thinking

**Easiest (7.1):** "Section 1, 3, 6 easiest." No reasoning.

**Hardest (7.2):** "Section 4 hardest." No reasoning.

**Method (7.3):** "Read paragraph multiple times and visualize." Minimal process articulation.

**Improvement (7.4):** "Should have attempted easier sections first." A strategy, but generic.

**Why 2:** Labels without reasoning in 7.1/7.2. 7.3 offers a minimal process ("read and visualize"). 7.4 is a basic test-taking strategy. Meets minimum for 2 but no genuine cognitive insight.

### **Global. Clear Articulation**
**Score: 2 | Traits:** Clear Articulation (applied across entire test)

- Uses section labels (Q1.1, Q1.2, etc.) for basic structure
- Answers are often very brief (one-liners for S2)
- Answered S1 questions out of order (1.4 before 1.2)
- Some answers are unclear or compressed
- 2.4 demonstrates misunderstanding of the question
- Understandable but disorganized

---

## **Strengths**

- Produces answers for all sections — doesn't leave any blank
- Shows basic pattern recognition (S3.4 "race condition" is an interesting cross-domain label)
- Identifies entities and process flow at a basic level in S1
- Has practical instincts in backup planning (S5.4)

**Exceptional Candidate Markers (if applicable):**
- None triggered

---

## **Concerns / Weaknesses**

- Consistently surface-level across all sections — no depth of reasoning
- Dependency rule in S1 articulated as abstract jargon ("functional dependency") rather than specific business rule
- Misunderstands questions: S2.4 (gives solutions instead of missing info), S6.4 (gives costs instead of events)
- Overly optimistic S5 plan (training an LLM as beginners with no budget)
- Claims full understanding of event sourcing (S6.3) while misapplying it in S6.4
- Reflection shows no genuine cognitive insight

**Red Flags to Note:**
- Pattern of surface-level engagement without genuine reasoning depth
- Misapplication of concepts after claiming understanding (S6)
- Tendency to use jargon without substance (S1.3 "functional dependency")

---

## **Final Recommendation (AI Generated)**

* **Adequate** (low end) — Aryan demonstrates basic competence across all sections, meeting minimum thresholds, but shows no genuine depth in any area. The consistent 2-level performance suggests he engages with problems at a surface level without drilling into underlying structure or reasoning. Key concerns: misunderstanding questions (S2.4, S6.4), jargon without substance (S1.3), and overly optimistic planning (S5). F2F should probe whether this surface-level pattern is due to time pressure or represents his natural analytical depth. The absence of any section at 3+ is a significant concern for an R&D role that requires deep analytical thinking.
