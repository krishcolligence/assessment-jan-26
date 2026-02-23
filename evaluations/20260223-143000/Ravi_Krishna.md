# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ravi Krishna
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-23

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 4 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 3 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 3 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 3 |
| S7. Reflection | Reflective Thinking | — | 3 |
| Global. Communication | Clear Articulation | — | 4 |
| **Total Score** |  |  | **26/32** |

**Final Band:** Strong — likely good fit, verify gaps in F2F

**Minimum Thresholds:**
* Foundation traits (S1=3, S4=3): PASS (both 2+)
* Change Governance (S5.5): PASS (2+)
* No section scores 1: PASS

**AI-determined Band:** Strong

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 3 | Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

**Entities (1.1):** Ravi identifies 12-15 entities including several implicit ones: phone ("maybe separate or same as personal"), cook's recipe book, vehicle for grocery shopping, containers, cutlery (plates, spoons, tissues, glasses), invoice, cash, and payment notes book. This "what must exist for the system to work" thinking is a strong signal. He also identifies the shopping list as "a dynamic list which might change based on customer need."

> "Then come containers to put the cooked food. And the food in itself is an object, delivered with all the cutlery and an invoice."

**Events (1.2):** Lists 11-12 events in correct sequence, including branching for customer changes. Notes decision events (availability yes/no) and dependent events ("An event dependent on the above event is the neighbour re-calling the cook").

**Dependency (1.3):** States rule clearly: *"When a change comes in, the neighbour MUST inform the chef of this change."* Identifies the structural issue: "there was no formal process to actually communicate it to the cook." Lists 4-5 downstream effects: food quantity, raw materials, cutlery/packaging, and delivery mode. Effects span different operational areas but don't explicitly trace through different actors as deeply as a 4 would require.

**Shopping List (1.4):** Identifies Order No., Event date, Name and Ph. No. as required fields on ALL pages. Proposes practical confirmation call mechanism during shopping event.

**Why 3 not 4:** Implicit entity identification is exceptional, but downstream effects cluster around "more quantity needed" rather than spanning distinct actors (cook, helper, customer, driver) with different consequences.

### **S2. Information Synthesis**
**Score: 4 | Traits:** Modeling from Narrative (primary), Prioritization (secondary)

**Synthesis (2.1):** Identifies all three stakeholders explicitly (Student=Customer, Admin=Manager, Drivers=Operator). Synthesizes across sources — notes all agree on GPS needs but for different reasons. Insightfully observes:

> "10% is likely an average number which might reinforce the claim that evening crowd is high with buses running at 110% capacity."

This quantitative reasoning distinguishes him.

**Contradiction (2.2):** Excellent reframing: "Reduction in number of buses in the morning, in combination with route planning to reduce overlaps... Apply those reduced buses to ply in the evening." Quantifies the benefit: "reduces the fuel used per person and increases the percentage of buses that run at just below 100% capacity."

**Balanced Solution (2.3):** Proposes creative tech solution: use driver's GPS phones as bus trackers (avoids separate GPS device costs). States assumptions explicitly. Proposes phased approach: location sharing first (biggest impact), dynamic route planning later. Defines success metrics: student satisfaction, app adoption, <1% location error.

**Missing Information (2.4):** Genuinely actionable items: parent data (missed stakeholder), morning/evening capacity data, and whether GPS pilot failure was due to adoption, technology, or reliability. Each would change the recommendation.

**Why 4:** Synthesizes across all three sources, creatively reframes contradiction with quantitative reasoning, solution addresses all stakeholders with phased deployment, and missing information is truly actionable.

### **S3. Finding Patterns**
**Score: 3 | Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

**Pattern (3.1-3.2):** Abstracts well in three parts: "Service is fine during normal hours → Demand rises above available resources during peak hours → Resource is overstretched causing degraded service."

**Cafeteria (3.3):** Correctly applies pattern: "Average occupancy is 40% because it is most likely empty for all other times compared to peak hours." Proposes specific solution: staggered entry for 500 students in 4-5 batches of ~20 minutes each. Very practical.

