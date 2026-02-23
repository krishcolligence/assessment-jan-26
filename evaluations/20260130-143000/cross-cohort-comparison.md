# Cross-Cohort Candidate Comparison

**Objective:** Rank Ravi Krishna (ECE, Jan 2026) against top 3 performers from Nov 2025 cohort (Nandan, Shreecharan, Nikhil — all CS)

**Date:** 30/01/2026

---

## 1. Assessment Overview

| Attribute | Nov 2025 | Jan 2026 |
|-----------|----------|----------|
| Candidates | 9 (top 3 analyzed) | 1 |
| Max Score | 32 | 32 |
| Sections | 8 | 8 |
| S6 Concept | Bloom Filter | Event Sourcing |
| S5 Scope | Prioritization only | Prioritization + Governance |

---

## 2. Section-by-Section Comparison

### Legend
- **=** : Identical question
- **≈** : Near-identical (minor additions)
- **~** : Same trait, different content
- Ravi scores shown as Raw / (ECE-Adjusted)

| Sec | Topic | Comparability | Nandan | Shreecharan | Nikhil | Ravi |
|-----|-------|---------------|--------|-------------|--------|------|
| S1 | Structural Thinking | ~ | 3 | 4 | 3 | 3 / (3) |
| S2 | Bus System Synthesis | = | **4** | 3 | 3 | 3 / (3) |
| S3 | Pattern Recognition | ≈ | 3 | **4** | 3 | 3 / (3) |
| S4 | Timer Debugging | = | 3 | 3 | 3 | 2 / (**3**) |
| S5 | Prioritization (+Gov) | ≈ | **4** | 3 | 3 | 2 / (**3**) |
| S6 | Rapid Learning | ~ | **4** | 3 | 2 | 2 / (**3**) |
| S7 | Reflection | ≈ | 3 | 3 | 3 | 2 / (2) |
| S8 | Communication | = | **4** | 3 | 3 | 3 / (3) |
| | **TOTAL** | | **28** | **26** | **23** | **20 / (23)** |

---

## 3. Identical-Section Analysis (Highest Confidence)

**Sections with identical questions:** S2 (Bus System), S4 (Timer), S8 (Communication)

| Candidate | S2 | S4 | S8 | Sum/12 |
|-----------|----|----|----|----|
| Nandan | 4 | 3 | 4 | **11** |
| Shreecharan | 3 | 3 | 3 | **9** |
| Nikhil | 3 | 3 | 3 | **9** |
| Ravi (Raw) | 3 | 2 | 3 | **8** |
| Ravi (ECE-Adj) | 3 | 3 | 3 | **9** |

**Interpretation:** On identical questions, ECE-adjusted Ravi matches Shreecharan and Nikhil.

---

## 4. Trait-by-Trait Deep Comparison

### 4.1 Information Synthesis (S2) — Identical Question

All four candidates tackled the same bus system problem.

| Candidate | Key Insight | Score |
|-----------|-------------|-------|
| **Nandan** | Budget-neutral reallocation (morning→evening), mentions Dijkstra's algorithm for routing | 4 |
| **Shreecharan** | Redistribution insight, combine routes to cover more students | 3 |
| **Nikhil** | Case-based approach, RFID for scanning efficiency | 3 |
| **Ravi** | Redistribution insight, driver-phone GPS solution, phased implementation | 3 |

**Assessment:** Ravi's answer is on par with Shreecharan and Nikhil. He shows the same reframing insight (distribution not quantity) and adds practical implementation thinking (driver phones as GPS). Nandan edges ahead with technical depth (Dijkstra mention) and exceptional synthesis.

---

### 4.2 Diagnostic Reasoning (S4) — Identical Question

Same timer app debugging scenario.

| Candidate | # Hypotheses | Test Quality | Score |
|-----------|--------------|--------------|-------|
| **Nandan** | 4 (input, system timer, trigger, parsing) | Clear isolation tests | 3 |
| **Shreecharan** | 5 (cache, code, modules, compiler, packages) | Reasonable tests | 3 |
| **Nikhil** | 4 (time function, latency, counter, exception) | Reasonable tests | 3 |
| **Ravi** | 4 (conversion, clock, check, speaker) | Vague tests, jumps to solution | 2 |

**Assessment:** Ravi's hypotheses include hardware thinking (speaker, clock) which reflects ECE training. His diagnostic *method* shows systems thinking but lacks software debugging vocabulary. ECE-adjusted score of 3 is appropriate — he demonstrates the approach but lacks domain-specific hypothesis space.

---

### 4.3 Pattern Recognition (S3) — Near-Identical

Jan 2026 adds question 3.4 (fest coordination pattern).

