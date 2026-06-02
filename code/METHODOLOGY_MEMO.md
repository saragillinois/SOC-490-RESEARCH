# Methodological Memo: Using the AI Coding Assistant

## Project Overview

This tool assists with content analysis of sociology journal articles (1990-2026) to document how the discipline's working vocabulary deploys theoretically loaded terms. The project maps variation across:
- **Journal venues**: Flagship (ASR, AJS) to specialty (Social Problems, Demography, etc.)
- **Subfields**: Race/ethnicity, gender, class, culture, methods, and others
- **Time periods**: Seven 5-year blocks from 1990-1994 to 2020-2024

The tool produces empirical evidence supporting the argument that institutionally-exportable vocabulary came from a specific subset of sociological production, not from sociology as a whole.

---

## How the Tool Works

### What You're Coding

**Layer 1: Named Target Concepts** — Explicit, recognizable theoretical terms
- Colorblind racism
- Structural racism / systemic racism
- Privilege
- Microaggressions
- Intersectionality
- Heteronormativity / cisnormativity
- Implicit bias / unconscious bias

**Layer 2: Direct Post-Cascade Redefinitions of Foundational Vocabulary** — Terms redefined to operate outside agent-act-victim specification
- **Harm**: Structural-experiential harm rather than agent-act-victim
- **Violence**: Extended senses (legal, structural, symbolic, epistemic, slow)
- **Power**: Group-level structural position rather than exercised agency
- **Trauma**: Cultural, collective, structural trauma
- **Oppression**: Structural oppression
- **Domination**: Structural-position term
- **Marginalization**: Structural subordination
- **Gender vocabulary**: Cisgender, non-binary, gender identity, AGAB — when treated as separable from sex
- **Disparities/Inequalities**: When framed as automatically problematic rather than as differences requiring analysis

**Identity-Centering Axis**
- How are identity categories present in the abstract?
- Deployment: Descriptive (demographic variable) vs. Structural (position producing analytical findings)
- Is group identity the primary analytical organization?

---

## Workflow

### Step 1: Prepare the Abstract
Gather these pieces of information:
- Article ID (auto-generated)
- Full citation (journal, year, volume, issue, author, affiliation)
- Complete abstract text
- Sampling classification (random / citation-weighted / anchor)
- Google Scholar citation count at time of coding

### Step 2: Feed into Tool
Paste title and abstract into the project chat.

### Step 3: Review First-Pass Codes
The tool produces:
- Structured codes for each category
- Visible reasoning explaining the codes
- Text evidence (quotes or excerpts)
- Flagged ambiguities requiring human judgment
- Connections to manuscript frameworks when relevant

### Step 4: Make Final Coding Decisions
Review each code and decide:
- **Agree**: Accept the coding
- **Disagree**: Push back with alternative judgment; the conversation continues
- **Unclear**: Ask the tool to reconsider or flag for additional context

When you disagree, explain your reasoning. The tool reconsiders its initial coding.

### Step 5: Transfer to Spreadsheet
Final codes go into the master analytical spreadsheet using the standardized column structure.

**Preserve the tool's reasoning in conversation history** — this creates an auditable record for:
- Replicability
- Calibration checking
- Identifying where codebook refinement is needed

---

## Key Coding Principles

### 1. Layer 1 vs. Layer 2: The Critical Distinction

**Layer 1 (Named Concepts)** are recognizable and attributable:
- "Colorblind racism" — can be cited to specific scholars
- "Microaggressions" — has a defined theoretical lineage
- "Intersectionality" — explicitly theorized and named
- These often appear as explicit analytical frameworks

**Layer 2 (Post-Cascade Redefinitions)** are vocabulary shifts:
- "Harm" moves from agent-act-victim ("X caused Y harm to Z") to structural-experiential ("the system causes harm")
- "Violence" extends beyond physical acts to legal, structural, symbolic, epistemic forms
- "Power" becomes group-level structural position rather than exercised agency
- "Disparities" treated as automatically indicating injustice rather than as differences requiring analysis

**The key insight**: Layer 2 vocabulary often appears as working analytical language *without being flagged as theoretically loaded*. You need to recognize when these redefined terms are carrying analytical weight in a way that reflects post-cascade vocabulary deployment.

