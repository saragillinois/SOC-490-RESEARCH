# AI Coding Assistant for SOC 490 Research

## Project Purpose

This AI coding assistant supports content analysis of sociology journal articles (1990-2026) to document how the discipline deploys theoretically loaded terms and vocabularies. The project maps variation across journal venues, subfields, and time periods, producing empirical evidence that institutionally-exportable vocabulary came from a specific subset of sociological production.

**Target Dataset**: ~840 abstracts across 6 journals, 7 time periods (1990-1994 through 2020-2024)

---

## What This Tool Does

The coding assistant:
1. **Receives** article titles and abstracts
2. **Analyzes** for Layer 1 (named target concepts) and Layer 2 (post-cascade redefinitions)
3. **Evaluates** identity deployment (descriptive vs. structural)
4. **Produces** first-pass codes with visible reasoning
5. **Flags** ambiguities and edge cases
6. **Connects** findings to manuscript frameworks (POG, Edgar)
7. **Outputs** codes in spreadsheet-ready format

The tool is a **methodological assistant**, not an authoritative judge. Your human judgment, especially informed disagreement, is where analytical value is created.

---

## Core Concepts

### Layer 1: Named Target Concepts
Explicit, recognizable theoretical terms from recent sociology:
- Colorblind racism
- Structural racism / systemic racism
- Privilege
- Microaggressions
- Intersectionality
- Heteronormativity / cisnormativity
- Implicit bias / unconscious bias

### Layer 2: Post-Cascade Redefinitions of Foundational Vocabulary
Terms redefined to operate outside agent-act-victim specification:
- **Harm**: Structural-experiential rather than agent-act-victim
- **Violence**: Extended senses (legal, structural, symbolic, epistemic, slow)
- **Power**: Group-level structural position, not exercised agency
- **Trauma**: Cultural, collective, structural trauma
- **Oppression**: Structural oppression
- **Domination**: Structural-position term
- **Marginalization**: Structural subordination
- **Gender vocabulary**: Cisgender, non-binary, gender identity, AGAB
- **Disparities/Inequalities**: Framed as automatically problematic

### Identity-Centering Axis
- **Descriptive**: Identity as demographic variable
- **Structural**: Identity as position producing analytical findings
- **Mixed**: Both deployments present

---

## How to Use This Tool

### Basic Workflow

1. **Gather Information**
   - Article title, journal, year, volume, issue
   - Author(s) and institutional affiliation
   - Complete abstract text
   - Sampling classification (random/citation-weighted/anchor)
   - Google Scholar citation count

2. **Feed into Tool**
   ```
   Paste title and abstract into the project chat
   ```

3. **Review First-Pass Codes**
   - Structured codes for each category
   - Visible reasoning explaining each code
   - Text evidence (quotes from abstract)
   - Flagged ambiguities
   - Manuscript connections

4. **Make Final Coding Decisions**
   - Agree with codes: Accept them
   - Disagree: Push back with your reasoning; conversation continues
   - Unclear: Ask tool to reconsider or flag for additional context

5. **Transfer to Spreadsheet**
   - Tool outputs codes in exact column order for master spreadsheet
   - Copy standardized output directly into sheet
   - Preserve tool reasoning in conversation history

### Key Principles

- **Don't force codes**: Flag ambiguity instead
- **Push back on the tool**: Your disagreement is analytical data
- **Keep reasoning visible**: Auditable records create reliable datasets
- **Preserve conversation history**: This is how patterns emerge for codebook refinement

---

## Documentation Files

### In this directory
- **system_prompt.md** — Core instructions governing the tool's analytical approach
- **METHODOLOGY_MEMO.md** — How to use the tool, key coding principles, workflow
- **TEST_CASE_CALIBRATION_GUIDE.md** — Eight reference cases representing different coding patterns
- **coding_template.md** — Coding output template and spreadsheet transfer format

---

## Understanding Test Cases

Eight calibration cases represent different vocabulary deployment patterns:

| Test Case | Title | Journal | Pattern | Key Insight |
|-----------|-------|---------|---------|------------|
| 1 | Living with Ghosts | ASR | FOUNDATIONAL | Vocabulary IS the analysis |
| 2 | Kinship Interlocks | ASR | ANALYTICAL | Vocabulary layered on empirical work |
| 3 | Collateral Decision-Making | ASR | WRAPPING | Empirical finding + vocabulary frame |
| 4 | Expanding Free Secondary Education | AJS | TRADITIONAL | Rigorous work without post-cascade vocabulary |
| 5 | Soft Regulatory Capture | AJS | TRADITIONAL | Named, attributed concepts as options |
| 6 | Legal Status Categories | Social Problems | FRAMEWORK | Vocabulary structures the question |
| 7 | Transgender and Non-Binary Workers | Social Problems | QUANTITATIVE+WRAPPING | Rigorous methods + vocabulary framing |
| 8 | Exclusionary Zoning | Demography | ALTERNATIVE TRADITION | Theoretical but different tradition |

These serve as ongoing reference points for pattern recognition and calibration.

---

## Coding Quick Reference

### Layer 1 Decision Tree
```
Do I see explicitly named theoretical terms from the list?
├─ YES → Code as PRESENT
├─ NO → Code as ABSENT
└─ UNCLEAR → Code as UNCLEAR and flag
```

### Layer 2 Decision Tree
```
Do I see redefined foundational terms (harm, violence, power, trauma, etc.)?
├─ YES → Identify which terms
│  ├─ How deployed? FOUNDATIONAL / ANALYTICAL / WRAPPING
│  └─ Code as PRESENT
├─ NO → Code as ABSENT
└─ UNCLEAR → Code as UNCLEAR and flag
```

### Identity Decision Tree
```
Are identity categories present?
├─ YES → Deployment mode?
│  ├─ Demographic variables → DESCRIPTIVE
│  ├─ Analytical positions → STRUCTURAL
│  ├─ Both → MIXED
│  └─ Record categories invoked
├─ NO → N/A
└─ UNCLEAR → Flag for human judgment
```

---

## Expected Output Format

When you code an abstract, you'll receive:

```
IDENTIFICATION
─────────────────────
[Basic bibliographic info]

LAYER 1: NAMED TARGET CONCEPTS
─────────────────────
[Each concept: PRESENT/ABSENT/UNCLEAR with reasoning]

LAYER 2: POST-CASCADE REDEFINITIONS
─────────────────────
[Each foundational term: PRESENT/ABSENT/UNCLEAR with deployment mode and reasoning]

IDENTITY-CENTERING AXIS
─────────────────────
[Categories present, deployment mode, how presented]

ANALYTICAL CONTEXT
─────────────────────
[Method type, subfield, journal type]

OBSERVATIONS & FLAGS
─────────────────────
[Manuscript connections, calibration patterns, ambiguities, overall observations]
```

All codes are then transferable directly to your master spreadsheet.

---

## Calibration & Improvement

### Weekly Calibration Checks
- Code 1-2 test cases independently
- Compare your codes to expected patterns
- If divergence: Consider whether coding criteria have shifted

### Week 4: Inter-Rater Reliability
- Code 25 articles independently (without tool)
- Compare to tool's codes on same articles
- Record discrepancies and patterns
- Use patterns to guide tool and codebook refinement

### Running Divergence Log
- Track cases where your final coding diverges from tool's first-pass
- Note category, reason for divergence, implication
- Patterns identify tool refinement needs and codebook ambiguities

---

## Important Reminders

1. **The tool surfaces, you judge** — AI generates first-pass codes; you apply analytical judgment.

2. **Ambiguity is data** — Difficult-to-code articles inform codebook refinement.

3. **Disagreement creates value** — When you diverge from the tool, that's analytical sophistication at work. Log it.

4. **Reasoning is auditable** — Visible reasoning means replicability, not just results.

5. **Iteration improves quality** — Tool and codebook improve through use. Divergence logs are the improvement mechanism.

---

## Support & Questions

When you're uncertain:
- Review METHODOLOGY_MEMO.md for coding principles
- Consult TEST_CASE_CALIBRATION_GUIDE.md for pattern examples
- Flag ambiguities clearly rather than forcing codes
- Push back on tool coding; conversation continues until you're confident

---

## Getting Started

1. Read this README for project overview
2. Review METHODOLOGY_MEMO.md for workflow and principles
3. Study TEST_CASE_CALIBRATION_GUIDE.md to understand coding patterns
4. Consult coding_template.md for output format
5. Begin coding: Paste abstract into tool, review codes, make final decisions

---

## Project Contact

For questions about coding logic, manuscript frameworks, or methodological decisions, consult system_prompt.md for the analytical framework governing all coding decisions.

Welcome to the project. The tool is your analytical partner—use it, disagree with it, and improve it through use.
