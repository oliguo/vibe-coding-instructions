# AI IDE Project Documentation Instructions

**Version**: 2.0  
**Last Updated**: 2025-07-12  
**Compatible With**: Cursor, Windsurf, VS Code + AI Extensions

## Ove### 8. Maintenance Procedures

#### ## Implementation Checklist (AI-Enhanced)

Before implementing these instructions, ensure:
- [ ] **Directory structure created** (`doc/`, `app/`, `ideas/` with subdirs)
- [ ] **Initial knowledge.md exists** with AI coding guidelines integrated
- [ ] **Master tracking files initialized** (`todo.md`, `step_plan.md`)
- [ ] **AI IDE rules configured** (`.cursor/rules/` or `rules.md`)
- [ ] **File naming conventions understood** (YYYYMMDD_HHMMSS format)
- [ ] **Maintenance schedule established** (daily 5min, weekly 15min)
- [ ] **MCP Context7 integration tested** ("Use Context7" command)
- [ ] **AI assistant prompts prepared** (copy-paste snippets ready)

## AI-Optimized Examplestenance (≤ 5 minutes)
- **Task Status Updates**: Modify progress in tracking files
- **Knowledge Base Review**: Update `knowledge.md` with new insights
- **Completed Task Archive**: Move finished items to archive section
- **AI Context Refresh**: Run "Use Context7" if major changes

#### Weekly Maintenance (≤ 15 minutes)  
- **Progress Review**: Analyze overall project advancement
- **Step Plan Updates**: Refine plans based on learnings
- **Consolidation**: Merge duplicate or outdated information
- **Compliance Check**: Verify adherence to AI coding guidelines

#### Quality Assurance (Continuous)
- **Naming Convention Audit**: Ensure all files follow standards
- **Task Tracking Verification**: Confirm all tasks properly indexed
- **Documentation Consistency**: Maintain uniform formatting
- **AI Readability Test**: Validate structure supports AI parsing

## Implementation Checklist (AI-Enhanced)e guidelines for AI-optimized project documentation that ensures both human readability and AI assistant effectiveness. Follow these standards to maintain organized, traceable documentation supporting long-term maintainability and seamless AI collaboration.

## AI Optimization Principles
- **Token Efficiency**: Keep sections ≤ 300 lines for full context embedding
- **Structured Patterns**: Consistent formatting for AI parsing
- **Semantic Clarity**: Descriptive naming with 4-6 word conventions  
- **Modular Design**: Atomic components following single responsibility
- **Explicit Intent**: Clear documentation with examples

## Core Documentation Workflow

### 1. Knowledge Base Management
- **Primary Document**: `knowledge.md`
- **Purpose**: Consolidated project knowledge base (≤ 300 LOC per section)
- **Maintenance**: Immediate updates when new information available
- **Content Structure**:
  - Requirements analysis (AI coding standards, UI/UX, feasibility)
  - Architecture decisions (documented with rationale)
  - Maintainability guidelines (following F-LEN, F-RESP principles)
  - Integration requirements (MCP Context7, AI IDE compatibility)

### 2. Requirements Analysis Process
**Step-by-Step Workflow**:
1. **Read `ideas/` folder** - Analyze all requirement documents
2. **Apply AI coding standards** - Evaluate against function/module rules
3. **Document findings** in `knowledge.md` with:
   - Best UI/UX practices for AI readability
   - Long-term maintainability (≤ 25 LOC functions, ≤ 3 params)
   - Code readability (descriptive names, clear structure)
   - Technical feasibility (AI IDE compatibility)

### 3. Task Management Workflow

#### Task Creation Process
1. **Receive task assignment**
2. **Analyze and understand** the task requirements
3. **Create todo task file** using naming convention:
   ```
   YYYYMMDD_HHMMSS_todo_taskname.md
   ```
   Example: `20250710_203000_todo_makelandingpage.md`

4. **Update main todo.md** with new task entry including:
   - Task name
   - File reference
   - Status (Pending|In Progress|Completed)
   - Priority level
   - Estimated completion date