| Candidate | Pattern Abstraction | Cafeteria Application | 3.4 (if applicable) | Score |
|-----------|--------------------|-----------------------|---------------------|-------|
| **Nandan** | "Congestion" — clear | Practical (add seats) | N/A | 3 |
| **Shreecharan** | "High demand at certain time" | Two-perspective solution | N/A | 4 |
| **Nikhil** | "Exceeds capacity → lagging" | Creative (stagger times) | N/A | 3 |
| **Ravi** | "Peak demand > resources" | Quantified batches (500/4-5) | Misses pattern distinction | 3 |

**Assessment:** Ravi's 3.1-3.3 performance matches Nandan and Nikhil. His quantified cafeteria solution (batches of 120, 20-min windows) shows engineering rigor. However, he struggled with 3.4 (failed to distinguish temporal vs. informational patterns). Nov 2025 candidates weren't tested on this. Score of 3 is fair — he'd likely have scored 4 without 3.4, but the harder question exposed a gap.

---

### 4.4 Prioritization (S5) — Jan 2026 Harder

Jan 2026 adds governance component (5.5a, 5.5b, 5.5c).

| Candidate | Feasibility | Plan Quality | Backup | Governance | Score |
|-----------|-------------|--------------|--------|------------|-------|
| **Nandan** | Excellent | Detailed (Docker, AWS) | Strong (scope cut) | N/A | 4 |
| **Shreecharan** | Reasonable | Structured but less detailed | Good (top 20 Qs) | N/A | 3 |
| **Nikhil** | Good | Time-allocated | Weak (overtime) | N/A | 3 |
| **Ravi** | Over-engineered | Detailed but unrealistic | Reasonable | Adequate (chose suboptimal option) | 2 |

**Assessment:** Ravi's score is penalized by:
1. Unrealistic assumptions (skilled team vs. stated beginners)
2. Over-engineering (RAG, vector DBs, pen testing)
3. Suboptimal governance choice (option ii vs. iii)

However, his governance section (5.5c) was strong — he addressed all three fix requirements. Nov candidates weren't tested on governance at all. If scored on 5.1-5.4 only, Ravi's would likely be a 3 (matching Nikhil). The governance addition created the gap.

---

### 4.5 Rapid Domain Learning (S6) — Different Concepts

| Candidate | Concept | Explanation | Examples | Unknowns | Experiment | Score |
|-----------|---------|-------------|----------|----------|------------|-------|
| **Nandan** | Bloom Filter | Clear, accurate | E-commerce, lost & found | Thoughtful (hashing types) | Company analysis | 4 |
| **Shreecharan** | Bloom Filter | Good (bag analogy) | Disease detection, spam, fraud | Honest (code-level) | Black/white balls (analogy, not test) | 3 |
| **Nikhil** | Bloom Filter | Confused ("Bloom Tree") | Cinema seats, DBs | Misunderstands efficiency | Dataset manipulation | 2 |
| **Ravi** | Event Sourcing | Adequate (car service) | Parking, warehouse | "No questions" (red flag) | N/A (applied to S1) | 2 |

**Assessment:** This is the weakest comparison — different concepts with different CS-proximity.

- Bloom Filter is algorithmic/technical (favors CS)
- Event Sourcing is architectural/conceptual (more accessible)

Ravi's "no questions" is concerning, similar to Nikhil's misunderstanding. Both scored 2, suggesting comparable learning velocity on unfamiliar concepts. ECE-adjusted score of 3 accounts for event sourcing being somewhat foreign to ECE curriculum.

---

### 4.6 Reflection (S7) — Similar Questions

| Candidate | Self-Insight Depth | Method Articulation | Improvement Specificity | Score |
|-----------|-------------------|---------------------|------------------------|-------|
| **Nandan** | Good (identifies pattern-finding strength) | Reasonable | Generic ("more critical") | 3 |
| **Shreecharan** | Good (multi-perspective approach) | Reasonable | Actionable (opposite approach) | 3 |
| **Nikhil** | Strong (knows he goes off-topic) | Reasonable | Specific (be more concise) | 3 |
| **Ravi** | Surface (prior experience) | Generic (client→process→deliver) | Weak (write actual code) | 2 |

**Assessment:** Ravi's reflection is genuinely weaker. He attributes success to "prior experience" rather than cognitive patterns. His improvement suggestion addresses test format, not personal approach. This gap is real and not ECE-related. All Nov candidates demonstrated better metacognitive awareness.

---

### 4.7 Communication (S8/Global) — Identical Trait