### 2. Identity Deployment: Descriptive vs. Structural

**Descriptive Identity Deployment** (older, methodologically neutral):
- Identity variables mark populations being studied
- "We compared outcomes for men and women" — identity is demographic
- "We sampled from communities with different racial compositions" — identity marks subgroups
- Identity categories are essentially demographic controls

**Structural Identity Deployment** (post-cascade move):
- Identity operates as a position that produces the analytical findings
- Identity *framework* structures the question itself
- "How does being marked as X create systematic disadvantage?" — identity position generates findings
- Identity categories are analytically constitutive, not descriptive

### 3. Deployment Modes for Layer 2 Vocabulary

When Layer 2 vocabulary is present, code its mode:

**FOUNDATIONAL**: The redefined vocabulary *is* the analysis
- You couldn't remove it without losing the entire analytical contribution
- Example: "Living with Ghosts" — the analysis of how physical traces shape cultural trauma is impossible outside the redefined trauma vocabulary

**ANALYTICAL**: The article has a real empirical contribution, but layers post-cascade vocabulary on top
- The empirical finding could be stated without the vocabulary, but the framing adds a theoretical layer
- Example: "Kinship Interlocks" — the finding about wealth/status/power transmission is empirically solid, but "power" is deployed in post-cascade sense

**WRAPPING**: The empirical finding could stand entirely on its own, but is wrapped in redefined vocabulary anyway
- The vocabulary is presentational rather than analytical
- Example: "Collateral Decision-Making" — the pretrial detention finding is independent, but the article wraps it in post-cascade vocabulary

### 4. Handle Ambiguity Carefully

When you're uncertain:
- **Don't force a code**
- Flag the ambiguity explicitly
- Explain what makes it difficult
- Suggest what information would resolve it
- Let the human coder (you) make the final decision

The tool is here to surface what's in the abstract and offer reasoning. Your judgment, especially when informed by disagreement with the tool, is where analytical sophistication enters the process.

---

## When to Push Back on the Tool

Push back if:
1. **You see Layer 1 or Layer 2 vocabulary the tool missed** — Point out the passage and explain why you see it differently
2. **The reasoning doesn't match what you read** — Explain your understanding of the abstract
3. **Identity deployment seems misclassified** — Push back with your reading of how identity is used
4. **Ambiguity seems forced rather than flagged** — Ask the tool to flag the difficulty instead of choosing

When you push back, explain your reasoning. The tool will reconsider.

**Important**: When your judgment differs from the tool's initial coding, that's valuable data. Make a note of it in the running divergence log — these patterns help refine both the tool and the codebook.

---

## Calibration Against Test Cases

You have eight calibration cases that represent different coding patterns:

**ASR Cases (American Sociological Review) — Full Post-Cascade**
1. *Living with Ghosts*: Redefined vocabulary IS the analysis
2. *Kinship Interlocks*: Real empirical contribution + layered vocabulary
3. *Collateral Decision-Making*: Empirical finding wrapped in vocabulary

**AJS Cases (American Journal of Sociology) — Traditional Empirical**
4. *Does Expanding Free Secondary Education...*: Rigorous empirical work without redefined vocabulary
5. *Soft Regulatory Capture...*: Named, attributed concepts; presented as one analytical option

**Social Problems — Framework Structures Question**
6. *Legal Status Categories*: Fully operates within redefined vocabulary; framework structures the question

**Quantitative with Vocabulary Wrapping**
7. *Transgender and Non-Binary Workers*: Rigorous quantitative methods but wraps findings in redefined vocabulary

**Alternative Theoretical Tradition**
8. *Cumulative Exposure to Exclusionary Zoning*: Uses theoretically loaded terms but from different tradition (urban inequality, not race/gender/identity)

When you encounter an abstract, consider: Which test case does this most resemble? That classification helps calibrate your coding.

---

## Preservation of Tool Reasoning

