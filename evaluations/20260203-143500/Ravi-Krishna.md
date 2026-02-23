# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Ravi Krishna
**Application ID / Email:** —
**Date of Evaluation:** 2026-02-03

---

## **Overall Score Summary**

| Section | Primary Trait | Secondary Trait | Score (1–4) |
| ------- | ------------- | --------------- | ----------- |
| S1. Understanding How Work Happens | Modeling from Narrative | Dependency & Ripple Reasoning | 3 |
| S2. Information Synthesis | Modeling from Narrative | Prioritization | 3 |
| S3. Finding Patterns | Pattern Recognition | Dependency & Ripple Reasoning | 3 |
| S4. Diagnostic Reasoning | Diagnostic Reasoning | — | 2 |
| S5. Prioritization & Change Governance | Prioritization Under Constraints | Change Governance Mindset | 3 |
| S6. Rapid Domain Learning | Rapid Domain Learning | Reflective Thinking | 3 |
| S7. Reflection | Reflective Thinking | — | 3 |
| Global. Communication | Clear Articulation | — | 3 |
| **Total Score** |  |  | **23/32** |

**Final Band:** 22–27 → *Strong — likely good fit, verify gaps in F2F*

**Minimum Thresholds:**
* Foundation traits (S1, S4): S1=3 ✓, S4=2 ✓
* Change Governance (S5.5): Addressed ✓
* No section scores 1 ✓

**AI-determined Band:** Strong

---

## **Section-wise Evaluation Notes**

### **S1. Understanding How Work Happens**
**Score: 3 (Strong)**

**Entities (1.1):** Candidate identifies ~12 items including explicit ones (diary, guests, date, cook, shopping list, driver, payment book) and some implicit ones (vehicle, containers, cutlery, invoice). Shows structural thinking by grouping related items: *"containers to put the cooked food. And the food in itself is an object, delivered with all the cutlery and an invoice."* However, misses key implicit entities like availability/status tracking.

**Events (1.2):** Lists ~10 events in correct sequence with good branching awareness: *"This, if it happens is another major event. When the customer changes requirements."* Includes customer call → noting → availability check → menu planning → changes → shopping → cooking → packing/QC → delivery → payment.

**Dependency (1.3):** States rule clearly: *"When a change comes in, the neighbour MUST inform the chef of this change."* Lists 4 downstream effects (food quantity, raw materials, cutlery/plates, delivery mode), but effects mostly focus on quantity changes rather than spanning multiple actors (cook, helper, driver, customer).

**Traceability (1.4):** Proposes Order No., Event date, Name + Ph. No. on ALL pages. Suggests confirmation call before shopping: *"a confirmation call MUST happen to ensure mix ups don't happen."* Good linking concept.

### **S2. Information Synthesis**
**Score: 3 (Strong)**

**Synthesis (2.1):** Identifies that all stakeholders agree GPS is needed, though synthesis of agreements/disagreements could be clearer. Correctly notes the contradiction between student demands and budget constraints.

**Contradiction Handling (2.2):** Creative reframing: *"10% is likely an average number which might reinforce the claim that evening crowd is high with buses running at 110% capacity."* Proposes redistribution: *"Reduction in number of buses in the morning... Apply those reduced buses to ply in the evening."*

**Solution (2.3):** Practical phased approach using driver phones for GPS instead of dedicated devices. Includes success metrics: *"Increased student satisfaction. Adoption of the App. Less than 1% error in location tracking."* Prioritizes location sharing as MVP.

**Missing Information (2.4):** Actionable items: parent data, morning/evening capacity data, adoption vs technology vs reliability issue.

### **S3. Finding Patterns**
**Score: 3 (Strong)**

**Pattern (3.1-3.2):** Identifies "peak time crowd management" and abstracts it: *"The service is fine and non-stressed during normal hours. The demand rises above available resources during peak hours and/or at specific times. When this happens, the resource is overstretched and this causes degraded service."*

**Application (3.3):** Correct application to cafeteria: *"Seats in a cafeteria can be considered as a resource... crowd most likely surges leading to stretching of the resource."* Proposes staggered entry with concrete detail: *"500 students divided into 4-5 batches of 20 minutes each."*

**Pattern Distinction (3.4):** Proposes living document for stall tracking but conflates patterns: *"This is a mix of lack of communication and a lack of resources. All the problems link back to lack of available resources compared to the need."* Does not distinguish temporal (WiFi/gym/printer) vs informational (fest stall coordination) patterns.

### **S4. Diagnostic Reasoning**
**Score: 2 (Adequate)**

**Hypotheses (4.1):** Shows good architectural thinking by first outlining system: *"[Input] -> [Convert HH:MM:SS to seconds] -> [Check every second for time] -> If Yes [Ring alarm]."* However, only 4 hypotheses: time conversion error, system clock slow due to load, check failing, speaker faulty. Limited diversity (mostly software-focused), missing hardware (battery saver) and environment (phone sleep mode, background interruptions) categories.

**Tests (4.2):** Proposes test cases for conversion function, checking iteration speed, isolated speaker test. Tests are reasonable but brief.

**Root Cause (4.3):** Jumps to a specific solution rather than describing isolation methodology: *"Implementing threading and making it thread safe should help."* This assumes the cause rather than describing how to isolate among multiple possibilities.

### **S5. Prioritization & Change Governance**
**Score: 3 (Strong)**

**Feasibility (5.1):** Correctly identifies achievable (50 questions, fast responses) vs unrealistic (voice—*"requires advanced TTS and STT systems which are not feasible for beginners"*).