| Candidate | Structure | Clarity | Appropriate Detail | Score |
|-----------|-----------|---------|-------------------|-------|
| **Nandan** | Excellent (numbered, bulleted) | Very clear | Technical depth appropriate | 4 |
| **Shreecharan** | Good (headers, sub-bullets) | Clear | Good technical vocab | 3 |
| **Nikhil** | Good (bullets, cases) | Generally clear, verbose | Sometimes tangential | 3 |
| **Ravi** | Good (numbered, tables) | Clear | Some trailing off | 3 |

**Assessment:** Ravi's communication matches Shreecharan and Nikhil. His use of tables (S6.4) and structured lists shows organization. Some answers trail off (possibly due to handwriting/page limits). Solid 3.

---

## 5. Composite Rankings

### 5.1 Raw Score Ranking

| Rank | Candidate | Score | Band |
|------|-----------|-------|------|
| 1 | Nandan | 28 | Strong Hire |
| 2 | Shreecharan | 26 | Hire |
| 3 | Nikhil | 23 | Hire |
| 4 | **Ravi** | 20 | Adequate |

### 5.2 ECE-Adjusted Ranking

| Rank | Candidate | Score | Band |
|------|-----------|-------|------|
| 1 | Nandan | 28 | Strong Hire |
| 2 | Shreecharan | 26 | Hire |
| 3 | **Ravi** | 23 | Strong Adequate / Borderline Hire |
| 3= | Nikhil | 23 | Hire |

### 5.3 Identical-Section-Only Ranking (S2+S4+S8)

| Rank | Candidate | Score/12 |
|------|-----------|----------|
| 1 | Nandan | 11 |
| 2= | Shreecharan | 9 |
| 2= | Nikhil | 9 |
| 2= | **Ravi (ECE-Adj)** | 9 |
| 5 | Ravi (Raw) | 8 |

---

## 6. Head-to-Head Comparisons

### Ravi vs. Nikhil (Closest Comparison)

| Dimension | Ravi | Nikhil | Edge |
|-----------|------|--------|------|
| S2 (Synthesis) | 3 | 3 | Tie |
| S3 (Patterns) | 3 | 3 | Tie |
| S4 (Debugging) | 2→3 | 3 | Nikhil (raw); Tie (adjusted) |
| S5 (Prioritization) | 2→3 | 3 | Nikhil (raw); Tie (adjusted) |
| S6 (Learning) | 2→3 | 2 | Tie (both had gaps) |
| S7 (Reflection) | 2 | 3 | **Nikhil** |
| S8 (Communication) | 3 | 3 | Tie |
| **ECE Factor** | +3 | — | Ravi benefits |

**Verdict:** Ravi and Nikhil are **closely matched**. Nikhil has genuine edge in reflection/metacognition. Ravi has comparable synthesis and pattern skills. If ECE-adjusted, they're tied at 23. Key difference: Nikhil's gaps are in theoretical concepts (Bloom Filter); Ravi's are in software debugging vocabulary and metacognition.

### Ravi vs. Shreecharan

| Dimension | Ravi | Shreecharan | Edge |
|-----------|------|-------------|------|
| S1 (Structure) | 3 | 4 | **Shreecharan** |
| S2 (Synthesis) | 3 | 3 | Tie |
| S3 (Patterns) | 3 | 4 | **Shreecharan** |
| S4 (Debugging) | 2→3 | 3 | Shreecharan (raw); Tie (adjusted) |
| S5 (Prioritization) | 2→3 | 3 | Shreecharan (raw); Tie (adjusted) |
| S6 (Learning) | 2→3 | 3 | Shreecharan (slight edge) |
| S7 (Reflection) | 2 | 3 | **Shreecharan** |
| S8 (Communication) | 3 | 3 | Tie |

**Verdict:** Shreecharan is clearly ahead. He excels in structural thinking and pattern recognition — two foundational R&D traits. Even with ECE adjustment, Ravi trails by 3 points.

### Ravi vs. Nandan

| Dimension | Ravi | Nandan | Edge |
|-----------|------|--------|------|
| S2 (Synthesis) | 3 | 4 | **Nandan** |
| S3 (Patterns) | 3 | 3 | Tie |
| S4 (Debugging) | 2→3 | 3 | Nandan (raw); Tie (adjusted) |
| S5 (Prioritization) | 2→3 | 4 | **Nandan** |
| S6 (Learning) | 2→3 | 4 | **Nandan** |
| S7 (Reflection) | 2 | 3 | **Nandan** |
| S8 (Communication) | 3 | 4 | **Nandan** |

**Verdict:** Nandan is in a different tier. He has exceptional synthesis, technical depth, and communication. The gap (5 points even after ECE adjustment) reflects genuine capability difference, not just domain exposure.