**Fest (3.4):** Identifies information gap: proposes "living document that tracks availability of stalls shared between all three heads" with real-time updates. However, concludes "All the problems link back to lack of available resources compared to the need" — doesn't clearly distinguish the temporal (peak demand) vs informational (coordination failure) patterns.

**Why 3 not 4:** Excellent pattern abstraction and application, but doesn't articulate the distinction between temporal contention (WiFi/gym/printer) and informational contention (fest stalls).

### **S4. Diagnostic Reasoning**
**Score: 3 | Traits:** Diagnostic Reasoning

**Approach:** Begins by diagramming the timer architecture: `[Input] → [Convert HH:MM:SS] → [Check every second] → [Ring alarm]`. This systematic decomposition before hypothesizing is a strong signal.

**Hypotheses (4.1):** 4 hypotheses spanning multiple categories:
1. Time conversion error (software logic)
2. System clock slow/inconsistent due to load (system/environment)
3. Check mechanism failing (software logic)
4. Speaker faulty, ringing inconsistently (hardware)

Also notes assumption: "pattern repeats the same for 3 minutes, 5 minutes" — validates the problem scope.

**Tests (4.2):** Proposes isolated tests: unit tests for conversion function, checking iteration speed (faster/slower than 1 second), speaker isolation test.

**Root Cause (4.3):** Proposes specific root cause hypothesis: frequent checking blocking the main thread with a resource-heavy loop. Suggests threading as solution. This shows good technical reasoning but jumps to a conclusion rather than describing a systematic narrowing process.

**Why 3 not 4:** 4 good hypotheses spanning hardware/software/system, tests isolate components, but only 4 hypotheses (not 5+) and root cause strategy jumps to conclusion rather than systematic elimination.

### **S5. Prioritization & Change Governance**
**Score: 3 | Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)

**Feasibility (5.1):** Correctly identifies text Q&A and fast responses as achievable, voice input as infeasible ("requires advanced TTS and STT systems which are not feasible for beginners").

**Top Features (5.2):** Conversational UI for FAQs, link to source truth (trust-building insight), and save chats. Rationale: user experience, user trust, customer satisfaction. The "link to source truth" is a sophisticated product insight.

**Plan (5.3):** Very detailed day-by-day plan with role assignments. However, **assumes skilled team members** (frontend devs, backend dev, AI dev) when the constraint says "all team members are beginners" — this is a notable gap.

**Backup (5.4):** Narrow to conversational platform, push link/storage features to later phase. Practical.

**Governance (5.5):**
- **(a)** Chooses option (ii) — show answers and let students flag. Reasoning: builds a database of wrong answers + "verified human feedback data which is very valuable for Reinforcement learning." Creative but doesn't acknowledge student harm risk (students get wrong info first).
- **(b)** Session-based tracing: "we have saved all chats with user session."
- **(c)** Addresses all three requirements concretely: correct data + update RAG database (stop harm), find by session ID + send callback notifications (identify affected), implement generator-validator agent (prevent future).

> "implement a generator validator agent where one gives information from source documents and another checks with VERIFIED EXTERNAL SOURCES"

**Why 3 not 4:** Governance is nearly exceptional (all three requirements addressed concretely), but the role assumption in 5.3 violates constraints, and option (ii) choice doesn't acknowledge student harm trade-off.

### **S6. Rapid Domain Learning**
**Score: 3 | Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

**Explanation (6.1):** Good paraphrase followed by novel analogy: car service station — track cars entering/exiting to know current capacity. Apt and different from the bank example.

> "If we keep track of the cars that enter the station from when it was empty and track the cars leaving the station, we can accurately tell the number of cars in the service station."

**Applications (6.2):** Two strong examples with reasoning:
1. Parking garage: sensors at each bay are expensive, track entry/exit events instead (cost-efficient + security audits)
2. Logistics warehouse: signed-in/signed-out inventory events (accountability + audit trail)

**Unclear Parts (6.3):** "The idea is clear, No questions." — This is a weakness. Claiming full understanding suggests insufficient critical engagement.

