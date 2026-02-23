# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ravi Krishna
**Application ID / Email:** —
**Date of Evaluation:** 30/01/2026

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 3 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 2 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 2 |
| S7. Reflection | Reflective Thinking | 2 |
| Global. Communication | Clear Articulation | — | 3 |
| **Total Score** |  |  | **20/32** |

**Final Band:** Adequate — significant gaps, needs strong F2F performance

**Minimum Thresholds:**
* Foundation traits (S1, S4): S1=3 ✓, S4=2 ✓ (meets minimum)
* Change Governance (S5.5): 2 ✓ (meets minimum)
* No section scored 1 ✓

**AI-determined Band:** Adequate (20/32)

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Traits:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

**Score: 3 — Strong**

**Rationale:**

*1.1 Entities (Strong):* Candidate identifies 10+ entities including diary, phone, menu, shopping list, driver, vehicle, containers, food, cutlery, payment, payment notes book. Shows some implicit thinking (e.g., "maybe separate or same as personal" for phone, "recipe book" for cook). However, misses key implicit entities like: availability/time slots, order status, customer type, credit/account balance.

*1.2 Events (Strong):* Lists ~10 events in roughly correct sequence: customer calls → noting details → availability decision → menu planning → shopping list → changes if any → informing cook → purchasing → cooking → packing/quality checks → delivery → payment recording. Recognizes branching ("Yes/No based on availability") and conditional events (customer changes). Good structural thinking.

*1.3 Dependency (Strong):* Correctly states: "When a change comes in, the neighbour MUST inform the chef of this change." Lists downstream effects: quantity of food, raw materials, cutlery items, mode of delivery. However, only lists 4 effects and they're mostly quantity-related—doesn't span multiple actors (misses: price revision, preparation time, payment amount changes).

*1.4 Traceability (Strong):* Identifies needed info: Order No., Event date, Name and Phone. Proposes linking via phone number and suggests confirmation call. Concept is present but the "confirmation call" approach is manual rather than systemic.

**Evidence:** "Order No. on ALL pages. Event date on ALL pages. Name and Ph. No. of the source."

---

### **S2. Information Synthesis**
**Traits:** Modeling from Narrative (primary), Prioritization (secondary)

**Score: 3 — Strong**

**Rationale:**

*2.1 Agreements/Disagreements (Strong):* Candidate correctly identifies GPS as something all three sources touch on, and correctly notes the evening demand issue. However, the analysis conflates "agreeing GPS is needed" when actually Admin discontinued it and drivers said devices didn't work—this is more nuanced than presented.

*2.2 Contradiction Handling (Strong):* Good creative reframing: "Reduction in number of buses in the morning, in combination with route planning to reduce overlaps" and "Apply those reduced buses to ply in the evening." This is the distribution insight the rubric looks for. Also correctly calculates that "10% is likely an average number."

*2.3 Solution (Strong):* Proposes driver-phone GPS solution as practical alternative, with phased approach (location sharing first, dynamic routing later). Mentions success metrics. Solution addresses student need (real-time tracking) within budget constraints (using existing driver phones). However, doesn't fully address all three stakeholder concerns—drivers' scanning friction isn't addressed.

*2.4 Missing Information (Adequate):* Lists: parent needs, capacity data by time, whether issue was adoption/technology/reliability. These are reasonable but somewhat generic. Missing more actionable items like per-route occupancy, GPS pilot failure root cause.

**Evidence:** "This might lead to a reduction in usage of resources and more efficient operation."

---

### **S3. Finding Patterns**
**Traits:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

**Score: 3 — Strong**

**Rationale:**

*3.1-3.2 Pattern (Strong):* Correctly identifies "peak time crowd management" and abstracts to: "The demand rises above available resources during peak hours...When this happens, the resource is overstretched and this causes degraded service." This is domain-independent language.

*3.3 Cafeteria (Strong):* Correctly applies pattern: "during breakfast, lunch, snacks and dinner times, crowd most likely surges." Proposes staggered entry with specific implementation ("500 students divided into 4-5 batches of 20 minutes each"). Shows quantitative thinking.

*3.4 Fest Pattern (Adequate):* Correctly identifies need for "living document that tracks the availability of stalls" shared between all heads. However, the pattern comparison is weak: states "This is a mix of lack of communication and a lack of resources" and "All the problems link back to lack of available resources compared to the need." This misses the key distinction—fest issue is *informational synchronization* (knowledge-based collision) not *temporal demand concentration*. The rubric specifically looks for distinguishing these two patterns.

**Evidence:** "Ideally in this situation they should have kept a living document that tracks the availability of stalls and that should have been shared between all three heads."