---

## 7. Final Ranking

| Rank | Candidate | Raw Score | Adjusted Score | Band | Confidence |
|------|-----------|-----------|----------------|------|------------|
| 1 | **Nandan** | 28 | 28 | Strong Hire | High |
| 2 | **Shreecharan** | 26 | 26 | Hire | High |
| 3 | **Nikhil** | 23 | 23 | Hire | High |
| 4 | **Ravi Krishna** | 20 | 23 | Hire (with ECE adjustment) | Medium |

### Confidence Notes
- **High** = Same assessment, straightforward scoring
- **Medium** = Cross-assessment comparison with justified adjustments

---

## 8. Qualitative Summary

### Where Ravi is Competitive
1. **Information Synthesis (S2):** Same reframing insight as top performers; adds practical implementation thinking
2. **Pattern Recognition (S3 core):** Matches Nandan/Nikhil on 3.1-3.3; quantified approach shows engineering rigor
3. **Communication:** Clear, structured responses; effective use of tables and lists
4. **Practical Orientation:** Driver-phone GPS, staggered batches — shows implementer mindset

### Where Ravi Trails
1. **Reflection/Metacognition:** Genuine gap — all three Nov candidates showed better self-awareness
2. **Theoretical Depth:** Less comfort with abstract CS concepts (though ECE background explains this)
3. **Software Debugging Vocabulary:** Limited hypothesis space due to curriculum differences
4. **Pattern Distinction (3.4):** Missed temporal vs. informational pattern difference

### Genuine Gaps vs. Exposure Gaps

| Gap Type | Evidence | Trainable? |
|----------|----------|------------|
| **Exposure** | S4 (debugging), S6 (event sourcing) | Yes — needs domain ramp-up |
| **Genuine** | S7 (reflection), S5.5a (governance choice) | Slower — requires coaching |

---

## 9. Hiring Recommendation

**If all 4 candidates were in the same cohort:**

| Candidate | Recommendation | Priority |
|-----------|----------------|----------|
| Nandan | **Strong Hire** — Ready for R&D with minimal ramp-up | 1 |
| Shreecharan | **Hire** — Strong analytical skills, standard onboarding | 2 |
| Nikhil | **Hire** — Consistent performer, guide on theoretical concepts | 3 |
| Ravi Krishna | **Hire (Conditional)** — Strong potential, needs domain ramp-up | 4 |

### Ravi-Specific Recommendation

**Hire with Investment** — Ravi's ECE-adjusted score of 23 places him at the Hire threshold, competitive with Nikhil. His gaps are primarily *exposure-based* (software debugging, CS concepts) rather than *capability-based*. The concerning area is metacognition/reflection, which needs coaching.

**Ideal for:** Roles involving systems thinking, hardware-software integration, or where diverse engineering perspectives add value.

**Onboarding needs:**
- Software debugging methodology training
- Exposure to architectural patterns (event sourcing, etc.)
- Coaching on reflective practice

**Risk:** If role requires immediate software debugging proficiency, Ravi may need 3-6 months ramp-up that other candidates wouldn't.

---

## 10. Summary Table

| Metric | Nandan | Shreecharan | Nikhil | Ravi (Adj) |
|--------|--------|-------------|--------|------------|
| Total Score | 28 | 26 | 23 | 23 |
| Band | Strong Hire | Hire | Hire | Hire* |
| Strongest Section | S2, S5, S6 (all 4s) | S1, S3 (both 4s) | Consistent 3s | S1, S2, S3 (all 3s) |
| Weakest Section | None below 3 | None below 3 | S6 (2) | S7 (2) |
| Key Strength | Technical depth + synthesis | Structural thinking | Practical consistency | Synthesis + practical solutions |
| Key Concern | Minor (diag. plan granularity) | Project planning detail | Theoretical gaps | Metacognition + domain exposure |
| Background | CS | CS | CS | ECE |

*With ECE adjustment applied

---

## Appendix: Adjustment Justification

The 3-point ECE adjustment (+15%) applied to Ravi's score reflects:

1. **S4 (+1):** Software debugging is not in ECE curriculum; his method was sound despite limited vocabulary
2. **S5 (+1):** Over-engineering reflects learning AI/software without calibration; governance wasn't tested for Nov candidates
3. **S6 (+1):** Event sourcing is architecturally foreign to ECE; his grasp was reasonable given starting distance

**Not adjusted:**
- S7 (Reflection): Metacognition is domain-agnostic; his weakness is genuine
- S1, S2, S3, S8: Domain-neutral sections; his scores are fair

This adjustment normalizes for *curriculum exposure* while preserving signal about *reasoning capability*.
