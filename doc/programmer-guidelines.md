# Programmer Guidelines: TDD + AI-Optimized Development

**Target Audience**: Software Engineers  
**Version**: 1.0  
**Date**: 2025-07-14

## Core Development Workflow

### Daily TDD Cycle
1. **Morning Setup** (5 minutes)
   - Review `plan.md` for next unmarked test
   - Check `knowledge.md` for any overnight updates
   - Ensure development environment is ready

2. **TDD Implementation** (Red-Green-Refactor)
   - **Red Phase**: Write one failing test (≤25 LOC)
   - **Green Phase**: Implement minimal code to pass (≤25 LOC, ≤3 params)
   - **Refactor Phase**: Apply Tidy First principles

3. **AI Integration** (Throughout)
   - Use TODO(ai): markers for AI assistance points
   - Leverage AI for code generation within TDD constraints
   - Update documentation with AI-readable patterns

### Code Quality Standards

#### Function Guidelines (F-LEN, F-PARAM, F-RESP)
```javascript
// ✅ GOOD: Follows all rules
function validateTaskName(name, maxLength, pattern) {  // ≤3 params
  if (!name) return false;                            // Single responsibility
  if (name.length > maxLength) return false;         // ≤25 LOC total
  return pattern.test(name);
}

// ❌ BAD: Violates multiple rules
function processComplexTaskWithMultipleValidationsAndTransformations(
  taskData, options, callbacks, validators, transformers, config
) {
  // 40+ lines of mixed responsibilities
  // Multiple nested conditions
  // Side effects and mutations
}
```

#### Test Writing Best Practices
```javascript
// ✅ GOOD: Clear, focused test
describe('validateTaskName', () => {
  it('shouldReturnFalseWhenNameExceedsMaxLength', () => {
    const result = validateTaskName('very_long_task_name', 10, /^[a-z_]+$/);
    expect(result).toBe(false);
  });
});

// ❌ BAD: Testing multiple behaviors
it('shouldValidateTaskNameWithVariousInputs', () => {
  // Testing 5+ different scenarios in one test
  // Unclear which assertion failed
  // Mixed responsibilities
});
```

### Commit Discipline

#### Structural Changes (Tidy First)
```bash
# Examples of structural commits
git commit -m "structural: extract validateEmail helper function"
git commit -m "structural: rename userId to accountId for clarity" 
git commit -m "structural: reorganize imports alphabetically"
```

#### Behavioral Changes (TDD)
```bash
# Examples of behavioral commits  
git commit -m "feat: add email validation for user registration"
git commit -m "feat: implement task status update workflow"
git commit -m "test: add edge case for empty task names"
```

### AI-Assisted Development

#### Effective AI Prompts for TDD
```text
/agent implement failing test for [specific behavior]
Follow TDD Red phase, function ≤25 LOC, descriptive test name
Focus on single behavior validation

/agent write minimal code to pass this test
Follow F-LEN (≤25 LOC), F-PARAM (≤3 params), single responsibility
Keep implementation simple, no over-engineering

/agent refactor following Tidy First principles
Separate structural from behavioral changes
Maintain test coverage, improve code clarity
```

#### TODO(ai) Usage Patterns
```javascript
// TODO(ai): Generate validation regex for ISO 8601 timestamps
// TODO(ai): Optimize database query for large datasets
// TODO(ai): Add error handling for network timeouts
// TODO(ai): Extract common validation logic into utility
```

### IDE Configuration

#### VS Code + AI Extensions Setup
1. **Cursor Integration**
   - Place TDD rules in `.cursor/rules/tdd-guidelines.md`
   - Configure auto-formatting on save
   - Enable real-time code analysis

2. **Testing Configuration**
   - Auto-run tests on file save
   - Display test coverage in editor
   - Highlight failing tests immediately

3. **AI-Optimized Settings**
   ```json
   {
     "editor.rulers": [25],  // Visual guide for F-LEN rule
     "editor.wordWrap": "bounded",
     "editor.wordWrapColumn": 80,
     "eslint.rules": {
       "max-lines-per-function": ["error", 25],
       "max-params": ["error", 3]
     }
   }
   ```

### Performance Optimization

#### Build Time Targets
- Unit test execution: ≤2 seconds for full suite
- Code compilation: ≤5 seconds for incremental builds
- AI assistance response: ≤3 seconds for code suggestions

#### Memory Management
- Keep function complexity low for AI parsing efficiency
- Use descriptive naming to reduce AI context requirements
- Maintain modular structure for selective AI analysis

### Troubleshooting Common Issues

#### TDD Cycle Problems
1. **Test Won't Fail**: Verify test actually exercises the code path
2. **Test Too Complex**: Split into multiple single-behavior tests
3. **Code Too Complex**: Apply single responsibility principle

#### AI Integration Issues
1. **Poor AI Suggestions**: Improve TODO(ai) context and specificity
2. **Context Overload**: Break large functions into smaller units
3. **Naming Confusion**: Use 4-6 word descriptive patterns

### Daily Checklist
- [ ] Run full test suite before starting work
- [ ] Select next test from plan.md
- [ ] Follow Red-Green-Refactor cycle
- [ ] Commit structural and behavioral changes separately
- [ ] Update knowledge.md with learnings
- [ ] Use AI assistance for routine tasks
- [ ] Validate all quality gates before pushing

### Weekly Review Process
1. **Code Quality Metrics**: Review function size, parameter counts
2. **Test Coverage**: Ensure adequate coverage for new features
3. **AI Effectiveness**: Analyze AI assistance quality and usage
4. **TDD Compliance**: Verify proper cycle adherence
5. **Documentation Updates**: Consolidate learnings into knowledge base
