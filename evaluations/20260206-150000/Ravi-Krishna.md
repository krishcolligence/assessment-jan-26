# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ravi Krishna
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-06

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 3 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 3 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 3 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | — | 2 |
| Global. Communication | Clear Articulation | — | 3 |
| **Total Score** |  |  | **22/32** |

**Final Band:** 22–27 → *Strong — likely good fit, verify gaps in F2F*

**Minimum Thresholds:**
* Foundation traits (S1, S4): 3, 3 ✓
* Change Governance (S5.5): ≥2 ✓
* No section scores 1 ✓

**AI-determined Band:** Strong

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)
**Score: 3**

Ravi identifies ~12 entities including several implicit ones (phone, recipe book, containers, cutlery, invoice, vehicle) — going beyond what was explicitly stated. His process flow covers ~10 events in correct sequence and recognizes conditional branching: *"This, if it happens is another major event. When the customer changes requirements."* The dependency rule is stated clearly: *"When a change comes in, the neighbour MUST inform the chef of this change."* He lists 4 downstream effects spanning quantity of food, raw materials, supplies (cutlery), and delivery mode — touching multiple actors.

Falls short of 4 because entity identification is presented in narrative style rather than clean structural extraction (e.g., *"There is a phone linked to the business where calls come in, maybe separate or same as personal"* — speculative description rather than structural listing). Misses some key implicit entities like availability slots, order status, and ingredients as distinct from shopping list items. The linking mechanism in 1.4 (confirmation call) is procedural rather than structural.

### **S2. Information Synthesis**
**Traits:** Modeling from Narrative (primary), Prioritization (secondary)
**Score: 3**

Good creative reframing of the core contradiction: *"10% is likely an average number which might reinforce the claim that evening crowd is high with buses running at 110% capacity."* Proposes an insightful redistribution solution: shift morning buses to evening peak. His balanced solution (2.3) creatively uses driver phones as GPS substitutes — addressing students (tracking), admin (no new budget), and drivers (route planning). Proposes success metrics (adoption, satisfaction, <1% location error) showing product thinking.

Weaknesses: 2.1 synthesis has an inaccuracy — states "all three agree GPS is needed" when drivers actually say GPS devices didn't work well. The solution focuses heavily on GPS/tracking rather than addressing boarding speed or route optimization equally. Missing information (2.4) is actionable (parent data, per-period capacity, GPS failure root cause).

### **S3. Finding Patterns**
**Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)
**Score: 3**

Pattern correctly identified and described in three general steps: *"The service is fine and non-stressed during normal hours. The demand rises above available resources during peak hours. When this happens, the resource is overstretched and this causes degraded service."* Good cafeteria application with a detailed practical solution (staggered entry: *"500 students divided into 4-5 batches of 20 minutes each"*).

In 3.4, correctly identifies the need for a *"living document that tracks the availability of stalls"* shared between all heads. However, fails to distinguish between temporal resource contention (WiFi/gym/printer) and informational collision (fest stalls). Instead, lumps both under *"lack of available resources compared to the need"* — missing the key insight that the fest problem is about information synchronization, not demand concentration.

### **S4. Diagnostic Reasoning**
**Traits:** Diagnostic Reasoning
**Score: 3**

Begins with an architecture diagram showing understanding of timer internals: *"[Input] → [Convert HH:MM:SS to seconds] → [Check every second] → If Yes [Ring] / If No [Check again]."* Lists 4 hypotheses across software and hardware: time conversion error, system clock inconsistency under load, check failure, faulty speaker. Tests are specific: unit test for conversion function, CPU usage check, iteration speed verification, isolated speaker test.

Falls short of 4 because only 4 hypotheses (not 5+) and all are relatively close in domain (no environmental factors like battery saver, no user behavior factors, no multitasking interference). 4.3 jumps to a specific diagnosis (*"main thread is blocked... implementing threading"*) rather than describing a systematic isolation methodology (change one variable at a time, repeated trials).

### **S5. Prioritization & Change Governance**
**Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)
**Score: 3**

**5.1-5.4:** Correctly identifies text Q&A as feasible and voice as unrealistic. Feature selection shows product thinking: conversational chatbot, link to source truth, chat history. Detailed 28-day plan with specific day ranges and role assignments. However, plan is overly ambitious for beginners (includes stress testing, penetration testing, vector DB, RAG architecture). Assumes specialized team roles (*"Two members are skilled in frontend dev, one is backend and one is an AI/agent dev"*) — contradicting the "all beginners" constraint. Backup plan is practical: narrow to core platform, defer features.

