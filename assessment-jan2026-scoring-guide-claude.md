# R&D Engineering Aptitude Test — Scoring Guide

## Scoring Overview

| Section | Primary Trait | Secondary Trait | Points |
|---------|---------------|-----------------|--------|
| S1 | Modeling from Narrative | Dependency & Ripple Reasoning | 4 |
| S2 | Modeling from Narrative | Prioritization | 4 |
| S3 | Pattern Recognition | Dependency & Ripple Reasoning | 4 |
| S4 | Diagnostic Reasoning | — | 4 |
| S5 | Prioritization Under Constraints | Change Governance Mindset | 4 |
| S6 | Rapid Domain Learning | Reflective Thinking | 4 |
| S7 | Reflective Thinking | — | 4 |
| Global | Clear Articulation | — | 4 |

**Total: 32 points**

**Scoring note:** All sections weighted equally. Time differences reflect task complexity, not importance.

---

# Section 1 — Understanding How Work Happens

**Traits tested:** Modeling from Narrative (primary), Dependency & Ripple Reasoning (secondary)

## Model Answer (Exceptional)

### 1.1 Things (Entities)

**Explicit:**
- Customer
- Order
- Event date
- Guest count
- Menu/food type
- Price estimate
- Diary/calendar
- Cook
- Shopping list
- Helper
- Driver
- Payment
- Payment book

**Implicit (strong candidates identify):**
- Availability (time slots)
- Menu items/dishes
- Ingredients
- Delivery address
- Order status
- Customer type (regular vs one-time)
- Credit/account balance

### 1.2 Events (Process Flow)

1. Customer calls with inquiry
2. Availability checked
3. Order details recorded
4. Price estimate given
5. Order confirmed
6. Menu planned by cook
7. Shopping list created
8. (Possible) Customer requests changes
9. Changes communicated to cook
10. Shopping list updated
11. Shopping done (day before)
12. Food prepared (event day)
13. Food delivered
14. Payment received
15. Payment recorded

### 1.3 Dependency Violation & Ripple Effects

**Dependency rule:**
"When guest count changes, cook must be informed before shopping list is finalized."

Or: "Order changes → Menu update → Shopping list update (in sequence)"

**Downstream effects (at least 3):**
- Shopping list quantities wrong
- Ingredient costs change
- Price estimate needs revision
- Preparation time may increase
- May need additional helpers
- Delivery vehicle capacity may be insufficient
- Payment amount changes

### 1.4 Shopping List Confusion

**Required information:**
- Order ID or customer name + event date
- Event date clearly marked
- Customer name
- Creation date
- Link to original order

**Required link:**
Each shopping list must reference its source order. One shopping list per order, clearly labeled.

---

## Scoring Rubric

### 4 — Exceptional

**1.1:** Identifies 10+ entities including implicit ones (availability, ingredients, order status). Shows structural thinking.

**1.2:** Lists 8+ events in correct sequence. Recognizes branching (payment types, changes).

**1.3:** States dependency precisely as a rule. Lists 4+ downstream effects spanning different actors (cook, helper, customer, driver).

**1.4:** Identifies traceability need. Proposes clear linking mechanism.

**Overall:** Sees the system, not just the story. Identifies what must exist for the system to work.

### 3 — Strong

**1.1:** Identifies 7-9 entities, mostly explicit. May miss some implicit ones.

**1.2:** Lists 6-7 events in roughly correct order.

**1.3:** States dependency correctly. Lists 2-3 downstream effects.

**1.4:** Identifies basic information needs. Linking concept present but not precise.

### 2 — Adequate

**1.1:** Lists 4-6 entities, only explicit ones.

**1.2:** Lists some events but sequence unclear or incomplete.

**1.3:** Understands something went wrong but can't articulate the rule. Lists 1-2 effects.

**1.4:** Vague answer about "better organization."

### 1 — Weak

**1.1:** Lists fewer than 4 items or lists actions instead of entities.

**1.2:** Cannot extract process flow.

