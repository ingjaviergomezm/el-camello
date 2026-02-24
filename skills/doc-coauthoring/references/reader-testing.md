# Reader Testing Protocol

**Goal:** Test the document with a fresh Claude (no context bleed) to verify it works for readers. This catches blind spots — things that make sense to the authors but might confuse others.

## With Sub-Agent Access (e.g., Antigravity, Claude Code)

Perform testing directly without user involvement.

### Step 1: Predict Reader Questions
Generate 5-10 questions readers would realistically ask when discovering this document.

### Step 2: Test with Sub-Agent
For each question, invoke a sub-agent with just the document content and the question. Summarize what Reader Claude got right/wrong.

### Step 3: Run Additional Checks
Invoke sub-agent to check for ambiguity, false assumptions, contradictions. Summarize issues found.

### Step 4: Report and Fix
If issues found, list them. Loop back to refinement for problematic sections.

---

## Without Sub-Agent Access (e.g., claude.ai web)

The user does the testing manually.

### Step 1: Predict Reader Questions
Generate 5-10 reader questions collaboratively.

### Step 2: Setup Testing
Instruct the user to:
1. Open a fresh Claude conversation: https://claude.ai
2. Paste or share the document content
3. Ask Reader Claude the generated questions

For each question, instruct Reader Claude to provide:
- The answer
- Whether anything was ambiguous or unclear
- What knowledge/context the doc assumes is already known

### Step 3: Additional Checks
Also ask Reader Claude:
- "What in this doc might be ambiguous or unclear to readers?"
- "What knowledge or context does this doc assume readers already have?"
- "Are there any internal contradictions or inconsistencies?"

### Step 4: Iterate Based on Results
Fix gaps found by Reader Claude. Loop back to refinement.

---

## Exit Condition
When Reader Claude consistently answers questions correctly and doesn't surface new gaps or ambiguities, the doc is ready.