#### Step Planning Process
1. **Create detailed step plan** for each todo task
2. **Use naming convention**:
   ```
   YYYYMMDD_HHMMSS_steps_plan_taskname.md
   ```
   Example: `20250710_203000_steps_plan_makelandingpage.md`

3. **Update main step_plan.md** with:
   - Plan name
   - Associated todo task
   - File reference
   - Planning status

### 4. File Organization Standards

#### Directory Structure
```
doc/                              # Primary documentation root
├── knowledge.md                  # Central knowledge base (≤ 300 LOC)
├── todo.md                       # Master todo tracking  
├── step_plan.md                  # Master step plan index
├── todos/                        # Individual task files (≤ 25 LOC each)
│   └── YYYYMMDD_HHMMSS_todo_taskname.md
└── step_plans/                   # Step plan files (atomic sections)
    └── YYYYMMDD_HHMMSS_steps_plan_taskname.md

app/                              # Source code (following AI guidelines)
├── [modules ≤ 300 LOC each]
└── [functions ≤ 25 LOC, ≤ 3 params]

ideas/                            # Requirements repository
└── [requirement documents]
```

#### AI-Optimized File Naming
- **Date Format**: `YYYYMMDD` (ISO 8601, sortable)
- **Time Format**: `HHMMSS` (24-hour, precise)
- **Separators**: Underscores only (`_`) for AI parsing
- **Task Names**: `lowercase_descriptive_4_to_6_words`
- **Forbidden**: Special chars, spaces, inconsistent formatting

### 5. AI-Optimized Documentation Standards

#### Task Documentation Requirements (≤ 25 logical sections)
Each todo file must contain:
- **Task Description**: Clear, single-responsibility objective
- **Acceptance Criteria**: Measurable success conditions (≤ 10 items)
- **Dependencies**: Prerequisites and blockers (explicit listing)
- **Estimated Effort**: Time/resource requirements
- **Status Updates**: Progress tracking with timestamps
- **AI Hints**: `TODO(ai):` markers for AI assistant tasks

#### Step Plan Documentation Requirements (Atomic Structure)
Each step plan file must contain:
- **Overview**: High-level approach (≤ 3 paragraphs)
- **Detailed Steps**: Sequential, actionable items (≤ 10 steps per phase)
- **Resource Requirements**: Tools, skills, dependencies (explicit list)
- **Risk Assessment**: Potential challenges with mitigation strategies
- **Validation Criteria**: Verification steps (automatable where possible)
- **AI Integration**: Specific AI assistant capabilities utilized

#### Code Documentation Standards
- **Function Length**: ≤ 25 logical lines of code (F-LEN rule)
- **Parameter Limit**: ≤ 3 parameters or use dataclass/DTO (F-PARAM rule)
- **Cyclomatic Complexity**: ≤ 10 branches (F-CYCLO rule)
- **Nesting Depth**: ≤ 3 levels (F-NEST rule)
- **Documentation**: One-line summary + examples (F-DOC rule)

### 6. AI Integration Guidelines

#### MCP Context7 Integration
- **Command**: Use "Use Context7" for knowledge base updates
- **Frequency**: After each significant requirement change
- **Scope**: Full project context including guidelines and progress
- **Documentation**: Update `knowledge.md` with MCP insights

#### AI IDE Compatibility
- **Cursor**: Place rules in `.cursor/rules/ai-function-guidelines.md`
- **Windsurf**: Configure `rules.md` + `.aider.conf.yml`
- **General**: Follow structured patterns for consistent AI parsing

#### AI Assistant Prompt Patterns
```text
/agent apply house rules from ai-function-guidelines.md
Focus on F-LEN, F-RESP principles. Split functions >25 LOC.
Keep behavior identical. Validate with tests.
```

### 7. Quality Assurance & Validation

