Batch evaluate candidate answer sheets against R&D Engineering Aptitude Test.

## Reference Files (read first)
- `assessment-jan2026-scoring-guide-claude.md` — rubric, model answers, 1-4 ladder
- `candidate-evaluation-template.txt` — output template
- `assessment-jan2026-claude.md` — questions

## Input
- If $ARGUMENTS provided: evaluate specified files
- If no arguments: evaluate all `candidates/*` (md/txt)

## Evaluation Flow

**Phase 1: Section-wise batch scoring**
For each section (S1→S7): restate rubric criteria → read ALL candidates' responses → score (1-4) + rationale → rank candidates on section.

| Section | Primary Trait | Secondary Trait |
|---------|---------------|-----------------|
| S1 | Modeling from Narrative | Dependency & Ripple Reasoning |
| S2 | Modeling from Narrative | Prioritization |
| S3 | Pattern Recognition | Dependency & Ripple Reasoning |
| S4 | Diagnostic Reasoning | — |
| S5 | Prioritization Under Constraints (5.1–5.4) | Change Governance Mindset (5.5) |
| S6 | Rapid Domain Learning | Reflective Thinking |
| S7 | Reflective Thinking | — |

**Phase 2: Global (Clear Articulation)**
Holistic per-candidate assessment across full response: structure, clarity, appropriate detail, concrete examples.

**Phase 3: Cross-check**
Verify rationale↔score alignment per candidate. Adjust mismatches.

**Phase 4: Minimum threshold check**
- Foundation traits (S1, S4): Must score 2+ on both
- Change Governance (S5.5): Must score 2+
- No section should score 1

**Phase 5: Pairwise sanity**
Candidates within 2pts total: head-to-head confirmation of relative ordering.

## Output
Create timestamped folder: `evaluations/YYYYMMDD-HHMMSS/`

Contents:
1. `{candidate-name}.md` — individual evaluation report (filled template) per candidate
2. `summary.md` — ranking table: Name | Score/32 | Band | Key Strengths | Key Concerns

Bands: 28-32=Exceptional, 22-27=Strong, 16-21=Adequate, <16=Weak

## Constraints
- Scores 1-4 only, no half points
- S1 (Modeling from Narrative) ≠ S4 (Diagnostic Reasoning) — score independently
- Equal section weights (4pts × 8 = 32)
- Evidence-backed rationales (quote candidate text)

## Exceptional Candidate Markers
Flag candidates who demonstrate:
- S1 score of 4 (strongest signal for Foundry fit)
- Connections between sections (e.g., 6.4 references S1, 7.4 shows integration)
- Spontaneous governance thinking before S5.5
