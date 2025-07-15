# Vibe Coding Instructions - AI-Optimized TDD Framework

**Version**: 2.0  
**Framework**: Kent Beck TDD + AI-Optimized Development  
**Compatible**: Cursor, Windsurf, VS Code + AI Extensions

## Credits & Methodology

This framework integrates **Kent Beck's Test-Driven Development (TDD)** and **Tidy First** methodologies with AI-optimized development practices.

**TDD Methodology Credit**: [Kent Beck](https://github.com/KentBeck/BPlusTree3/blob/main/rust/docs/CLAUDE.md) - Original TDD principles and Red-Green-Refactor cycle

**Core Principles Applied**:

```mermaid
graph LR
    A[TDD Cycle] --> B[Red: Failing Test]
    B --> C[Green: Minimal Code]
    C --> D[Refactor: Tidy First]
    D --> B
    
    E[AI Optimization] --> F[≤25 LOC Functions]
    E --> G[≤3 Parameters]
    E --> H[Single Responsibility]
    
    I[Quality Gates] --> J[All Tests Pass]
    I --> K[No Compiler Warnings]
    I --> L[AI Readability]
    
    style A fill:#ffcdd2
    style E fill:#c8e6c9
    style I fill:#bbdefb
```

- Always follow the TDD cycle: Red → Green → Refactor
- Write the simplest failing test first
- Implement minimum code needed to make tests pass
- Separate structural changes from behavioral changes (Tidy First)
- Maintain high code quality throughout development

## Project Structure Overview

```mermaid
graph TD
    A[Vibe Coding Instructions Framework] --> B[Source Code]
    A --> C[Requirements]
    A --> D[Documentation]
    A --> E[AI Optimization: ai-ide-instructions.md]
    
    B --> B1[≤300 LOC per file]
    B --> B2[≤25 LOC per function]
    B --> B3[≤3 parameters per function]
    
    C --> C1[PRD.md]
    C --> C2[Technical Specs]
    C --> C3[Product Requirements]
    
    D --> D1[knowledge.md - Central Knowledge Base]
    D --> D2[plan.md - TDD Test Roadmap]
    D --> D3[todo.md - Master Task Tracking]
    D --> D4[step_plan.md - Implementation Plans]
    D --> D5[Role Guidelines]
    D --> D6[Individual Tasks: todos/]
    D --> D7[Detailed Plans: step_plans/]
    
    D5 --> D5A[programmer-guidelines.md]
    D5 --> D5B[designer-guidelines.md]
    D5 --> D5C[tester-guidelines.md]
    
    E --> E1[F-LEN: ≤25 LOC]
    E --> E2[F-PARAM: ≤3 params]
    E --> E3[F-RESP: Single responsibility]
    E --> E4[M-SIZE: ≤300 LOC files]
    
    style A fill:#e1f5fe
    style B fill:#f3e5f5
    style C fill:#e8f5e8
    style D fill:#fff3e0
    style E fill:#fce4ec
```

### Directory Structure
```
├── @/app/                   # Source code (≤300 LOC per file, ≤25 LOC per function)
├── @/ideas/                 # Requirements and project concepts
├── @/doc/                   # Documentation and guidelines
│   ├── knowledge.md         # Central knowledge base (use MCP Context7)
│   ├── plan.md             # TDD test roadmap (20 tests ready)
│   ├── todo.md             # Master task tracking
│   ├── step_plan.md        # Master step plan index
│   ├── programmer-guidelines.md    # TDD + AI development workflow
│   ├── designer-guidelines.md      # AI-optimized design patterns
│   ├── tester-guidelines.md        # Quality assurance strategy
│   ├── todos/              # Individual task files (YYYYMMDD_HHMMSS format)
│   └── step_plans/         # Detailed implementation plans
└── ai-ide-instructions.md  # Core AI optimization principles
```

---

## 🚀 New Requirements & AI Startup Workflow

```mermaid
flowchart TD
    A[Add PRD.md to ideas folder] --> B[Phase 1: Requirements Analysis]
    B --> C[Phase 2: Security & Structure Setup]
    C --> D[Phase 3: Development Cycle Kickoff]
    D --> E[Phase 4: Task Management]
    
    B --> B1[Step 1: Analyze Requirements<br/>AI Prompt: Extract tech requirements]
    B --> B2[Step 2: Update Knowledge Base<br/>Use Context7 + consolidate insights]
    
    C --> C1[Step 3: Security Validation<br/>Validate .gitignore, .dockerignore]
    C --> C2[Step 4: Map to TDD Tests<br/>Link requirements to plan.md]
    
    D --> D1[Step 5: Start TDD Cycle<br/>go command + Red phase]
    D --> D2[Step 6: Green Implementation<br/>≤25 LOC, ≤3 params]
    D --> D3[Step 7: Refactor<br/>Tidy First principles]
    
    E --> E1[Step 8: Create Task Files<br/>YYYYMMDD_HHMMSS format]
    E --> E2[Step 9: Generate Step Plans<br/>Atomic implementation steps]
    
    E --> F[Continue TDD Cycles]
    F --> D1
    
    style A fill:#e8f5e8
    style B fill:#e3f2fd
    style C fill:#fff3e0
    style D fill:#f3e5f5
    style E fill:#fce4ec
    style F fill:#e0f2f1
```

## 🔄 Complete Document Integration Workflow

```mermaid
graph TD
    subgraph "Input Documents"
        A[PRD.md in ideas folder]
        B[PR.md - Pull Request]
        C[Technical Specs]
    end
    
    subgraph "Document Processing Pipeline"
        D[Step 1: Document Analysis]
        E[Step 2: Knowledge Integration]
        F[Step 3: Task Generation]
        G[Step 4: Implementation Planning]
    end
    
    subgraph "Framework Documents"
        H[ai-ide-instructions.md]
        I[knowledge.md]
        J[plan.md - 20 TDD Tests]
        K[todo.md - Task Tracking]
        L[step_plan.md - Plans Index]
    end
    
    subgraph "Role Guidelines"
        M[programmer-guidelines.md]
        N[designer-guidelines.md]
        O[tester-guidelines.md]
    end
    
    subgraph "Implementation Outputs"
        P[Individual TODO Files]
        Q[Step Plan Files]
        R[Source Code in app/]
        S[Test Implementation]
    end
    
    A --> D
    B --> D
    C --> D
    
    D --> E
    E --> F
    F --> G
    
    H --> E
    I --> E
    J --> F
    K --> F
    L --> G
    
    M --> G
    N --> G
    O --> G
    
    G --> P
    G --> Q
    P --> R
    Q --> S
    
    style A fill:#e8f5e8
    style B fill:#ffe0b2
    style H fill:#fce4ec
    style I fill:#fff3e0
    style R fill:#f3e5f5
```

### **Complete Integration Workflow: From Requirements to Code**

When you add requirements documents (PRD.md, PR.md, technical specs, etc.) to the [`@/ideas/`](ideas) folder, follow this systematic integration workflow that connects all framework documents:

### **Phase 1: Document Analysis & Requirements Processing**

```mermaid
sequenceDiagram
    participant User as User
    participant AI as AI Assistant
    participant Ideas as ideas/ folder
    participant AiInst as ai-ide-instructions.md
    participant Know as knowledge.md
    participant Context as MCP Context7
    
    User->>Ideas: Add PRD.md or PR.md
    User->>AI: Analyze new requirements
    AI->>Ideas: Read all requirement documents
    AI->>AiInst: Apply AI optimization principles
    AI-->>User: Requirements analysis complete
    
    User->>Context: Use Context7
    Context->>Know: Update knowledge base
    AI->>Know: Consolidate insights with framework
    AI-->>User: Knowledge base updated
    
    Note over User,Know: Phase 1 Complete: Requirements understood
```

#### **Step 1: Requirements Analysis with Framework Integration**
```bash
# AI Prompt for Comprehensive Requirements Analysis
/agent analyze new requirements from @/ideas/ folder
Apply framework principles from @/ai-ide-instructions.md:
- F-LEN: Break features into ≤25 LOC functions
- F-PARAM: Design APIs with ≤3 parameters
- F-RESP: Single responsibility per component
- M-SIZE: Keep modules ≤300 LOC

Extract and document:
- UI/UX requirements mapping to @/doc/designer-guidelines.md
- Technical implementation following @/doc/programmer-guidelines.md
- Testing strategy aligned with @/doc/tester-guidelines.md
- Maintainability considerations for long-term AI assistance

Update @/doc/knowledge.md with consolidated analysis
```

#### **Step 2: Knowledge Base Integration**
```bash
# MCP Context7 Integration
Use Context7

# AI Knowledge Consolidation Prompt
/agent update @/doc/knowledge.md with comprehensive integration
Cross-reference with existing framework documents:
- Validate against established patterns in @/doc/plan.md
- Check consistency with @/doc/todo.md priorities
- Align with @/doc/step_plan.md methodology
- Ensure compatibility with role-specific guidelines

Document integration points and dependencies
Identify potential conflicts with existing architecture
```

#### **Phase 1: Requirements Analysis & Knowledge Base Setup**

**Step 1: Analyze Requirements**
```bash
# AI Prompt for Requirements Analysis
/agent analyze requirements from @/ideas/ folder
Apply AI coding standards from @/ai-ide-instructions.md
Focus on F-LEN (≤25 LOC), F-PARAM (≤3 params), single responsibility
Extract UI/UX requirements, technical feasibility, maintainability considerations
Document findings in @/doc/knowledge.md following ≤300 LOC sections
```

**Step 2: Update Knowledge Base with MCP Context7**
```bash
# Command to refresh AI context
Use Context7

# Follow-up AI Prompt
/agent update @/doc/knowledge.md with MCP Context7 insights
Consolidate requirements analysis with:
- Best UI/UX practices for AI readability
- Long-term maintainability (≤25 LOC functions)
- Code readability (descriptive names, clear structure)
- Technical feasibility (AI IDE compatibility)
```

### **Phase 2: Task Generation & Planning Integration**

```mermaid
sequenceDiagram
    participant Know as knowledge.md
    participant Plan as plan.md
    participant Todo as todo.md
    participant StepPlan as step_plan.md
    participant AI as AI Assistant
    participant Guidelines as Role Guidelines
    
    Know->>AI: Requirements consolidated
    AI->>Plan: Map to TDD test roadmap
    Plan->>Todo: Generate specific tasks
    Todo->>StepPlan: Create implementation plans
    
    AI->>Guidelines: Apply role-specific patterns
    Guidelines-->>StepPlan: Validate against constraints
    
    Note over Know,Guidelines: Phase 2 Complete: Tasks planned
```

#### **Step 3: TDD Test Mapping & Integration**
```bash
# AI Test Integration Prompt
/agent analyze @/doc/plan.md 20-test roadmap
Map new requirements from @/ideas/ to existing test framework:
- Cross-reference with @/doc/programmer-guidelines.md TDD methodology
- Cross-reference with @/doc/tester-guidelines.md quality standards
- Cross-reference with @/doc/designer-guidelines.md testable components

For each requirement:
- Identify which existing tests cover new functionality
- Create additional tests if needed (following TDD Red-Green-Refactor)
- Prioritize tests based on:
  * Core functionality importance
  * Risk assessment from requirements
  * Dependencies between features
  * Integration with existing @/doc/todo.md priorities

Update plan.md with new test scenarios
Ensure each test follows ≤25 LOC constraint
Validate test names follow shouldDoSomething pattern
Cross-reference with all role guidelines for comprehensive coverage
```

#### **Step 4: Comprehensive Task Decomposition**
```bash
# AI Task Generation Prompt (Framework-Integrated)
/agent create comprehensive task breakdown
Based on updated @/doc/plan.md and @/doc/knowledge.md
Integrate with ALL framework documents:

For each requirement, generate tasks using role guidelines:

PROGRAMMER TASKS (apply @/doc/programmer-guidelines.md):
- TDD implementation tasks (Red-Green-Refactor cycles)
- Code structure following F-LEN (≤25 LOC), F-PARAM (≤3 params)
- AI integration points for code generation
- Security validation tasks

DESIGNER TASKS (apply @/doc/designer-guidelines.md):
- Component design with ≤3 props (F-PARAM mapping)
- Atomic design system integration
- Testable UI specification
- AI assistance for design token generation

TESTER TASKS (apply @/doc/tester-guidelines.md):
- Test strategy aligned with TDD cycles
- Quality gate validation
- AI-assisted test case generation
- Performance and accessibility validation

Each task file: YYYYMMDD_HHMMSS_todo_taskname.md must include:
- Single responsibility description
- Acceptance criteria (≤10 items, measurable)
- Dependencies linking to framework documents
- AI integration points (TODO(ai) markers)
- Role assignment and cross-role dependencies

Update @/doc/todo.md with complete integrated task index
```

### **Phase 3: Implementation Planning & Role Integration**

```mermaid
flowchart TD
    A[Tasks from todo.md] --> B[Role Assignment Matrix]
    
    B --> C[Programmer Tasks]
    B --> D[Designer Tasks]
    B --> E[Tester Tasks]
    
    C --> C1[programmer-guidelines.md]
    D --> D1[designer-guidelines.md]
    E --> E1[tester-guidelines.md]
    
    C1 --> F[Cross-Role Integration]
    D1 --> F
    E1 --> F
    
    F --> G[Unified Step Plans]
    G --> H[YYYYMMDD_HHMMSS_steps_plan_*.md]
    H --> I[step_plan.md Index Update]
    
    I --> J[TDD Implementation Ready]
    J --> K[go command execution]
    
    style A fill:#fff3e0
    style C fill:#f3e5f5
    style D fill:#e8f5e8
    style E fill:#e3f2fd
    style F fill:#ffecb3
    style K fill:#e0f2f1
```

#### **Step 5: Integrated Step Planning**
```bash
# AI Step Plan Generation (Cross-Role Integration)
/agent create detailed step plans with framework integration
Following ALL role-specific guidelines with cross-dependencies:

For each task, create unified step plan that integrates:

TECHNICAL IMPLEMENTATION (programmer-guidelines.md):
- TDD Red-Green-Refactor methodology
- Function constraints: ≤25 LOC, ≤3 parameters
- Atomic commits (structural vs behavioral)
- AI assistance points for code generation
- Security validation checkpoints

UI/UX IMPLEMENTATION (designer-guidelines.md):
- Atomic design principles
- Component specs with ≤3 props (F-PARAM mapping)
- Design-to-code AI generation points
- Testability considerations for development

QUALITY ASSURANCE (tester-guidelines.md):
- Test integration with TDD cycles
- Quality gates and automation
- AI-assisted test generation
- Cross-browser and accessibility validation

CROSS-ROLE DEPENDENCIES:
- Designer → Programmer: Component specs for implementation
- Programmer → Tester: Code structure for test design
- Tester → Designer: Accessibility feedback for design
- All roles → knowledge.md: Consolidated learnings

Each step plan file: YYYYMMDD_HHMMSS_steps_plan_taskname.md
Include comprehensive resource requirements and validation criteria
Update @/doc/step_plan.md with integrated index
```

#### **Phase 4: Security Validation & Project Setup**

**Step 6: Security Validation (CRITICAL FIRST)**
```bash
# AI Security Audit Prompt
/agent validate project security setup
Confirm .gitignore, .dockerignore, .env.example are comprehensive
Audit for any sensitive data in repository
Create language-specific ignore patterns if needed
Validate no API keys, passwords, or secrets in code
```

### **Phase 5: TDD Implementation & Continuous Integration**

```mermaid
graph TD
    A[All Phases Complete] --> B[go Command]
    B --> C[First TDD Cycle]
    
    subgraph "TDD Implementation"
        C --> D[Red Phase: Write Failing Test]
        D --> E[Green Phase: Minimal Implementation]
        E --> F[Refactor Phase: Tidy First]
        F --> G[Documentation Update]
        G --> H[Next Test Selection]
        H --> D
    end
    
    subgraph "PR Integration"
        I[PR.md Created] --> J[Link to Implementation]
        J --> K[Testing & Verification]
        K --> L[Documentation Updates]
        L --> M[Ready for Review]
    end
    
    G --> I
    M --> N[Deployment Ready]
    
    style A fill:#e0f2f1
    style B fill:#ffcdd2
    style N fill:#c8e6c9
```

#### **Step 7: TDD Implementation Launch**
```bash
# Command to start implementation
go

# This triggers the first test from plan.md following complete integration:
/agent implement failing test for [first behavior from updated plan.md]
Apply framework integration:
- Use knowledge.md context for implementation approach
- Follow programmer-guidelines.md for TDD Red phase
- Consider designer-guidelines.md for UI-related tests
- Integrate tester-guidelines.md quality standards

Test implementation must:
- Follow ≤25 LOC constraint (ai-ide-instructions.md)
- Use descriptive shouldDoSomething naming pattern
- Include single behavior validation
- Reference framework documentation in test comments
```

#### **Step 8: Pull Request Integration (PR.md)**
When creating PR.md documents, integrate with framework:

```bash
# AI PR Integration Prompt
/agent create PR.md following framework standards
Based on completed implementation and framework documents:

## Background (Why) - Reference Framework Docs
- Link to original requirements in @/ideas/
- Reference decisions documented in @/doc/knowledge.md
- Cross-reference with @/doc/plan.md test implementations

## Implementation Approach (How) - Framework Compliance
- Validate against @/ai-ide-instructions.md constraints:
  * Functions ≤25 LOC (F-LEN compliance)
  * Parameters ≤3 (F-PARAM compliance)
  * Single responsibility (F-RESP compliance)
- Reference @/doc/programmer-guidelines.md TDD methodology
- Include @/doc/designer-guidelines.md design decisions (if UI)
- Document @/doc/tester-guidelines.md quality validations

## Actual Changes (What was done) - Cross-Reference Tasks
- Link to completed tasks in @/doc/todo.md
- Reference step plans in @/doc/step_plan.md
- Update @/doc/knowledge.md with implementation insights

## Testing & Verification - Framework Integration
- Validate all tests from @/doc/plan.md pass
- Confirm @/doc/tester-guidelines.md standards met
- Include AI assistance effectiveness metrics
- Document any framework constraint violations and resolutions

## Framework Compliance Checklist:
- [ ] All functions ≤25 LOC (F-LEN)
- [ ] All functions ≤3 parameters (F-PARAM)
- [ ] TDD Red-Green-Refactor cycle followed
- [ ] Documentation updated in knowledge.md
- [ ] Tasks marked complete in todo.md
- [ ] Cross-role guidelines followed
- [ ] AI optimization maintained
```

### **Continuous Framework Integration**

```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Framework as Framework Docs
    participant AI as AI Assistant
    participant Quality as Quality Gates
    
    loop Every Commit
        Dev->>Framework: Check compliance
        Framework->>AI: Apply constraints
        AI->>Dev: Validate implementation
        Dev->>Quality: Run quality gates
        Quality-->>Dev: Pass/Fail feedback
    end
    
    loop Weekly Review
        Dev->>Framework: Update learnings
        Framework->>AI: Refresh context
        AI->>Framework: Suggest improvements
    end
    
    Note over Dev,Quality: Continuous Integration with Framework
```

### **Complete Integration Checklist**

Before considering any feature complete, validate integration across ALL framework documents:

#### **Document Integration Validation**
```bash
# AI Integration Validation Prompt
/agent validate complete framework integration
Check all document cross-references and consistency:

REQUIREMENTS INTEGRATION:
- [ ] @/ideas/ documents fully processed
- [ ] @/doc/knowledge.md updated with all insights
- [ ] Requirements mapped to @/doc/plan.md tests

ROLE INTEGRATION:
- [ ] @/doc/programmer-guidelines.md patterns followed
- [ ] @/doc/designer-guidelines.md principles applied
- [ ] @/doc/tester-guidelines.md standards met

TASK INTEGRATION:
- [ ] All tasks created in @/doc/todo.md
- [ ] Step plans generated in @/doc/step_plan.md
- [ ] Cross-dependencies documented

AI OPTIMIZATION INTEGRATION:
- [ ] @/ai-ide-instructions.md rules enforced
- [ ] Function constraints validated (≤25 LOC, ≤3 params)
- [ ] AI readability patterns maintained

TDD INTEGRATION:
- [ ] Red-Green-Refactor cycles completed
- [ ] All tests in @/doc/plan.md implemented
- [ ] Quality gates passing

DOCUMENTATION INTEGRATION:
- [ ] Knowledge base current and comprehensive
- [ ] All TODO(ai) markers addressed
- [ ] Framework compliance documented
```

### **Sample Complete Integration: PRD → Running Code → PR**

```bash
# Complete End-to-End Example
# 1. Add PRD.md to ideas/
echo "New user authentication feature" > ideas/PRD_user_auth.md

# 2. Run complete integration workflow
/agent analyze requirements from @/ideas/PRD_user_auth.md
Apply @/ai-ide-instructions.md principles
Cross-reference ALL @/doc/ guidelines
Update @/doc/knowledge.md with integrated analysis

# 3. Generate integrated tasks and plans
/agent create tasks following framework integration
Reference @/doc/programmer-guidelines.md for TDD tasks
Reference @/doc/designer-guidelines.md for UI tasks
Reference @/doc/tester-guidelines.md for QA tasks
Update @/doc/todo.md and @/doc/step_plan.md

# 4. Start TDD implementation
go
/agent implement first failing test
Follow complete framework integration

# 5. Create PR with framework compliance
/agent create PR.md with framework documentation
Include compliance checklist and cross-references
Document framework integration points
```

This integration ensures that when AI assistants receive new PRD.md or PR.md documents, they follow a systematic approach that leverages ALL framework documents, maintains strong connections between them, and produces consistently high-quality, maintainable code that follows TDD principles and AI optimization constraints.

#### **Phase 3: Development Cycle Kickoff**

**Step 5: Start First TDD Cycle**
```bash
# Command to begin development
go

# AI Implementation Prompt
/agent implement failing test for [first behavior from plan.md]
Follow TDD Red phase:
- Test name: shouldDoSomething pattern (≤25 LOC)
- Single behavior validation
- Descriptive assertions
- No implementation code yet
```

**Step 6: Minimal Implementation (Green Phase)**
```bash
# AI Green Phase Prompt
/agent write minimal code to pass current failing test
Follow F-LEN (≤25 LOC), F-PARAM (≤3 params), F-RESP (single responsibility)
No over-engineering, just enough to make test pass
Maintain AI readability patterns from @/ai-ide-instructions.md
```

**Step 7: Refactoring (Tidy First)**
```bash
# AI Refactoring Prompt
/agent refactor following Tidy First principles
Separate structural from behavioral changes:
1. Structural: extract helpers, rename variables, reorganize imports
2. Behavioral: new features, logic changes
Commit each type separately with proper prefixes (structural: / feat:)
```

#### **Phase 4: Task Management & Documentation**

**Step 8: Create Task Files**
```bash
# AI Task Creation Prompt
/agent create todo task file for [specific feature]
Use naming: YYYYMMDD_HHMMSS_todo_featurename.md
Include:
- Task description (single responsibility)
- Acceptance criteria (≤10 items, measurable)
- Dependencies (explicit prerequisites)
- AI integration points (TODO(ai) markers)
Update @/doc/todo.md with new task entry
```

**Step 9: Generate Detailed Step Plans**
```bash
# AI Step Planning Prompt
/agent create step plan for [todo task]
Use naming: YYYYMMDD_HHMMSS_steps_plan_featurename.md
Structure with:
- Overview (≤3 paragraphs)
- Detailed steps (≤10 per phase, atomic ≤25 LOC implementations)
- Resource requirements (explicit tools, skills, dependencies)
- Risk assessment (with AI-assisted mitigation strategies)
- Validation criteria (automatable where possible)
Update @/doc/step_plan.md index
```

### **Sample Complete Workflow: From PRD to Running Code**

```bash
# 1. Process Requirements
/agent analyze requirements from @/ideas/PRD.md
Apply AI coding standards, extract technical requirements

# 2. Update Knowledge Base
Use Context7
/agent update @/doc/knowledge.md with consolidated insights

# 3. Security Check
/agent validate comprehensive security setup

# 4. Plan Tests
/agent map PRD requirements to @/doc/plan.md TDD tests

# 5. Start Development
go
/agent implement failing test for user authentication

# 6. Implement Minimal Code
/agent write minimal code to pass authentication test

# 7. Refactor & Clean
/agent refactor following Tidy First principles

# 8. Create Tasks
/agent create todo task for dashboard component

# 9. Continue Cycle
# Select next test from plan.md and repeat
```

### **Daily AI-Assisted Development Routine**

```bash
# Morning Standup (≤5 minutes)
/agent daily standup analysis
Check @/doc/todo.md for today's priorities
Review @/doc/knowledge.md for overnight updates
Select next unmarked test from @/doc/plan.md
Validate AI-optimization compliance (F-LEN, F-PARAM, F-RESP)

# Development Cycle
/agent implement next TDD cycle
Follow Red-Green-Refactor methodology
Maintain ≤25 LOC functions, ≤3 parameters
Update documentation with learnings

# End of Day
/agent update progress tracking
Mark completed tasks in @/doc/todo.md
Update @/doc/knowledge.md with insights
Prepare tomorrow's priorities
```

---

## 🚀 Project Initialization (New Team Members)

```mermaid
graph TD
    A[New Team Member] --> B{What's Your Role?}
    
    B --> C[Project Leader/CTO]
    B --> D[Developer]
    B --> E[Designer]
    B --> F[Tester/QA]
    
    C --> C1[Read Framework Docs]
    C --> C2[Use Context7]
    C --> C3[Assign Team Roles]
    
    D --> D1[Read AI Optimization Rules]
    D --> D2[Setup IDE + AI Extensions]
    D --> D3[SECURITY FIRST: Create Ignore Files]
    D --> D4[Start TDD Cycle: go command]
    
    E --> E1[Read Design Guidelines]
    E --> E2[Setup Design System]
    E --> E3[Create Component Specs]
    
    F --> F1[Read Testing Strategy]
    F --> F2[Setup Test Environment]
    F --> F3[Join TDD Cycle]
    
    C1 --> C1A[ai-ide-instructions.md]
    C1 --> C1B[doc/knowledge.md]
    C1 --> C1C[doc/plan.md]
    
    D1 --> D1A[≤25 LOC functions]
    D1 --> D1B[≤3 parameters]
    D1 --> D1C[Single responsibility]
    
    D3 --> D3A[.gitignore]
    D3 --> D3B[.dockerignore]
    D3 --> D3C[.env.example]
    
    E2 --> E2A[Design tokens → code constants]
    E2 --> E2B[≤3 props per component]
    E2 --> E2C[Testable interactions]
    
    F2 --> F2A[Test frameworks]
    F2 --> F2B[Coverage reporting]
    F2 --> F2C[CI integration]
    
    style C fill:#e1f5fe
    style D fill:#f3e5f5
    style E fill:#e8f5e8
    style F fill:#fff3e0
```

### **For Project Leaders/CTOs**
```bash
# 1. Read core framework
📖 Read: @/ai-ide-instructions.md (AI optimization principles)
📖 Read: @/doc/knowledge.md (project knowledge base)
📖 Read: @/doc/plan.md (TDD roadmap with 20 tests)

# 2. Update knowledge base
💡 Command: "Use Context7" (MCP server integration)
📝 Update: @/doc/knowledge.md with project requirements from @/ideas/

# 3. Assign roles and review guidelines
👥 Team: Review role-specific guidelines in @/doc/
🎯 Next: Choose starting point based on team composition
```

### **For Developers (First Time)**
```bash
# 1. Understand the framework
📖 Read: @/ai-ide-instructions.md (Function rules: ≤25 LOC, ≤3 params)
📖 Read: @/doc/programmer-guidelines.md (TDD workflow)
📖 Read: @/doc/plan.md (Available tests to implement)

# 2. Setup development environment
⚙️ Configure: IDE with AI extensions (Cursor/Windsurf/VS Code)
⚙️ Setup: Testing framework and linting rules
⚙️ Validate: F-LEN, F-PARAM compliance in IDE

# 3. Create security and ignore files (CRITICAL FIRST STEP)
🔒 Create: .gitignore (prevent sensitive files in git)
🔒 Create: .dockerignore (optimize docker builds)
🔒 Create: .env.example (template for environment variables)
🔒 Setup: IDE-specific ignore patterns
🔒 Validate: No sensitive data in repository

# 4. Start TDD cycle
🔴 Command: "go" (Implements first test from plan.md)
🟢 Follow: Red-Green-Refactor methodology
📝 Update: @/doc/knowledge.md with learnings
```

### **For Designers (First Time)**
```bash
# 1. Understand design constraints
📖 Read: @/doc/designer-guidelines.md (Atomic design + TDD)
📖 Read: @/ai-ide-instructions.md (AI-optimized patterns)
📖 Review: Component size limits (≤25 LOC implementation)

# 2. Setup design system
🎨 Create: Design tokens mapping to code constants
🎨 Plan: Components with ≤3 props (F-PARAM rule)
🎨 Document: Testable interaction specifications

# 3. Collaborate with development
🤝 Review: @/doc/plan.md for UI-related tests
📝 Create: Component specs following guidelines
✅ Validate: Designs support automated testing
```

### **For Testers/QA (First Time)**
```bash
# 1. Understand testing strategy
📖 Read: @/doc/tester-guidelines.md (TDD integration)
📖 Read: @/doc/plan.md (20 tests ready for implementation)
📖 Review: Quality gates and validation criteria

# 2. Setup testing environment
⚙️ Configure: Test frameworks and automation tools
⚙️ Setup: Coverage reporting and CI integration
⚙️ Prepare: Test data fixtures and mocks

# 3. Join TDD cycle
🔴 Collaborate: Help write meaningful failing tests
🟢 Validate: Minimal implementations meet requirements
🔧 Ensure: Structural changes don't break functionality
```

---

## 🔄 Project Continuation (Daily/Weekly Work)

```mermaid
sequenceDiagram
    participant D as Developer
    participant T as Tester
    participant Des as Designer
    participant AI as AI Assistant
    participant K as Knowledge Base
    
    Note over D,K: Daily Workflow (≤5 minutes setup)
    
    D->>K: Check todo.md priorities
    D->>K: Review knowledge.md updates
    D->>AI: Select next test from plan.md
    
    Note over D,AI: TDD Red-Green-Refactor Cycle
    
    D->>AI: /agent implement failing test
    AI-->>D: Test code ≤25 LOC
    D->>AI: /agent write minimal implementation
    AI-->>D: Code ≤25 LOC, ≤3 params
    
    T->>AI: /agent validate test quality
    AI-->>T: Coverage + quality metrics
    
    Des->>AI: /agent design component specs
    AI-->>Des: ≤3 props, testable states
    
    D->>AI: /agent refactor following Tidy First
    AI-->>D: Structural vs behavioral separation
    
    Note over D,K: End of Day
    D->>K: Update progress in todo.md
    D->>K: Document insights in knowledge.md
    
    Note over D,K: Weekly Review
    rect rgb(240, 248, 255)
        D->>AI: /agent weekly progress review
        AI-->>D: Compliance metrics + suggestions
        D->>K: Update team learnings
    end
```

### **Daily Standup Prompt**
```bash
# Morning routine (≤5 minutes)
📋 Check: @/doc/todo.md for today's priorities
📖 Review: @/doc/knowledge.md for overnight updates
🎯 Select: Next unmarked test from @/doc/plan.md (if developing)
⚡ Command: "Use Context7" (if major changes occurred)

# Role-specific daily prep
👨‍💻 Developers: Review @/doc/programmer-guidelines.md TDD cycle
🎨 Designers: Check @/doc/designer-guidelines.md for component work
🧪 Testers: Review @/doc/tester-guidelines.md for validation tasks
```

### **Weekly Progress Review**
```bash
# Team lead review (≤15 minutes)
📊 Analyze: @/doc/todo.md completion rates
📈 Review: @/doc/plan.md test implementation progress
🔍 Validate: AI-optimization compliance across codebase
📝 Update: @/doc/knowledge.md with team learnings

# Quality assurance check
✅ Verify: Functions ≤25 LOC, ≤3 parameters
✅ Confirm: TDD Red-Green-Refactor cycles followed
✅ Check: Documentation consistency across @/doc/
✅ Validate: AI readability patterns maintained
```

---

## � Security & Project Setup (CRITICAL FIRST STEP)

### **When Starting Any New Project**
```bash
# Security and ignore files setup (BEFORE any code commits)
🔒 Create: Standard ignore files to prevent data leaks
📁 Setup: Project structure with security best practices
🛡️ Validate: No sensitive information in version control
⚙️ Configure: Environment variable templates
```

### **Essential Ignore Files to Create**

#### 1. .gitignore (Universal - Always Required)
```bash
# AI Development Environment
.cursor/
.windsurf/
.vscode/settings.json
.vscode/launch.json

# Dependencies
node_modules/
venv/
env/
.env
.env.local
.env.development
.env.production

# Build outputs
dist/
build/
target/
out/
*.log
*.tmp

# OS generated files
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# IDE files
*.swp
*.swo
*~
.idea/
.vscode/
*.sublime-project
*.sublime-workspace

# Test coverage
coverage/
.nyc_output/
.coverage
htmlcov/

# Cache directories
.cache/
.npm/
.yarn/cache/
__pycache__/
*.pyc
*.pyo
*.pyd

# Database files
*.db
*.sqlite
*.sqlite3

# API keys and secrets
config/secrets/
.env*
!.env.example
secrets.json
credentials.json
service-account-key.json

# AI model files (often large)
*.h5
*.pkl
*.joblib
models/
checkpoints/

# Documentation builds
docs/_build/
site/
```

#### 2. .dockerignore (For Docker Projects)
```bash
# Version control
.git
.gitignore

# Documentation
README.md
docs/
*.md

# Development files
.env*
!.env.example
.vscode/
.cursor/
.windsurf/

# Dependencies (install fresh in container)
node_modules/
venv/
env/

# Build artifacts
dist/
build/
target/
*.log

# OS files
.DS_Store
Thumbs.db

# Test files
tests/
**/*.test.*
coverage/

# CI/CD files
.github/
.gitlab-ci.yml
Jenkinsfile
```

#### 3. .env.example (Environment Template)
```bash
# Database Configuration
DATABASE_URL=postgresql://user:password@localhost:5432/dbname
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_NAME=your_database_name

# API Keys (Use actual keys in .env file, never commit)
API_KEY=your_api_key_here
SECRET_KEY=your_secret_key_here
JWT_SECRET=your_jwt_secret_here

# AI Service Configuration
OPENAI_API_KEY=your_openai_key_here
ANTHROPIC_API_KEY=your_anthropic_key_here

# Application Settings
NODE_ENV=development
PORT=3000
DEBUG=true

# External Services
REDIS_URL=redis://localhost:6379
ELASTICSEARCH_URL=http://localhost:9200

# Email Configuration
SMTP_HOST=smtp.example.com
SMTP_PORT=587
SMTP_USER=your_email@example.com
SMTP_PASS=your_email_password
```

#### 4. Language-Specific Ignore Patterns

**For Python Projects:**
```bash
# Add to .gitignore
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
pip-wheel-metadata/
share/python-wheels/
*.egg-info/
.installed.cfg
*.egg
MANIFEST
```

**For Node.js Projects:**
```bash
# Add to .gitignore
npm-debug.log*
yarn-debug.log*
yarn-error.log*
lerna-debug.log*
.pnpm-debug.log*
.npm
.eslintcache
.yarn-integrity
.yarn/cache/
.yarn/unplugged/
.yarn/build-state.yml
.yarn/install-state.gz
.pnp.*
```

**For AI/ML Projects:**
```bash
# Add to .gitignore
# Jupyter Notebook
.ipynb_checkpoints
*.ipynb

# Data files (often large/sensitive)
data/
datasets/
*.csv
*.json
*.parquet

# Model artifacts
models/
weights/
checkpoints/
*.h5
*.pkl
*.joblib
*.onnx

# Experiment tracking
mlruns/
.mlflow/
wandb/
```

### **Security Validation Checklist**
```bash
# Before first commit, verify:
✅ .gitignore created and comprehensive
✅ .env.example created (template only, no real secrets)
✅ .env added to .gitignore
✅ No API keys, passwords, or secrets in code
✅ Database files ignored
✅ Build artifacts ignored
✅ OS-specific files ignored
✅ IDE-specific files ignored
✅ Large binary files ignored
✅ AI model files ignored (if applicable)
```

### **AI Programming Security Commands**
```bash
# Security validation prompts for AI assistants
🔒 "/agent create comprehensive .gitignore for [language/framework]"
🔒 "/agent validate no sensitive data in repository"
🔒 "/agent create .env.example template for project dependencies"
🔒 "/agent setup .dockerignore optimized for [project type]"
🔒 "/agent audit codebase for hardcoded secrets or credentials"
```

### **Post-Setup Validation**
```bash
# After creating ignore files, run these commands:
git status                    # Verify sensitive files not tracked
git check-ignore -v file.env  # Test ignore patterns work
docker build . --dry-run     # Verify dockerignore effectiveness (if using Docker)
```

## 💻 Development Phase Prompts

```mermaid
stateDiagram-v2
    [*] --> Planning: New Feature Request
    
    Planning --> Red: Feature Planned
    Planning --> Planning: Refine Requirements
    
    state Red {
        [*] --> WriteTest: Start TDD Cycle
        WriteTest --> ValidateTest: Test Written ≤25 LOC
        ValidateTest --> TestFails: Run Test
        TestFails --> [*]: Red Phase Complete
    }
    
    Red --> Green: Test Failing
    
    state Green {
        [*] --> WriteCode: Implement Minimal Code
        WriteCode --> ValidateCode: Code ≤25 LOC, ≤3 params
        ValidateCode --> TestPasses: Run All Tests
        TestPasses --> [*]: Green Phase Complete
    }
    
    Green --> Refactor: Tests Passing
    
    state Refactor {
        [*] --> StructuralChanges: Tidy First Approach
        StructuralChanges --> BehavioralChanges: Separate Commits
        BehavioralChanges --> ValidateRefactor: Maintain Test Coverage
        ValidateRefactor --> [*]: Refactor Complete
    }
    
    Refactor --> Documentation: Code Clean
    
    state Documentation {
        [*] --> UpdateKnowledge: Document Insights
        UpdateKnowledge --> UpdateTodos: Track Progress
        UpdateTodos --> [*]: Documentation Complete
    }
    
    Documentation --> Planning: Next Feature
    Documentation --> [*]: Feature Complete
    
    state AI_Assistant {
        RedPhase: /agent implement failing test
        GreenPhase: /agent write minimal code
        RefactorPhase: /agent refactor following Tidy First
        ValidatePhase: /agent validate compliance
    }
    
    Red --> AI_Assistant
    Green --> AI_Assistant
    Refactor --> AI_Assistant
```

### **AI-Optimized TDD Cycle**

```mermaid
flowchart TD
    A[🔴 RED PHASE] --> A1[Write Failing Test]
    A1 --> A2[≤25 LOC per test]
    A2 --> A3[Single behavior validation]
    A3 --> A4[Descriptive test name]
    A4 --> A5[Run test - must fail]
    
    A5 --> B[🟢 GREEN PHASE]
    B --> B1[Write minimal code]
    B1 --> B2[≤25 LOC functions]
    B2 --> B3[≤3 parameters]
    B3 --> B4[Single responsibility]
    B4 --> B5[Run tests - all pass]
    
    B5 --> C[🔧 REFACTOR PHASE]
    C --> C1[Structural changes first]
    C1 --> C2[Extract helpers]
    C2 --> C3[Rename for clarity]
    C3 --> C4[Reorganize imports]
    C4 --> C5[Behavioral changes second]
    C5 --> C6[Separate commits]
    
    C6 --> D[📝 DOCUMENT]
    D --> D1[Update knowledge.md]
    D1 --> D2[Update todo progress]
    D2 --> D3[Add AI markers]
    
    D3 --> E{Next Test?}
    E -->|Yes| A
    E -->|No| F[Feature Complete]
    
    style A fill:#ffcdd2
    style B fill:#c8e6c9
    style C fill:#bbdefb
    style D fill:#fff3e0
```

### **When Starting New Features**
```bash
# Feature planning
📖 Read: @/doc/knowledge.md for context
📝 Create: New todo file using YYYYMMDD_HHMMSS_todo_featurename.md
📋 Plan: Break feature into ≤25 LOC functions
🎯 Add: Test to @/doc/plan.md following TDD pattern

# TDD implementation
🔴 Red: Write failing test (≤25 LOC)
🟢 Green: Implement minimal code to pass
🔧 Refactor: Apply Tidy First principles
📝 Document: Update @/doc/knowledge.md with insights
```

### **When Debugging Issues**
```bash
# Debugging workflow
📖 Review: @/doc/programmer-guidelines.md error handling
🔍 Check: @/doc/plan.md for related tests
🧪 Add: Failing test that reproduces the bug (TDD approach)
🔧 Fix: Minimal code to make tests pass
📝 Update: @/doc/knowledge.md with root cause analysis
```

### **When Adding Dependencies**
```bash
# Dependency validation
📖 Check: @/ai-ide-instructions.md for dependency guidelines
🔍 Validate: Library supports ≤25 LOC integration patterns
🧪 Test: Integration following @/doc/tester-guidelines.md
📝 Document: Update @/doc/knowledge.md with integration notes
```

---

## 🎨 Design Phase Prompts

### **When Creating New Components**
```bash
# Component design workflow
📖 Read: @/doc/designer-guidelines.md atomic design principles
🎯 Plan: Component with ≤3 props (F-PARAM rule)
📝 Specify: Testable states and interactions
🧪 Document: Test scenarios for developers
✅ Validate: Design supports ≤25 LOC implementation
```

### **When Updating Design System**
```bash
# Design system evolution
📖 Review: @/doc/designer-guidelines.md for patterns
🔍 Analyze: @/app/ for implementation constraints
🎨 Update: Design tokens mapping to code constants
📝 Document: Changes in @/doc/knowledge.md
🤝 Coordinate: With developers for TDD integration
```

---

## 🧪 Testing Phase Prompts

### **When Writing Tests**
```bash
# Test creation workflow
📖 Follow: @/doc/tester-guidelines.md TDD patterns
🔴 Write: One failing test per behavior (≤25 LOC)
📝 Name: Descriptive test names (shouldDoSomething pattern)
🎯 Focus: Single responsibility per test
✅ Validate: Test covers edge cases and errors
```

### **When Validating Quality**
```bash
# Quality assurance workflow
📊 Run: Full test suite (≤2 min execution time)
📈 Check: Coverage metrics (≥85% target)
🔍 Validate: All functions ≤25 LOC, ≤3 parameters
📝 Review: @/doc/plan.md for test completion status
🚀 Approve: Ready for deployment if all gates pass
```

---

## 🚀 Deployment Phase Prompts

### **When Preparing for Release**
```bash
# Pre-deployment checklist
✅ Verify: All tests in @/doc/plan.md implemented
✅ Confirm: @/doc/knowledge.md is up-to-date
✅ Validate: AI-optimization compliance across @/app/
✅ Check: Performance benchmarks within limits
📝 Document: Release notes and deployment guide
```

### **When Monitoring Production**
```bash
# Post-deployment monitoring
📊 Monitor: Performance metrics vs benchmarks
🔍 Track: Error rates and user feedback
📝 Update: @/doc/knowledge.md with production insights
🔄 Plan: Next iteration based on learnings
```

---

## 🤖 AI Integration Commands & Troubleshooting

### **Context Management**
```bash
# Knowledge base updates
💡 "Use Context7" - Update knowledge base with MCP server
📝 Update @/doc/knowledge.md after major requirement changes
🔄 Refresh AI context when switching between projects
```

### **AI-Assisted Development**
```bash
# Effective AI prompts
🔴 "/agent implement failing test for [behavior] following TDD Red phase"
🟢 "/agent write minimal code to pass test, ≤25 LOC, ≤3 params"
🔧 "/agent refactor following Tidy First principles"
📝 "/agent update documentation following AI-readable patterns"

# Security-focused AI prompts
🔒 "/agent create comprehensive .gitignore for [language/framework]"
🔒 "/agent validate no sensitive data in repository"
🔒 "/agent audit codebase for hardcoded secrets or credentials"
🔒 "/agent setup environment variable management securely"
```

### **Role-Specific AI Prompts**

#### **For Designers:**
```bash
# Component Design Prompts
/agent design component following @/doc/designer-guidelines.md
Create atomic component with:
- Single responsibility purpose
- ≤3 props (maps to F-PARAM rule)
- Testable states (default, hover, error, disabled)
- AI-readable structure for code generation
Document component specification with implementation notes

# Design System Prompts
/agent generate design tokens following atomic design principles
Map design constants to code variables
Ensure ≤25 LOC implementation per component
Create testable interaction specifications
```

#### **For Testers:**
```bash
# Test Strategy Prompts
/agent create test strategy following @/doc/tester-guidelines.md
Design tests for:
- Unit tests (≤25 LOC per test, single behavior)
- Integration tests (API, workflows, data)
- Performance tests (≤2 sec unit tests, ≤30 sec integration)
- Accessibility tests (WCAG 2.1 AA compliance)
Use TODO(ai) markers for AI-assisted test generation

# Quality Assurance Prompts
/agent validate quality gates for deployment readiness
Check coverage metrics (≥85% target)
Verify all functions ≤25 LOC, ≤3 parameters
Validate TDD Red-Green-Refactor cycle compliance
Generate test reports with AI effectiveness metrics
```

#### **For Programmers:**
```bash
# TDD Cycle Prompts
/agent apply house rules from @/ai-ide-instructions.md
Focus on F-LEN (≤25 LOC), F-RESP (single responsibility), F-PARAM (≤3 params)
Split any function >25 LOC into pure helpers
Keep behavior identical, validate with tests

# Code Review Prompts
/agent review code for AI optimization compliance
Check function length, parameter count, cyclomatic complexity
Suggest refactoring opportunities following Tidy First
Validate descriptive naming conventions (4-6 words)
```

### **Emergency AI Troubleshooting Prompts**

#### **When Tests Fail:**
```bash
/agent debug failing test following @/doc/programmer-guidelines.md
1. Verify test exercises correct code path
2. Check if test is too complex (split if >25 LOC)
3. Apply single responsibility to implementation
4. Add failing test that reproduces bug (TDD approach)
5. Fix with minimal code to pass tests
```

#### **When AI Suggestions Are Poor:**
```bash
/agent improve AI context for better suggestions
1. Improve TODO(ai) markers with specific context
2. Break large functions into ≤25 LOC units
3. Use descriptive 4-6 word naming patterns
4. Verify compliance with @/ai-ide-instructions.md
5. Update @/doc/knowledge.md with clearer requirements
```

#### **When Code Becomes Complex:**
```bash
/agent simplify complex code following framework rules
Apply F-LEN rule: split functions >25 LOC
Apply F-PARAM rule: use DTOs for >3 parameters
Apply F-NEST rule: reduce nesting to ≤3 levels
Apply Tidy First: separate structural from behavioral changes
Maintain test coverage throughout refactoring
```

### **Weekly AI-Assisted Reviews**
```bash
# Progress Analysis
/agent weekly progress review
Analyze @/doc/todo.md completion rates
Review @/doc/plan.md test implementation progress
Validate AI-optimization compliance across codebase:
- Functions ≤25 LOC (F-LEN)
- Parameters ≤3 (F-PARAM)
- Files ≤300 LOC (M-SIZE)
- Cyclomatic complexity ≤10
Update @/doc/knowledge.md with team learnings

# Quality Metrics Review
/agent generate quality metrics report
Track test coverage, code complexity, AI assistance effectiveness
Identify patterns in bugs, performance issues, technical debt
Suggest improvements for next iteration
Plan refactoring priorities using Tidy First principles
```

---

## 📚 Quick Reference Guide

### **Framework Knowledge Flow**

```mermaid
graph TB
    subgraph "Input Layer"
        A[PRD.md in ideas folder]
        B[Technical Specs]
        C[Product Requirements]
    end
    
    subgraph "AI Processing Layer"
        D[MCP Context7]
        E[AI Analysis Engine]
        F[Requirement Processor]
    end
    
    subgraph "Knowledge Base Layer"
        G[knowledge.md]
        H[plan.md - 20 TDD Tests]
        I[todo.md - Task Tracking]
        J[step_plan.md - Implementation Plans]
    end
    
    subgraph "Guidelines Layer"
        K[ai-ide-instructions.md]
        L[programmer-guidelines.md]
        M[designer-guidelines.md]
        N[tester-guidelines.md]
    end
    
    subgraph "Implementation Layer"
        O[App Source Code]
        P[Individual Tasks]
        Q[Step Plans]
    end
    
    subgraph "Quality Gates"
        R[≤25 LOC Functions]
        S[≤3 Parameters]
        T[TDD Compliance]
        U[AI Readability]
    end
    
    A --> D
    B --> D
    C --> D
    
    D --> E
    E --> F
    F --> G
    
    G --> H
    G --> I
    G --> J
    
    K --> L
    K --> M
    K --> N
    
    H --> O
    I --> P
    J --> Q
    
    L --> O
    M --> O
    N --> O
    
    O --> R
    O --> S
    O --> T
    O --> U
    
    R --> V[Production Ready Code]
    S --> V
    T --> V
    U --> V
    
    style A fill:#e8f5e8
    style D fill:#e3f2fd
    style G fill:#fff3e0
    style K fill:#fce4ec
    style O fill:#f3e5f5
    style V fill:#e0f2f1
```

### **Phase Reference Table**

| Phase | Primary Files | Key Commands | Success Criteria |
|-------|---------------|--------------|------------------|
| **Security Setup** | .gitignore, .dockerignore, .env.example | Create ignore files | No sensitive data tracked |
| **Init** | ai-ide-instructions.md, knowledge.md | "Use Context7" | Framework understood |
| **Plan** | plan.md, todo.md | Select next test | Clear roadmap |
| **Design** | designer-guidelines.md | Create component specs | Testable designs |
| **Develop** | programmer-guidelines.md | "go" command | TDD cycle complete |
| **Test** | tester-guidelines.md | Run test suite | All quality gates pass |
| **Deploy** | All docs updated | Validate compliance | Production ready |

### **AI Optimization Quick Check**

```mermaid
pie title AI Compliance Metrics
    "Functions ≤25 LOC" : 25
    "Parameters ≤3" : 20
    "Single Responsibility" : 20
    "Files ≤300 LOC" : 15
    "Cyclomatic Complexity ≤10" : 10
    "AI Readability Patterns" : 10
```

### **Emergency Commands**
| Issue | Command | Expected Outcome |
|-------|---------|------------------|
| **Tests Failing** | `/agent debug failing test following @/doc/programmer-guidelines.md` | Root cause identified, minimal fix applied |
| **Poor AI Suggestions** | `/agent improve AI context for better suggestions` | Enhanced TODO(ai) markers, clearer requirements |
| **Code Too Complex** | `/agent simplify complex code following framework rules` | Functions split to ≤25 LOC, reduced complexity |
| **Security Concerns** | `/agent audit codebase for hardcoded secrets or credentials` | No sensitive data in repository |
| **Performance Issues** | `/agent weekly progress review` | Compliance metrics, improvement suggestions |

---

**🎯 Ready to Start?** Choose your role above and follow the corresponding prompts. Remember: this framework combines Kent Beck's TDD with AI-optimization for maximum development effectiveness.