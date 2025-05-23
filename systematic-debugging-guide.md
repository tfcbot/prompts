# Systematic Debugging Guide

When facing a complex bug or issue, follow this structured debugging approach before making code changes:

## 1. Problem Analysis
- Identify exact observed behavior vs expected behavior
- Verify reproducibility and conditions
- Determine likely responsible system parts
- Consider recent changes that might have caused the issue

## 2. Context Gathering
- Review the broader system architecture
- Examine component interactions
- Identify external dependencies
- Consider environment-specific factors

## 3. Hypothesis Formation
- List potential root causes by likelihood
- Consider common issues:
  - State management problems
  - Race conditions
  - Resource constraints
  - Configuration issues
  - Error handling gaps
  - Edge cases
- Challenge assumptions about expected behavior

## 4. Investigation Strategy
- Plan efficient validation steps
- Determine conclusive evidence needed
- Consider instrumentation requirements
- Create minimal test cases when possible

## 5. Solution Design
- Evaluate how precisely fixes address root causes
- Consider potential side effects
- Look for cleaner alternatives
- Avoid masking deeper issues
- Design with maintainability in mind

## 6. Verification Planning
- Establish confirmation criteria
- Determine necessary tests
- Set up appropriate monitoring
- Watch for partial fixes or new issues

## 7. Knowledge Integration
- Extract patterns from the issue
- Implement preventative measures
- Update documentation and tests
- Improve future debugging capability

Always work through these steps systematically before writing code fixes to minimize false starts and build comprehensive understanding.