---

### **S4. Diagnostic Reasoning**
**Traits:** Diagnostic Reasoning

**Score: 2 — Adequate**

**Rationale:**

*4.1 Hypotheses (Adequate):* Lists 4 hypotheses:
1. Conversion of time (format issue)
2. System clock slow/inconsistent due to load
3. The check might be failing
4. Speaker might be faulty

These are adequate but don't span diverse categories. Missing: phone sleep mode, battery saver throttling, app interruptions, UI lag vs actual timer, race conditions. The hypotheses stay narrowly in "code logic" space.

*4.2 Tests (Adequate):* Proposes:
1. Test cases for time conversion
2. Check if iteration is faster/slower
3. Check with another speaker

Tests are vague—"check the usage" is incomplete. Doesn't clearly isolate single variables.

*4.3 Root Cause (Weak):* Jumps to a specific solution ("Implementing threading and making it thread safe") rather than describing a general process for isolating root causes. Should describe: testing each variable independently, confirming with repeated trials, changing one variable at a time.

**Evidence:** "There might be a case where due to inconsistent/very frequent checking, the main thread is blocked"—this shows coding knowledge but also reveals tendency to jump to solutions rather than systematically isolate.

---

### **S5. Prioritization & Change Governance**
**Traits:** Prioritization Under Constraints (5.1–5.4), Change Governance Mindset (5.5)

**Score: 2 — Adequate**

**Prioritization (5.1-5.4): Adequate**

*5.1 Feasibility (Adequate):* Correctly identifies text/fast responses as achievable, voice as difficult. However, makes unrealistic assumption: "Two members are skilled in frontend dev, one is backend and one is an AI/agent dev"—the prompt says "All team members are beginners."

*5.2 Features (Weak):* Top 3 features listed are: conversational chatbot, link to source truth, ability to save chats. "Ability to upload images" is crossed out but still shows scope creep thinking. "Link to source truth" and "save chats" are nice-to-haves, not MVP-critical. Missing the core prioritization of: just answer questions first.

*5.3 Plan (Adequate):* Has structure but is over-engineered: mentions "vector DB," "RAG database," "stress testing and penetration testing"—unrealistic for beginners in 4 weeks. Doesn't adequately account for exam week (only 3 days allocated).

*5.4 Backup (Adequate):* "Narrow the scope further...release of the conversational platform and features of links and chat storage would be pushed to a further later phase." This is reasonable but vague.

**Change Governance (5.5): Adequate**

*5.5a (Adequate):* Chooses option (ii) "show answers quickly but let students flag wrong answers"—this is not the recommended choice. Reasoning mentions building "database of wrong answers" and "RLHF data" which is interesting but misses the core trade-off: students get wrong info first.

*5.5b (Adequate):* Answer is thin: "we would need the information of why the student thinks the information given by the bot is wrong." Doesn't specify what data must be recorded proactively (timestamp, question asked, confidence score, session ID).

*5.5c (Strong):* Addresses all three requirements:
- (i) "Correct the data and update the RAG database so the wrong answer stops"
- (ii) "find where the question was asked according to the session id and send callback notifications"
- (iii) "implement a generator validator agent...checks with VERIFIED EXTERNAL SOURCES"

This shows some governance thinking but the prevention mechanism is over-engineered.

**Evidence:** "we can send callback notifications to all affected session ids"—shows understanding of identifying affected users.

---

### **S6. Rapid Domain Learning**
**Traits:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

**Score: 2 — Adequate**

**Rationale:**

*6.1 Explanation (Adequate):* Uses car service station example: "If we keep track of the cars that enter the station from when it was empty and track the cars leaving the station, we can accurately tell the number of cars in the service station." This is an okay analogy but it's essentially a counting example (in/out), not capturing the full richness of event sourcing (history, point-in-time queries, audit trail, undo capability).

*6.2 Applications (Adequate):* Both examples (parking garage, logistics warehouse) are counting/inventory scenarios—similar to the bank example in structure. Not demonstrating transfer to truly novel domains. Missing the insight about "what was state at time X" or "how did we get here" that distinguishes event sourcing.

*6.3 Unclear Parts (Weak):* "The idea is clear, No questions." This is a red flag—genuine engagement would identify real questions like: how to handle long histories, what if events are recorded incorrectly, how to query efficiently. Claiming full understanding suggests superficial grasp.

*6.4 Catering Application (Adequate):* Shows table structure with events (order, change, payment). Correctly links "Cook Informed" column to track communication. However, concludes "This would not help with mixed up lists"—which is incorrect. Event sourcing would absolutely help because each shopping list would be traced to its source order events.