**S1 Connection (6.4):** Constructs specific event table for catering business (showed intent → order for 50 → changed to +50 → paid in full). Correctly identifies how this prevents forgotten changes. Honestly notes "This would not help with mixed up lists" — though this is actually incorrect (event-linked lists would prevent mix-ups), the honesty is notable.

**Why 3 not 4:** Novel analogy, good applications with reasoning, and specific S1 connection. But 6.3 claims full understanding (red flag) and 6.4 connection is partially incorrect about mixed-up lists.

### **S7. Reflection**
**Score: 3 | Traits:** Reflective Thinking

**Easiest (7.1):** "Pattern finding section was the easiest. It was my prior experience with real world problems that helped me spot patterns." Self-aware about the source of ease (experience-based).

**Hardest (7.2):** "Section 4 felt the hardest because without the code in front of me, it is hard to hypothesize a coding issue." Specific insight about the constraint that created difficulty — not just "it was hard."

**Method (7.3):** Articulates a general business process template: "Any process involves getting information from a client → Process information & act on it → deliver results → Repeat. Once you spot this process, it is easy to analyze any business."

**Improvement (7.4):** "The only thing I would change is code a simple timer, actually write code and then debug it." Specific and actionable — directly addresses the weakness identified in 7.2.

**Why 3 not 4:** Good self-awareness, genuine method, specific improvement. But reflections are experience-based rather than cognition-based ("I've done this before" vs "I think in structures"). Doesn't connect sections in 7.4 (e.g., noting that S6.4 depended on S1 understanding).

### **Global. Clear Articulation**
**Score: 4 | Traits:** Clear Articulation (applied across entire test)

Ravi's answers are exceptionally well-structured throughout:
- Uses headers, numbered lists, and logical flow consistently
- States assumptions explicitly before answering (S2, S5)
- Diagrams the timer architecture before hypothesizing (S4)
- Quantifies where appropriate (bus utilization percentages, staggered batches of 120)
- Uses concrete examples effectively (phone-GPS solution, car service station, event table)
- Balances detail appropriately — thorough without being excessive

---

## **Strengths**

- Consistently strong systems thinking across all sections — sees processes, not just tasks
- Exceptional information synthesis with quantitative reasoning (S2 is the standout section)
- Creative problem-solving: phone-as-GPS-tracker, car service station analogy, generator-validator agent
- Product-oriented mindset: states assumptions, defines success metrics, proposes phased deployments
- Excellent written communication: structured, clear, and appropriately detailed throughout

**Exceptional Candidate Markers (if applicable):**
- S1 score of 4 (strongest signal for Foundry fit): NOT MET (S1=3)
- Connections between sections: PARTIAL — 6.4 references S1 with a specific event table; 7.4 connects S4 difficulty to actionable improvement; but 7.4 doesn't show broader integration
- Spontaneous governance thinking before S5.5: NOT MET

---

## **Concerns / Weaknesses**

- S5 plan assumes skilled team roles (frontend, backend, AI dev) despite "all beginners" constraint — doesn't fully internalize constraints
- Claims full understanding in S6.3 rather than identifying genuine gaps — suggests possible overconfidence
- S5.5 governance choice (option ii) doesn't acknowledge student harm risk from showing wrong answers
- S1 downstream effects cluster around quantity rather than spanning distinct actors
- S4 root cause isolation jumps to a conclusion rather than describing systematic elimination

**Red Flags to Note:**
- None critical. The constraint-violation in S5 and the overconfidence in S6 are areas to probe in F2F.

---

## **Final Recommendation (AI Generated)**

* **Strong** — Ravi is the clear standout in this cohort. His information synthesis (S2=4), articulation (Global=4), and consistent 3-level performance across all other sections demonstrate strong analytical and communication abilities. His product-oriented thinking (assumptions, metrics, phased approaches) and creative problem-solving are notable. Key areas to verify in F2F: (1) constraint internalization — does he work within limits or redefine them? (2) intellectual humility — the "no questions" response in S6 suggests probing, and (3) whether his strong analytical skills translate when working in a team of beginners rather than with assumed specialists.