**Priorities (5.2):** Clean UI, link to source truth, saved chats. Reasoning: *"These three features target: User experience, User trust, Customer satisfaction."* Interesting focus on trust, though "link to source" may not be MVP-critical.

**Plan (5.3):** Detailed 28-day plan with role assignments. Accommodates exam week. Shows project management thinking, though somewhat over-engineered for "all beginners" constraint.

**Backup (5.4):** *"Narrow the scope further. The main focus would fall to release of the conversational platform and features of links and chat storage would be pushed to a further later phase."* Practical.

**Change Governance (5.5):**
- **(a)** Chooses option (ii)—show answers quickly, let students flag: *"this also lets us build a database of wrong answers and also gives us verified human feedback data which is very valuable for Reinforcement learning."* Trade-off reasoning present, but this choice has risk (students get wrong info first). Option (iii) would be safer for v1.
- **(b)** Describes tracing via flagging: *"we would need the information of why the student thinks the information given by the bot is wrong."* Somewhat vague on proactive data recording.
- **(c)** Addresses all three requirements: *(i)* Correct data and update RAG database; *(ii)* Check session IDs, send callbacks; *(iii)* Implement generator-validator agent. Comprehensive.

### **S6. Rapid Domain Learning**
**Score: 3 (Strong)**

**Explanation (6.1):** Novel, apt analogy: *"Consider a car service station. If we keep track of the cars that enter the station from when it was empty and track the cars leaving the station, we can accurately tell the number of cars in the service station."*

**Applications (6.2):** Two good examples with reasoning:
- Parking garage: *"Installing sensors at each bay becomes expensive and complex. Instead if the history is captured... we can find the capacity available."* Cost-efficient + security audits.
- Logistics warehouse: *"If an item was signed in by an employee, it is added into the count... letting the manager know exactly it went out and who it was signed out by."*

**Unclear Parts (6.3):** *"The idea is clear, No questions."* This is a weakness—rubric notes good answers acknowledge genuine gaps rather than claiming full understanding.

**S1 Connection (6.4):** Shows table structure with events (intent, order, change, payment) and "Cook Informed" column. Honest acknowledgment: *"This would not help with mixed-up lists."* Connection present and shows critical thinking.

### **S7. Reflection**
**Score: 3 (Strong)**

**Easy (7.1):** *"Pattern finding section was the easiest. It was my prior experience with real world problems that helped me spot pattern."* Experience-based insight rather than cognition-based.

**Hard (7.2):** *"Section 4 felt the hardest because without the code in front of me, it is hard to hypothesize a coding issue."* Honest insight but attributes difficulty to external factor.

**Method (7.3):** Articulates explicit framework: *"Any process involves getting information from a client (or find a problem) -> Process information & act on it -> deliver results -> Repeat till satisfaction of customer. Once you spot this process, it is easy to analyze any business."* Good abstraction.

**Improvement (7.4):** *"The only thing I would change is code a simple timer, actually write code and then debug it."* Specific but misses that the test assesses reasoning without code.

### **Global. Clear Articulation**
**Score: 3 (Strong)**

- Well-structured with labeled sub-questions
- Uses examples effectively (car service station, parking garage, logistics warehouse)
- Explicitly states assumptions (*"Assumptions: Every driver has a GPS enabled phone..."*)
- Appropriate detail in most sections
- Minor rambling in S2/S3 but generally clear logical flow

---

## **Strengths**

* **Creative problem reframing:** Reframes bus contradiction as distribution problem, not quantity problem
* **Practical phased thinking:** Proposes MVP approach with later phases consistently (S2, S5)
* **Process framework:** Articulates explicit mental model for analyzing businesses (input → process → deliver → repeat)
* **Cross-section connection:** 6.4 explicitly references and applies learning to S1 catering problem
* **Trust-focused design:** Prioritizes user trust features (source links, transparency) in chatbot

**Exceptional Candidate Markers:**
- S1 score of 4: No (scored 3)
- Connections between sections: Yes — 6.4 references S1 explicitly
- Spontaneous governance thinking before S5.5: Not observed

---

## **Concerns / Weaknesses**

* **Diagnostic depth (S4):** Only 4 hypotheses, mostly software-focused; jumps to threading solution without describing isolation methodology
* **Overclaims understanding (S6.3):** "The idea is clear, No questions" suggests lack of intellectual humility
* **Risk tolerance in governance (S5.5a):** Chose riskier approach (ii) over safer approach (iii) without fully justifying trade-off
* **Pattern distinction (S3.4):** Conflates temporal resource contention with informational coordination failure
* **Cognition insight limited (S7):** Reflection is experience-based ("I've seen real world problems") rather than cognition-based ("I naturally think in X way")

**Red Flags to Note:**
- Retelling story instead of extracting structure (S1): No — showed structural thinking
- Only thinks about happy path in governance (S5.5): No — addressed all three fix requirements
- No traceability thinking: No — present in S1.4 and S5.5b/c
- Labels without reasoning in reflection (S7): No — provided reasoning

---

## **Final Recommendation (AI Generated)**

**Strong**

Ravi demonstrates solid modeling capability, creative problem reframing, and practical prioritization thinking. His explicit process framework (7.3) and cross-section integration (6.4→S1) suggest strong systems thinking potential. Main gaps are in diagnostic reasoning depth and pattern distinction at abstract level. Recommended for F2F to probe: (1) diagnostic methodology when facing multiple hypotheses, (2) intellectual humility around complex domains, (3) deeper pattern abstraction ability.
