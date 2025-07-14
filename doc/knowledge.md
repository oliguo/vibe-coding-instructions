# Project Knowledge Base

**Version**: 1.0  
**Last Updated**: 2025-07-14  
**TDD Integration**: Kent Beck methodology with AI optimization

## Project Overview
This project implements AI-optimized development practices integrated with Test-Driven Development (TDD) and Tidy First principles.

## Core Principles Integration

### AI-Optimized TDD Workflow
- **Red Phase**: Write failing tests following AI-readable patterns (≤25 LOC per test)
- **Green Phase**: Implement minimal code to pass tests (≤25 LOC per function)
- **Refactor Phase**: Apply Tidy First principles with AI-assisted structural improvements

### Code Quality Standards (TDD + AI Compatible)
- Functions ≤ 25 LOC (F-LEN rule + TDD simplicity)
- Parameters ≤ 3 (F-PARAM rule + testability)
- Cyclomatic complexity ≤ 10 (maintainable + testable)
- Single responsibility principle (TDD + AI readability)

## Architecture Decisions

### Testing Strategy
- Unit tests: One test per behavior (TDD Red-Green-Refactor cycle)
- Integration tests: AI-assisted test generation for edge cases
- Test naming: Descriptive 4-6 word patterns following AI conventions

### Development Methodology
1. **Planning Phase**: Create todo files following AI naming conventions
2. **TDD Phase**: Implement Red-Green-Refactor cycles
3. **Tidy First Phase**: Separate structural from behavioral changes
4. **Documentation Phase**: Update knowledge base with AI-readable patterns

## Technical Requirements

### Development Environment
- IDE: VS Code + AI extensions (Cursor/Windsurf compatible)
- Testing Framework: Language-appropriate (Jest/pytest/etc.)
- AI Integration: MCP Context7 for knowledge base updates
- Version Control: Git with TDD commit discipline

### Quality Gates
- All tests passing before commit
- No compiler/linter warnings
- AI readability validation
- Function size compliance (≤25 LOC)

## Maintainability Guidelines

### Daily Practices
- Write one test at a time following TDD cycle
- Commit structural and behavioral changes separately
- Update knowledge base with new insights
- Run AI context refresh after significant changes

### Weekly Reviews
- Analyze test coverage and code quality
- Review AI optimization patterns
- Consolidate learning into documentation
- Plan next iteration improvements

## Security & Project Setup Requirements

### Essential Security Practices (FIRST PRIORITY)
- **Always create .gitignore before first commit** - Prevent sensitive data leaks
- **Setup .dockerignore for containerized projects** - Optimize builds and security
- **Create .env.example templates** - Document required environment variables
- **Validate no secrets in code** - Use environment variables for all sensitive data
- **Audit repository regularly** - Ensure no credentials accidentally committed

### Standard Ignore Files Required
1. **.gitignore**: Comprehensive patterns for OS, IDE, dependencies, secrets
2. **.dockerignore**: Optimize Docker builds, exclude development files
3. **.env.example**: Template for environment variables (no real secrets)
4. **Language-specific patterns**: Python __pycache__, Node node_modules/, etc.
5. **AI/ML specific**: Model files, datasets, experiment tracking directories

### Security Validation Checklist
- [ ] .gitignore created and comprehensive
- [ ] .env.example created (template only)
- [ ] .env added to .gitignore
- [ ] No API keys or passwords in code
- [ ] Database files ignored
- [ ] Build artifacts ignored
- [ ] AI model files ignored (if applicable)
- [ ] OS and IDE files ignored

## Integration Requirements

### MCP Context7 Usage
- Command: "Use Context7" after major requirement changes
- Frequency: Daily during active development
- Scope: Full project context including TDD progress
- Documentation: Immediate knowledge.md updates

### AI IDE Compatibility
- Follow structured patterns for consistent AI parsing
- Use descriptive naming conventions for AI understanding
- Maintain modular design for AI-assisted refactoring
- Include TODO(ai): markers for AI assistance points

## Next Steps
1. **SECURITY FIRST**: Create .gitignore, .dockerignore, .env.example
2. Create initial plan.md with TDD test roadmap
3. Set up development environment with testing framework
4. Implement first Red-Green-Refactor cycle
5. Document learnings and update this knowledge base