**5.5:** Chooses option (ii) — show answers immediately, let students flag. Justification includes building a wrong-answer database and *"verified human feedback data which is very valuable for Reinforcement learning."* This is the riskier governance choice (students get wrong info first) but provides a pragmatic rationale. For tracing (5.5b), identifies that session data and user feedback are needed. For the fix (5.5c), addresses all three requirements with specific mechanisms: (i) *"Correct the data and update the RAG database"*, (ii) *"find where the question was asked according to the session id and send callback notifications"*, (iii) *"implement a generator validator agent"* to prevent future errors. Strong governance thinking.

### **S6. Rapid Domain Learning**
**Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)
**Score: 2**

Explanation uses a car service station analogy — different from the bank example but stays close to counting/tracking patterns. Applications are reasonable but obvious: parking garage (entry/exit tracking instead of per-bay sensors) and logistics warehouse (sign-in/sign-out inventory). Both are inventory-tracking variants.

**Critical issue in 6.3:** States *"The idea is clear, No questions"* — a red flag. The rubric explicitly values acknowledging genuine gaps over claiming full understanding. Event sourcing has well-known complexities (replay performance, error correction, query complexity) that should prompt questions.

In 6.4, creates an event table with Cook Informed column — a creative addition connecting to S1. However, incorrectly states *"This would not help with mixed up lists"* — event sourcing with order-linked events directly addresses list traceability since every shopping event would reference its source order.

### **S7. Reflection**
**Traits:** Reflective Thinking
**Score: 2**

7.1: Pattern finding easiest — *"prior experience with real world problems"*. Experience-based reasoning, not cognition-based insight. 7.2: Good specific insight: *"without the code in front of me, it is hard to hypothesize a coding issue"* — identifies the gap between abstract and concrete debugging. 7.3: Describes a generic business process template: *"get information → process → deliver → repeat"*. Too generic to qualify as a structural extraction method. 7.4: *"Code a simple timer, actually write code and then debug it"* — specific and actionable but only addresses S4. No awareness of cross-section connections (e.g., how S6.4 depends on S1, how S5.5 governance thinking applies broadly).

---

## **Strengths**

- Consistent product thinking throughout — proposes metrics, phased rollouts, user impact analysis
- Creative problem reframing (bus redistribution in S2, driver-phone GPS alternative)
- Strong governance response in S5.5 — addresses all three fix requirements with specific mechanisms
- Good at identifying downstream effects across multiple actors (S1, S3)
- Maintains engagement and detailed responses across all sections

**Exceptional Candidate Markers (if applicable):**
- S1 score of 4: No (scored 3)
- Connections between sections: Partial — S6.4 references S1 with Cook Informed column, but states event sourcing wouldn't help with mixed-up lists
- Spontaneous governance thinking before S5.5: No

---

## **Concerns / Weaknesses**

- S6.3: Claims full understanding with "No questions" — shows lack of intellectual humility or genuine engagement with concept limitations
- S6.4: Incorrectly states event sourcing wouldn't help with mixed-up lists — misses a key application
- S7: Reflection is surface-level — generic method description, no cognitive insight, no cross-section awareness
- S5: Overly ambitious plan (stress testing, pen testing, RAG) and assumes specialized roles despite "all beginners" constraint
- S2.1: Mischaracterizes GPS as universal agreement when drivers noted it didn't work well

**Red Flags to Note:**
- "The idea is clear, No questions" in S6.3 may indicate reluctance to acknowledge uncertainty
- Plan ambition vs constraint awareness gap in S5 warrants F2F exploration

---

## **Final Recommendation (AI Generated)**

* **Strong**
  Ravi demonstrates consistent analytical thinking, creative problem-solving (bus redistribution, driver-phone GPS, session-based tracing), and strong governance instincts in S5.5. His main gaps are in reflective thinking (S7) and intellectual humility in learning (S6.3). Recommend F2F exploration of: (1) ability to acknowledge uncertainty and unknowns, (2) depth of reflective/meta-cognitive thinking, (3) calibration of plan ambition against real constraints.