**Evidence:** "This would not help with mixed up lists"—reveals incomplete understanding of traceability benefits.

---

### **S7. Reflection**
**Traits:** Reflective Thinking

**Score: 2 — Adequate**

**Rationale:**

*7.1 Easiest (Adequate):* "pattern finding section was the easiest. It was my prior experience with real world problems that helped me spot pattern." This is experience-based ("prior experience") not cognition-based. Doesn't articulate what about their thinking process made it easier.

*7.2 Hardest (Adequate):* "Section 4 felt the hardest because without the code in front of me, it is hard to hypothesize a coding issue." Reasonable but surface-level—just says it was hard because no code, not what specifically about their thinking struggled.

*7.3 Process (Adequate):* "Any process involves getting information from a client...Process information & act on it → deliver results → Repeat." This is a generic framework, not a specific articulation of their method for Section 1. Doesn't describe: how they identified entities, how they traced relationships, what they looked for.

*7.4 Improvement (Weak):* "The only thing I would change is code a simple timer, actually write code and then debug it." This only addresses Section 4 and is about changing the test format, not their approach. Missing: connections between sections, how to allocate time, what to focus on.

**Evidence:** "Once you spot this process, it is easy to analyze any business"—shows confidence but not specific cognitive insight.

---

### **Global. Clear Articulation**
**Traits:** Clear Articulation (applied across entire test)

**Score: 3 — Strong**

**Rationale:**

*Structure (Strong):* Answers are organized with numbered/lettered sub-points. Uses headers, tables (Section 6.4), and clear delineation between sections.

*Clarity (Strong):* Ideas are expressed clearly. The bus redistribution solution in 2.2 is well-articulated. Technical concepts explained accessibly.

*Detail Level (Adequate):* Some answers are appropriately detailed (Section 2 solution), others are too brief (Section 4 tests, Section 7 reflections).

*Examples (Strong):* Uses concrete examples (car service station, parking garage, staggered lunch batches).

*Minor Issues:* Some answers trail off (text cut off in transcription), occasional redundancy, and the page-by-page format causes some fragmentation.

**Evidence:** The bus solution is well-structured: problem statement → assumption → solutions → prioritization → success metrics.

---

## **Strengths**

1. **Strong synthesis ability in Section 2:** Correctly reframes the budget/bus contradiction as a distribution problem and proposes practical redistribution solution
2. **Good structural thinking in Section 1:** Identifies many entities and events with reasonable sequencing; understands handoffs between actors
3. **Practical solution orientation:** Proposes implementable solutions (driver-phone GPS, staggered batches) rather than theoretical ideals
4. **Clear written communication:** Well-organized responses with appropriate use of structure, though some trailing off
5. **Some governance awareness in 5.5c:** Addresses affected user identification and prevention mechanisms

**Exceptional Candidate Markers (if applicable):**
- S1 score of 4: No (scored 3)
- Connections between sections: Partial (6.4 attempts to connect to S1 but incomplete)
- Spontaneous governance thinking before S5.5: No

---

## **Concerns / Weaknesses**

1. **Weak diagnostic reasoning (S4):** Limited hypothesis diversity, jumps to solutions rather than systematic isolation process
2. **Shallow domain learning (S6):** Claims full understanding with "no questions," misses key event sourcing benefits for traceability
3. **Over-engineering tendency:** Proposes RAG databases, vector DBs, stress testing, penetration testing for a beginner team—unrealistic scope
4. **Pattern distinction gap (S3.4):** Fails to distinguish temporal demand concentration from informational synchronization patterns
5. **Surface-level reflection (S7):** Attributes success to "prior experience" rather than articulating cognitive process; improvement suggestion addresses test format, not approach

**Red Flags to Note:**
- "The idea is clear, No questions" in 6.3 suggests superficial engagement
- Assumes skilled team composition despite prompt stating "all beginners"
- "This would not help with mixed up lists" shows incomplete understanding of event sourcing benefits
- Chooses option (ii) in 5.5a without recognizing students receive wrong info first

---

## **Final Recommendation (AI Generated)**

**Adequate**

Ravi Krishna demonstrates solid foundational capabilities in structural thinking and information synthesis (S1-S3), with practical solution orientation. However, significant gaps exist in diagnostic reasoning, rapid domain learning, and reflective thinking. The tendency to over-engineer solutions and claim complete understanding without engaging deeply (S6) raises concerns about learning agility in an R&D context. The candidate meets minimum thresholds but would require strong face-to-face performance demonstrating deeper analytical rigor and intellectual humility to be considered for Foundry R&D.
