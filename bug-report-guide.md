# Bug Report Guide for AI Agents

When analyzing software bugs, follow this Guide to create comprehensive reports that identify root causes and explore potential solutions before implementing any code changes.

## 1. Issue Description
1. Clearly describe the observed behavior versus expected behavior
2. Document exact reproduction steps in numbered sequence
3. Specify the environment details (OS, browser, device, versions)
4. Include relevant error messages, logs, and stack traces
5. Reference any visual evidence (screenshots, videos) if mentioned

## 2. Impact Assessment
1. Enumerate all affected users, systems, or features
2. Assign a severity rating (critical, high, medium, low) with justification
3. Document any existing workarounds
4. Quantify performance impacts where possible
5. Identify potential cascading effects on related systems

## 3. Root Cause Analysis
1. Systematically investigate these common causes:
   - Logic implementation flaws
   - Unexpected data patterns or edge case inputs
   - State management inconsistencies
   - Resource constraints (memory, CPU, network)
   - Race conditions or timing issues
   - External dependency failures
   - Configuration mismatches
   - Environmental factors
2. Trace the execution path leading to the bug
3. Identify violated assumptions in the code
4. Provide a confidence level for each potential cause

## 4. Potential Solutions
1. Present three distinct solution approaches:

   **Solution A: Quick Fix**
   - Describe the fastest implementation approach
   - List specific pros (e.g., minimal changes, immediate relief)
   - List specific cons (e.g., technical debt, limited scope)
   - Rate implementation complexity (Low/Medium/High)
   - Estimate implementation time

   **Solution B: Robust Fix**
   - Describe a comprehensive solution addressing the root cause
   - List specific pros (e.g., complete resolution, future-proofing)
   - List specific cons (e.g., extensive testing needed, higher risk)
   - Rate implementation complexity (Low/Medium/High)
   - Estimate implementation time

   **Solution C: Alternative Approach**
   - Describe a fundamentally different strategy
   - List specific pros (e.g., architectural improvement, extensibility)
   - List specific cons (e.g., refactoring required, broader impact)
   - Rate implementation complexity (Low/Medium/High)
   - Estimate implementation time

## 5. Recommended Approach
1. Select and justify the best solution based on:
   - Implementation timeline constraints
   - Fix completeness requirements
   - Long-term maintainability needs
   - Risk tolerance for introducing new issues
2. Explain specific reasons for this recommendation
3. Identify any technical debt implications
4. Note any prerequisites or dependencies for implementation

## 6. Verification Plan
1. Enumerate specific test cases that must pass
2. Describe exact verification steps to confirm the fix
3. Identify potential regression areas to test
4. Outline monitoring recommendations post-implementation

## 7. Prevention Strategy
1. Suggest specific preventative measures:
   - Unit or integration tests that could have caught this
   - Code review practices to implement
   - Architectural improvements to consider
   - Documentation updates needed
   - Monitoring enhancements to implement

Always provide this structured analysis before suggesting any code changes. Your goal is to ensure understanding of the issue and thoughtful solution comparison. 