#### Pre-Commit Checklist (AI-Optimized)
- [ ] No functions >25 LOC or ≥4 parameters (F-LEN, F-PARAM)
- [ ] No classes with >8 public methods (M-EXPORTS)
- [ ] File length ≤300 LOC (M-SIZE)
- [ ] All public APIs documented with examples (F-DOC)
- [ ] Cyclomatic complexity ≤10 (F-CYCLO)
- [ ] Nesting depth ≤3 levels (F-NEST)
- [ ] Tests pass (`pytest -q` or equivalent)
- [ ] Documentation follows naming conventions
- [ ] AI-readable structure maintained

#### Automated Validation (CI Integration)
- **Code Quality**: Enforce function/module size limits
- **Documentation**: Verify all public APIs documented
- **Naming**: Check file naming convention compliance
- **Structure**: Validate directory organization
- **AI Compatibility**: Ensure guidelines are referenced

### 8. Maintenance Procedures

#### Daily Maintenance
- Update task statuses
- Review and update knowledge.md
- Check for completed tasks and archive if necessary

#### Weekly Maintenance
- Review overall project progress
- Update step plans based on learnings
- Consolidate duplicate or outdated information

#### Quality Assurance
- Ensure all files follow naming conventions
- Verify all tasks are properly tracked
- Maintain consistency across documentation

## Implementation Checklist

Before implementing these instructions, ensure:
- [ ] Directory structure is created
- [ ] Initial knowledge.md file exists
- [ ] Master todo.md and step_plan.md files are initialized
- [ ] File naming conventions are understood
- [ ] Maintenance schedule is established

## Examples

### Example Todo Task File (AI-Optimized)
```markdown
# Todo Task: Create Responsive Landing Page
**Created**: 2025-07-12 14:30:00
**Status**: Pending  
**Priority**: High
**Estimated Completion**: 2025-07-15
**AI Complexity**: Medium (UI components + responsive logic)

## Task Description (Single Responsibility)
Develop responsive landing page with hero section, features grid, and CTA button following F-LEN (≤25 LOC per component) and responsive design principles.

## Acceptance Criteria (≤ 10 Items)
- [ ] Mobile-first responsive design (320px to 1920px)
- [ ] Page load time ≤ 3 seconds (Core Web Vitals compliant)
- [ ] Images optimized and lazy-loaded
- [ ] SEO meta tags implemented
- [ ] Accessibility score ≥ 95 (WCAG 2.1 AA)
- [ ] Cross-browser compatibility (Chrome, Firefox, Safari, Edge)
- [ ] Component functions ≤ 25 LOC each
- [ ] CSS classes follow BEM methodology

## Dependencies (Explicit)
- Brand guidelines finalized (design system colors, fonts)
- Content copywriting completed (hero text, feature descriptions)  
- Image assets provided (hero image, feature icons)
- Development environment configured (build tools, linting)

## AI Integration Notes
- TODO(ai): Optimize image loading with lazy loading implementation
- TODO(ai): Generate responsive CSS grid for features section
- TODO(ai): Validate accessibility compliance automatically

## Technical Specifications
- **Framework**: Vanilla HTML/CSS/JS (no dependencies >10KB)
- **CSS**: Grid/Flexbox for layouts, CSS custom properties
- **JS**: ES6+ modules, ≤ 3 parameters per function
- **Performance Budget**: Bundle size ≤ 100KB total
```