Each coding session automatically preserves:
1. **Tool's first-pass codes** — Visible in conversation history
2. **Tool's reasoning** — Explains why each code was assigned
3. **Your feedback and pushback** — Your alternative judgments
4. **Final codes** — What you decided after review
5. **Divergences** — Where tool and human judgment differed

This creates an auditable record that serves:
- **Replicability**: Anyone can see how each code was determined
- **Calibration**: Patterns in human/tool divergence show where refinement is needed
- **Learning**: The tool can improve based on where its judgment diverged from human judgment

---

## Technical Transfer to Spreadsheet

Once you've finalized codes for an abstract:

1. The tool outputs codes in **exact column order** matching your master spreadsheet
2. You copy the standardized output directly into the spreadsheet
3. All codes are formatted for easy data entry
4. Tool's reasoning is preserved separately (in conversation history, not in spreadsheet)

The spreadsheet columns match the organization provided:
- **IDENTIFICATION**: Article metadata
- **LAYER 1**: Named target concepts (7 categories)
- **LAYER 2**: Post-cascade redefinitions (9 categories)
- **IDENTITY-CENTERING AXIS**: Identity deployment (4 columns)
- **ANALYTICAL CONTEXT**: Method, subfield, observations

---

## Inter-Rater Reliability: Week 4 Calibration

In Week 4, you'll code 25 articles independently (without tool assistance) and compare your codes to the tool's codes on the same articles.

For each article, record:
- Your coding
- Tool's coding
- Whether they match
- Reason for any divergence
- What that divergence implies

Patterns in divergence show:
- Where the tool needs refinement
- Where your judgment is doing important analytical work
- Where the codebook itself needs clarification

This becomes the basis for iterative tool improvement.

---

## Running Divergence Log: Why This Matters

As you code, keep a log of cases where your final coding diverges from the tool's first-pass coding. Format:

| Abstract ID | AI's Initial Code | Your Final Code | Category | Why AI Missed It | What This Reveals |
|-------------|-------------------|-----------------|----------|-----------------|-------------------|
| [ID] | [Code] | [Code] | Layer 1 / Layer 2 / Identity | [Reason] | [Implication for tool or codebook] |

This log shows:
- **Tool refinement needs**: Where the prompt or calibration needs adjustment
- **Codebook ambiguities**: Where the codebook itself is unclear
- **Your analytical sophistication**: Where human judgment does work that a tool can't yet match

---

## Important Reminders

1. **You're not looking for bad coding** — The tool's job is to surface what's in the text and offer reasoning. Your job is to apply analytical judgment.

2. **Ambiguity is data** — When something is difficult to code, that's valuable information. Flag it clearly so it contributes to codebook refinement.

3. **Conversation continues** — If you disagree with a code, push back. The back-and-forth is how you arrive at the coding that makes sense.

4. **Reasoning matters** — The tool's visible reasoning is as important as the codes themselves. This is what makes the process auditable and replicable.

5. **You're training the tool** — Every time you diverge from the tool's initial coding, you're providing training data for refinement. Make a note of it.

---

## Questions to Guide Your Coding

When you receive an abstract, ask yourself:

**For Layer 1:**
- Do I see explicitly named concepts from the list? (colorblind racism, microaggressions, intersectionality, etc.)
- Are these concepts presented as named theoretical frameworks or as working analytical language?

**For Layer 2:**
- Do I see redefined versions of foundational terms (harm, violence, power, trauma, etc.)?
- Are these terms deployed in agent-act-victim specification or in structural-position specification?
- Would the analysis differ if these vocabulary choices were changed?

**For Identity:**
- Are identity categories present?
- Are they demographic variables or analytical positions?
- Does the identity framework structure the analytical question itself?

**For Deployment Mode:**
- If Layer 2 vocabulary is present, is it foundational (the analysis), analytical (layered on top), or wrapping (presentational)?

**For Ambiguity:**
- Is anything unclear or difficult to code definitively?
- What additional information would help?
- Should I flag this for human judgment?

---

## Support & Refinement

As you use this tool:
- Flagged ambiguities will accumulate → These guide codebook refinement
- Divergences will accumulate → These guide tool prompt refinement
- Patterns will emerge → These will improve reliability over time

This is iterative. The tool and codebook improve through use.