**1.3:** No clear dependency articulation. No ripple effects identified.

**1.4:** No meaningful answer.

---

## Evaluator Notes

**What distinguishes exceptional from strong:**
- Exceptional candidates identify *implicit* entities (things that must exist but aren't named)
- Exceptional candidates see *system* — they ask "what must be true for this to work?"
- Exceptional candidates trace ripples through *multiple actors*

**Red flags:**
- Retelling the story instead of extracting structure
- Missing the guest count → cook → shopping list chain
- Treating the business as isolated transactions rather than connected flow

---

# Section 2 — Information Synthesis

**Traits tested:** Modeling from Narrative (primary), Prioritization (secondary)

## Model Answer (Exceptional)

### 2.1 Agreements & Disagreements

**Agreements:**
- Evenings are crowded (students: crowded; admin: 4× demand; drivers: implicit)
- Something needs improvement
- Delays occur

**Disagreements:**
- Students want more buses; Admin says buses underutilized (10% full)
- Students want GPS; Drivers say GPS didn't work
- Root cause differs: students blame quantity, drivers blame traffic/scanning

### 2.2 Handling Contradiction

More buses ≠ only solution. Reframe: problem is *distribution*, not *quantity*.

Solutions within budget:
- Redistribute existing buses (fewer morning, more evening)
- Optimize routes to reduce travel time
- Stagger schedules to reduce peak load
- Increase turnaround speed (faster boarding)

### 2.3 Balanced Solution

1. **Redistribute fleet:** Shift morning buses to evening peak
2. **Fix GPS properly:** Pilot failed due to device quality, not concept. Retry with better devices.
3. **Speed up boarding:** Reduce ID scanning friction (app-based, tap cards)
4. **Optimize routes:** Data-driven route planning to reduce traffic delays

### 2.4 Missing Information

- Per-route occupancy data (which routes full vs empty?)
- Actual vs scheduled arrival times
- Student origin-destination patterns
- GPS pilot failure root cause
- Current boarding time per student

---

## Scoring Rubric

### 4 — Exceptional

- Synthesizes across sources, doesn't just summarize
- Reframes contradiction creatively (distribution vs quantity)
- Solution addresses all three stakeholder concerns
- Missing information is actionable (would change recommendation)

### 3 — Strong

- Good synthesis
- Reasonable solution
- Some creative reframing

### 2 — Adequate

- Mostly restates information
- Solution favors one source over others
- Missing information is generic

### 1 — Weak

- No synthesis
- Superficial or impractical solution

---

# Section 3 — Finding Patterns

**Traits tested:** Pattern Recognition (primary), Dependency & Ripple Reasoning (secondary)

## Model Answer (Exceptional)

### 3.1 Pattern

Demand concentrates at specific times → resource overloaded during peaks.

### 3.2 General Description

"When many people need the same limited resource at the same time, the resource becomes overloaded even if average usage is low. Peak demand, not average demand, determines whether the system fails."

### 3.3 Cafeteria Application

**Why it happens:** Students have common break times. 40% average means peaks could be 80-100%. Demand isn't evenly distributed.

**Solution:** Stagger lunch times, add seating during peak, or speed up turnover.

### 3.4 Fest Coordination Problem

**Information gap:** Logistics Head's stall assignments weren't visible to Sponsorship Head. No shared record of commitments.

**Pattern comparison:**
- WiFi/gym/printer: *Demand concentration* (many users, same time)
- Fest stalls: *Information synchronization* (multiple actors, shared resource, no coordination)

Both are resource contention, but:
- First is *temporal* (time-based collision)
- Second is *informational* (knowledge-based collision)

Exceptional answer recognizes both patterns and articulates the difference.

---

## Scoring Rubric

### 4 — Exceptional

- Pattern abstracted cleanly (domain-independent language)
- Cafeteria application correct and insightful
- 3.4: Identifies *both* patterns and distinguishes them (temporal vs informational)

### 3 — Strong

- Pattern correct
- Application reasonable
- 3.4: Identifies information gap but may not articulate the pattern distinction

### 2 — Adequate

- Pattern partially correct (stays too concrete)
- Application vague
- 3.4: Superficial answer

### 1 — Weak

- Misses pattern
- Cannot transfer to new situation

---

# Section 4 — Diagnostic Reasoning

**Traits tested:** Diagnostic Reasoning

## Model Answer (Exceptional)

### 4.1 Hypotheses

1. Phone sleep mode pauses background timer
2. Timer code uses imprecise delay mechanism
3. System clock drifts
4. App interrupted by notifications/multitasking
5. CPU throttling in battery saver mode
6. Timer start/stop has race condition
7. Display update ≠ actual timer (UI lag)

### 4.2 Tests

1. **Sleep mode:** Keep screen on entire duration → check if accurate
2. **Code precision:** Log timestamps at start and end → compare to external clock
3. **Clock drift:** Run timer alongside physical stopwatch → compare
4. **Interruptions:** Run in airplane mode, no other apps → check if stable
5. **Battery saver:** Test with battery saver on vs off → compare
6. **Race condition:** Start multiple timers simultaneously → check consistency
7. **UI lag:** Add audio cue at exact timer end → compare audio to display

### 4.3 Root Cause Isolation

1. Run each test independently
2. Record which conditions change behavior
3. If multiple variables affect timing, test combinations
4. Confirm with repeated trials (rule out randomness)
5. Change one variable at a time to isolate

---

## Scoring Rubric

### 4 — Exceptional

- 5+ diverse hypotheses spanning different categories (hardware, software, environment)
- Tests isolate single variables
- Clear root cause narrowing strategy

### 3 — Strong

- 4 good hypotheses
- Tests mostly isolate variables

### 2 — Adequate

- 2-3 generic hypotheses
- Tests don't clearly discriminate

### 1 — Weak

- 1-2 obvious guesses
- No test design

---

# Section 5 — Prioritization & Change Governance

**Traits tested:** Prioritization Under Constraints (5.1-5.4), Change Governance Mindset (5.5)

## Model Answer (Exceptional)

### 5.1 Feasibility

**Realistic:**
- Text Q&A (core, achievable)
- Mobile (web works on mobile)
- Fast responses (simple lookup is fast)

**Difficult:**
- Voice input (requires speech-to-text, complex)
- 50 questions (may be too many to curate well)
- Quality answers (accuracy is hard)

### 5.2 Top 3 Features

1. **Text Q&A for top 20 questions** — Core value, achievable
2. **Mobile-friendly web interface** — Accessibility without app development
3. **Keyword search** — Lets users find answers without exact phrasing

*Not voice:* Adds complexity, can be added later.

### 5.3 4-Week Plan

- **Week 1:** Collect/curate top 20 questions, design simple matching logic
- **Week 2:** Build text interface + mobile UI
- **Week 3:** Light work (exams) — testing, bug fixes only
- **Week 4:** Final testing, deployment, buffer for issues

### 5.4 Backup Plan

- Cut scope to top 10 questions
- Drop any styling/polish
- Ship text-only MVP
- Add voice/more questions as v2

### 5.5 Change Governance

**(a) Approach choice:**

Option (iii) — confidence threshold — is best for v1.

Reasoning:
- Human review (i) doesn't scale and delays responses
- Flag wrong answers (ii) means students get wrong info first
- Confidence threshold (iii) prevents harm while being honest about limits

**(b) Tracing what went wrong:**

Need to record:
- Which question was asked (exact text)
- Which FAQ entry matched
- Confidence score
- Timestamp
- Student identifier (if available)
- Answer shown

Trace path: Student complaint → timestamp → logs → matched FAQ entry → root cause

**(c) Fix with three requirements:**

(i) **Immediate stop:** Update/remove incorrect FAQ entry. Takes effect immediately since answers are looked up in real-time.

(ii) **Identify affected students:** Query logs for all students who received answers from that FAQ entry in relevant time window.

(iii) **Prevent future errors:** Add review step for FAQ changes. Require source/verification for factual entries. Test new entries before deployment.

---

## Scoring Rubric

### 5.1-5.4: Prioritization (2 points)

**4:** Realistic assessment, clear rationale, practical plan, adaptable backup
**3:** Mostly realistic, reasonable plan
**2:** Overly optimistic, weak prioritization
**1:** No clear priorities

### 5.5: Change Governance (2 points)

**4:** Chooses approach with clear reasoning about trade-offs. Identifies specific data needed for tracing. Fix addresses all three requirements with concrete mechanisms.

**3:** Reasonable approach choice. Tracing answer present but incomplete. Fix addresses requirements but vaguely.

**2:** Approach chosen without trade-off reasoning. Vague tracing. Fix incomplete.

**1:** No meaningful answer to governance questions.

---

## Evaluator Notes for 5.5

**What distinguishes exceptional:**
- Spontaneously thinks about audit trail before being asked
- Recognizes that "fixing" has multiple dimensions (stop harm, identify affected, prevent recurrence)
- Thinks about what data must be recorded *proactively*

**Red flags:**
- Only thinks about happy path ("just fix the FAQ")
- No consideration of affected users
- No traceability thinking

---

# Section 6 — Rapid Domain Learning

**Traits tested:** Rapid Domain Learning (primary), Reflective Thinking (secondary)

## Model Answer (Exceptional)

### 6.1 Simple Explanation

"Instead of writing down where you are now, you write down every step you took to get there. If you want to know where you are, you retrace your steps from the beginning. If you want to know where you were yesterday, you retrace only up to yesterday.

Like a travel journal vs a 'current location' pin. The journal tells you everywhere you've been and how you got here. The pin only tells you where you are now."

### 6.2 Real-life Uses

1. **Medical records:** Store every diagnosis, prescription, test (events) rather than just "current health status." Allows seeing complete patient history, understanding how conditions developed, catching missed patterns.

2. **Inventory management:** Store every item received, sold, returned, damaged (events) rather than just "current stock = 50." Can trace where missing items went, audit discrepancies, understand seasonal patterns.

### 6.3 Unclear Parts

- How do you handle very long histories? (Performance)
- What if an event was recorded incorrectly?
- How do you query efficiently without replaying everything?
- How does this work with multiple related entities?

*Good answers acknowledge genuine gaps rather than claiming full understanding.*

### 6.4 Application to Catering Business

**Events to store:**
- Order created (customer, date, guests, menu)
- Guest count changed (old value → new value, timestamp, who requested)
- Menu item added/removed
- Shopping list generated (linked to order)
- Item purchased (linked to shopping list)
- Payment received (amount, method)
- Payment recorded

**How this helps:**

*Forgotten changes:* Every change is an event with timestamp. Can see complete order history. Can alert if "guest count changed" event exists but no "shopping list updated" event follows.

*Mixed-up lists:* Each shopping list is linked to order events. Can trace any item back to its source order. Impossible to have orphan lists.

---

## Scoring Rubric

### 4 — Exceptional

- Explanation uses novel, apt analogy (not just restating bank example)
- Applications are non-obvious and reasoning is clear
- Unclear parts show genuine engagement (not fake humility)
- Section 1 connection is specific and insightful

### 3 — Strong

- Good explanation
- Reasonable applications
- Some unclear parts identified
- Section 1 connection present but generic

### 2 — Adequate

- Paraphrases definition without true understanding
- Applications are superficial
- No real unclear parts identified
- Section 1 connection weak or missing

### 1 — Weak

- Cannot explain concept
- Wrong applications
- No connection made

---

# Section 7 — Reflection

**Traits tested:** Reflective Thinking

## Scoring Rubric

### 4 — Exceptional

**7.1-7.2:** Specific insight into own cognition. "I found Section 1 easier because I naturally look for structure when people describe processes — I was mentally drawing boxes and arrows."

**7.3:** Articulates a method, not just "I read it carefully." Example: "I first listed all the people mentioned, then asked what each person does, then looked for handoffs between them."

**7.4:** Concrete, actionable change. "I'd spend more time on Section 1 since my answers to 6.4 depended on understanding it well."

**Overall:** Demonstrates awareness of own thinking patterns, not just task difficulty.

### 3 — Strong

- Good reflection on easy/hard with reasonable "why"
- Some process articulation in 7.3
- Specific improvement suggestion

### 2 — Adequate

- Surface-level reflection ("Section X was hard because it had many parts")
- 7.3 is vague ("I just thought about it")
- Generic improvement ("manage time better")

### 1 — Weak

- No reasoning, just labels
- Cannot articulate process
- No meaningful improvement

---

## Anchor Examples

**Score 4:**
> "Section 3 was easiest because I naturally look for patterns — I often notice when different problems have the same underlying shape. Section 1 was harder; I kept wanting to describe *what happens* rather than *what things exist*. I had to consciously switch from narrative mode to structural mode. For 7.3: I first highlighted all nouns (potential entities), then looked for verbs connecting them (relationships), then asked 'what would break if this didn't exist?' Next time, I'd do Section 1 more slowly since Sections 5.5 and 6.4 built on it."

*Why 4: Specific cognitive insight ("narrative mode to structural mode"), articulates explicit method (nouns → verbs → breakage test), connects sections.*

**Score 3:**
> "Section 4 was easiest because I've debugged things before. Section 6 was hard because event sourcing was new. For 7.3: I tried to list all the things mentioned and figure out how they connect. Next time I'd read all questions first to see connections."

*Why 3: Honest, reasonable, but insights are experience-based ("I've debugged before") not cognition-based. Method is vague ("figure out how they connect").*

**Score 2:**
> "Section 3 was easy. Section 5 was hard because there was a lot to consider. For 7.3: I read it a few times and picked out the important parts. I would manage time better."

*Why 2: No "why" depth. No method. Generic improvement.*

**Score 1:**
> "Easy: Section 3. Hard: Section 1."

*Why 1: Labels only. No reflection.*

---

# Section 8 — Clear Articulation (Global)

**Applied across entire test, not standalone section.**

## Scoring Rubric

### 4 — Exceptional

- Answers are structured (headers, bullets, logical flow)
- Complex ideas explained simply
- Appropriate detail (not over/under-explained)
- Concrete examples used effectively

### 3 — Strong

- Mostly clear and organized
- Minor clarity issues

### 2 — Adequate

- Understandable but disorganized
- Some rambling or vagueness

### 1 — Weak

- Hard to follow
- Key points buried or missing

---

# Summary: Trait Coverage

| Trait | Primary Section | Secondary Section |
|-------|-----------------|-------------------|
| Modeling from Narrative | S1 | S2 |
| Dependency & Ripple Reasoning | S1 (1.3, 1.4) | S3 (3.4) |
| Diagnostic Reasoning | S4 | — |
| Prioritization Under Constraints | S5 (5.1-5.4) | S2 |
| Rapid Domain Learning | S6 | — |
| Pattern Recognition | S3 | — |
| Reflective Thinking | S7 | S6 (6.3, 6.4) |
| Change Governance Mindset | S5 (5.5) | — |
| Clear Articulation | Global | — |

---

# Score Interpretation

| Total Score | Interpretation |
|-------------|----------------|
| 28-32 | Exceptional — strong fit for Foundry R&D |
| 22-27 | Strong — likely good fit, verify gaps in F2F |
| 16-21 | Adequate — significant gaps, needs strong F2F performance |
| Below 16 | Weak — not recommended |

**Minimum thresholds:**
- Foundation traits (S1, S4): Must score 2+ on both
- Change Governance (S5.5): Must score 2+
- No section should score 1

**Exceptional candidate markers:**
- S1 score of 4 (strongest signal for Foundry fit)
- Connections between sections (6.4 references 1, 7.4 shows integration)
- Spontaneous governance thinking before 5.5