### Example Step Plan File (Atomic Structure)
```markdown
# Step Plan: Create Responsive Landing Page
**Created**: 2025-07-12 14:30:00
**Associated Todo**: 20250712_143000_todo_create_responsive_landing_page.md
**AI Optimization Level**: High (structured for AI assistant collaboration)

## Overview (≤ 3 Paragraphs)
Develop high-performance landing page using atomic component methodology. Each component follows F-LEN rule (≤25 LOC) with clear single responsibility. Focus on mobile-first responsive design with performance optimization.

Implementation uses modern CSS (Grid/Flexbox) and vanilla JavaScript (ES6+ modules). All functions maintain ≤3 parameters and ≤10 cyclomatic complexity for AI readability.

## Detailed Steps (≤ 10 Per Phase)

### Phase 1: Design Foundation (Day 1)
1. **Review brand guidelines** - Extract design tokens (colors, fonts, spacing)
2. **Create wireframe structure** - Define atomic components hierarchy
3. **Design responsive breakpoints** - Mobile (320px), Tablet (768px), Desktop (1024px)
4. **Component specification** - Document each component's single responsibility

### Phase 2: Development Setup (Day 1)  
1. **Initialize project structure** - Following M-SIZE rule (≤300 LOC per file)
2. **Configure build tools** - ESLint, Prettier, performance budgets
3. **Create base CSS** - Custom properties, reset, typography system
4. **Set up component templates** - HTML structure with semantic markup

### Phase 3: Component Development (Day 2-3)
1. **Hero section component** - Single CTA, background image, responsive text
2. **Features grid component** - 3-column layout, icon + text pairs
3. **Call-to-action component** - Button with hover states, form validation
4. **Performance optimization** - Image lazy loading, CSS/JS minification

### Phase 4: Testing & Validation (Day 4)
1. **Cross-browser testing** - Chrome, Firefox, Safari, Edge compatibility
2. **Responsive testing** - All breakpoints, device orientation changes
3. **Performance audit** - Core Web Vitals, bundle size validation
4. **Accessibility validation** - WCAG 2.1 AA compliance, screen reader testing

## Resource Requirements (Explicit)
- **Design Tools**: Figma access for design system tokens
- **Development**: VS Code + AI extensions (Cursor/Windsurf compatible)
- **Testing**: BrowserStack or local device lab for cross-browser testing
- **Performance**: Lighthouse CI, WebPageTest for optimization validation

## Risk Assessment (With AI Mitigation)
- **Risk**: Design approval delays → **Mitigation**: AI-generated design variations for rapid iteration
- **Risk**: Performance budget exceeded → **Mitigation**: AI code analysis for bundle optimization
- **Risk**: Cross-browser compatibility issues → **Mitigation**: AI-assisted feature detection and polyfills

## Validation Criteria (Automatable)
- [ ] All components ≤25 LOC (automated linting rule)
- [ ] Functions have ≤3 parameters (ESLint custom rule)
- [ ] Performance budget met (Lighthouse CI integration)
- [ ] Accessibility score ≥95 (automated axe-core testing)
- [ ] Cross-browser compatibility confirmed (automated testing suite)
- [ ] AI readability maintained (structure validation script)

## AI Assistant Integration
- **Code Generation**: Use AI for responsive CSS grid patterns
- **Optimization**: AI-driven image compression and lazy loading
- **Testing**: AI-generated test cases for edge cases
- **Documentation**: AI-assisted inline documentation generation
```

---

## Quick Reference for AI Assistants

### Copy-Paste Prompts
```text
/agent apply ai-function-guidelines.md rules
Focus on F-LEN (≤25 LOC), F-RESP (single responsibility), F-PARAM (≤3 params)
Split any function >25 LOC into pure helpers. Keep behavior identical.
```

```text
/agent create new module following M-STRUCT pattern
Top-down order: constants → types → helpers → main API
Expose clear exports, use descriptive 4-6 word names
```

```text
/agent optimize for AI readability
Apply knowledge.md guidelines, maintain ≤300 LOC per file
Use TODO(ai): markers for AI assistant tasks
```

### File Organization Quick Check
- ✅ Functions ≤ 25 LOC (F-LEN)
- ✅ Files ≤ 300 LOC (M-SIZE)  
- ✅ Parameters ≤ 3 (F-PARAM)
- ✅ Nesting ≤ 3 levels (F-NEST)
- ✅ Descriptive 4-6 word names
- ✅ ISO 8601 timestamps (YYYYMMDD_HHMMSS)

---

**Version**: 2.0 | **Last Updated**: 2025-07-12 | **AI Compatible**: Cursor, Windsurf, VS Code
*This document follows its own guidelines - structured for both human readability and AI assistant effectiveness.*