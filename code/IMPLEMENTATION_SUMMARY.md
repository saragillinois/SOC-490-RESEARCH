# Implementation Summary: AI Coding Assistant

**Date**: June 2, 2026  
**Repository**: saragillinois/SOC-490-RESEARCH  
**Branch**: `feature/ai-coding-assistant`

---

## Project Completed

An AI-powered coding assistant has been successfully built to support content analysis of sociology journal articles (1990-2026). The tool documents how the discipline deploys theoretically loaded terms across journals, subfields, and time periods.

---

## Deliverables Created

### 1. System Prompt (`system_prompt.md`)
The core analytical framework governing the tool's coding approach:
- **Framework Foundation**: Grounded in POG's four-category distinction and Edgar's vocabulary argument
- **Layer 1 Recognition**: Identifies 7 named target concepts (colorblind racism, microaggressions, intersectionality, etc.)
- **Layer 2 Recognition**: Identifies post-cascade redefinitions of foundational terms (harm, violence, power, trauma, oppression, domination, marginalization, gender vocabulary, disparities/inequalities)
- **Identity Analysis**: Distinguishes descriptive (demographic) vs. structural (position-producing) identity deployment
- **Deployment Modes**: Codes vocabulary as FOUNDATIONAL (is the analysis), ANALYTICAL (layered on empirical work), or WRAPPING (presentational)
- **Manuscript Connections**: Links coding to POG framework and Edgar vocabulary arguments
- **Calibration**: References 8 test cases for pattern recognition

**Key Principle**: The tool surfaces what's in abstracts and offers reasoning; human judgment applies analytical sophistication.

### 2. Methodological Memo (`METHODOLOGY_MEMO.md`)
Complete guidance for using the tool:
- **Workflow**: Step-by-step process from abstract input to spreadsheet transfer
- **Core Concepts**: Detailed explanation of Layer 1, Layer 2, and identity-centering axis
- **Coding Principles**: 
  - Layer 1 vs. Layer 2 distinction
  - Identity deployment (descriptive vs. structural)
  - Deployment modes for vocabulary
  - Ambiguity handling
  - Manuscript references
- **Role Clarification**: Tool as methodological assistant, not authoritative judge
- **Calibration Mechanisms**: Weekly checks against test cases, Week 4 inter-rater reliability, running divergence logs
- **Guidance Questions**: Decision trees for Layer 1, Layer 2, and identity coding

### 3. Test Case Calibration Guide (`TEST_CASE_CALIBRATION_GUIDE.md`)
Eight reference cases representing different coding patterns:

**ASR Cases (American Sociological Review)** — Full Post-Cascade:
- **Test Case 1**: Living with Ghosts — **FOUNDATIONAL** (vocabulary IS the analysis)
- **Test Case 2**: Kinship Interlocks — **ANALYTICAL** (vocabulary layered on empirical work)
- **Test Case 3**: Collateral Decision-Making — **WRAPPING** (empirical finding + vocabulary frame)

**AJS Cases (American Journal of Sociology)** — Traditional Empirical:
- **Test Case 4**: Education & Genes — **TRADITIONAL** (rigorous work without post-cascade vocabulary)
- **Test Case 5**: Regulatory Capture — **TRADITIONAL** (named, attributed concepts as analytical options)

**Specialty Journals** — Different Patterns:
- **Test Case 6**: Legal Status Categories (Social Problems) — **FRAMEWORK STRUCTURES QUESTION**
- **Test Case 7**: Transgender Workers (Social Problems) — **QUANTITATIVE + VOCABULARY WRAPPING**
- **Test Case 8**: Exclusionary Zoning (Demography) — **ALTERNATIVE THEORETICAL TRADITION**

Each case includes analytical notes, expected coding, and calibration guidance.

### 4. Coding Template (`coding_template.md`)
Standardized coding output format:
- **Structured Output**: Organized sections matching coding categories
- **Spreadsheet Transfer**: Columns organized to match existing master dataset structure exactly
- **Categories Included**:
  - IDENTIFICATION (metadata)
  - LAYER 1 (7 named concepts)
  - LAYER 2 (9 foundational term redefinitions)
  - IDENTITY-CENTERING AXIS (deployment categories)
  - ANALYTICAL CONTEXT (method, subfield)
  - OBSERVATIONS & FLAGS (ambiguities, connections)
- **Inter-Rater Reliability Tracking**: Template for Week 4 calibration
- **Running Divergence Log**: Template for tracking tool/human divergence patterns

**Key Feature**: All output codes directly transfer to master spreadsheet using existing column organization.

### 5. Project README (`code/README.md`)
Quick-start documentation:
- **Project Overview**: Purpose, scope, target dataset
- **Core Concepts**: Layer 1, Layer 2, identity-centering axis
- **How to Use**: Basic workflow in 5 steps
- **Quick Reference**: Decision trees for Layer 1, Layer 2, identity coding
- **Calibration & Improvement**: Weekly checks, Week 4 reliability, divergence logging
- **Getting Started**: Onboarding sequence

---

## How The Tool Works

### Workflow

1. **Input**: Paste article title and abstract into Claude Project chat
2. **Analysis**: Tool applies codebook against abstract using system prompt framework
3. **Output**: 
   - Structured codes for each category
   - Visible reasoning explaining each code
   - Text evidence from abstract
   - Flagged ambiguities
   - Manuscript connections when relevant
4. **Review**: You review codes and make final decisions
5. **Feedback**: Push back on codes you disagree with; conversation continues
6. **Transfer**: Finalized codes copy directly to spreadsheet

### Key Features

- **Visible Reasoning**: Every code includes explanation of logic
- **Ambiguity Flagging**: Tool doesn't force uncertain codes
- **Manuscript Grounding**: References POG and Edgar frameworks when relevant
- **Test Case Calibration**: Refers to 8 reference patterns for consistency
- **Human-Centered**: Your judgment is the final analytical step; tool surfaces, you decide
- **Auditable**: Conversation history preserves all coding decisions and reasoning

---

## Integration with Your Research

### Spreadsheet Structure
The tool outputs codes in exact column order matching your existing organizational spreadsheet:

**IDENTIFICATION** (10 columns)
- Article ID, Journal, Year, Volume, Issue, Author(s), Affiliation, Title, Abstract, Sample stratum, Citation count

**LAYER 1** (7 columns)
- Colorblind racism, Structural racism, Privilege, Microaggressions, Intersectionality, Heteronormativity, Implicit bias

**LAYER 2** (9 columns)
- Harm (structural), Violence (extended), Power (structural), Trauma (structural), Oppression, Domination, Marginalization, Gender vocabulary, Disparities/inequalities

**IDENTITY** (4 columns)
- Group identity as primary analytical organization, Identity categories, Identity deployment, How identity presented

**ANALYTICAL CONTEXT** (3 columns)
- Method type, Primary subfield, Observations

### Calibration Integration

- **Test Cases**: Embedded reference material for ongoing pattern recognition
- **Inter-Rater Reliability**: Week 4 calibration tracking you perform independently, then compare to tool
- **Divergence Logging**: Running log of where your judgment differs from tool's first-pass codes
- **Codebook Refinement**: Patterns in divergence guide tool and codebook improvement

---

## Repository Structure

```
SOC-490-RESEARCH/
├── feature/ai-coding-assistant/              [Active branch]
│   └── code/
│       ├── system_prompt.md                  # Core analytical framework
│       ├── METHODOLOGY_MEMO.md               # How to use the tool
│       ├── TEST_CASE_CALIBRATION_GUIDE.md   # 8 reference patterns
│       ├── coding_template.md                # Output format & transfer
│       └── README.md                         # Quick start guide
```

All files are markdown-based for version control and collaboration.

---

## Getting Started

1. **Read**: `code/README.md` — Overview and quick reference
2. **Learn**: `code/METHODOLOGY_MEMO.md` — Detailed workflow and principles
3. **Study**: `code/TEST_CASE_CALIBRATION_GUIDE.md` — Understand the patterns
4. **Reference**: `code/coding_template.md` — Know what output looks like
5. **Use**: Begin pasting abstracts to the Claude Project for coding

---

## Important Notes

### For Users (You)

- The tool is a **methodological assistant**, not an authoritative judge
- Your human judgment, especially when informed by disagreement with the tool, is where analytical value is created
- **Flag ambiguity** rather than forcing codes
- **Push back** on codes you disagree with; conversation continues until you're confident
- **Log divergences** — When you diverge from the tool's first-pass coding, that's valuable data for improvement

### For Tool Calibration

- Use test cases weekly to check consistency
- Complete Week 4 inter-rater reliability exercise: code 25 articles independently, compare to tool codes
- Track divergences in the running log — patterns identify refinement needs
- Ambiguities and divergences aren't failures; they're data for codebook and tool improvement

### For Data Quality

- All reasoning is preserved in conversation history (not just codes)
- Auditable record means replicable methodology
- Conversation history becomes documentation of analytical choices
- Reasoning visibility enables others to understand and replicate your process

---

## Project Status

✅ **Complete**: System prompt, methodology memo, test case guide, coding template, README  
✅ **Ready for Use**: Tool is configured and documented  
✅ **Next Steps**: Begin coding abstracts, establish calibration schedule, start divergence logging

---

## Support & Refinement

As you use the tool:
- Flagged ambiguities accumulate → guides codebook refinement
- Divergences accumulate → guides tool prompt refinement
- Patterns emerge → improve reliability over time
- This is **iterative**. The tool and codebook improve through use.

For questions about specific coding decisions, refer to the documentation files. For methodological questions about the project's theoretical framework, consult the system prompt and methodology memo.

---

**Status**: Ready for implementation  
**Branch**: `feature/ai-coding-assistant` on saragillinois/SOC-490-RESEARCH
