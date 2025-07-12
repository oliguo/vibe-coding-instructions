# AI IDE Project Documentation Instructions

## Overview
Follow these guidelines to maintain organized, traceable project documentation that supports long-term maintainability and collaboration.

## Core Documentation Workflow

### 1. Knowledge Base Management
- **Primary Document**: `knowledge.md`
- **Purpose**: Consolidated project knowledge base
- **Maintenance**: Update immediately when new information becomes available
- **Content**: Requirements analysis, UI/UX considerations, architecture decisions, maintainability guidelines

### 2. Requirements Analysis Process
- Read all documents from the `ideas/` folder
- Analyze requirements for:
  - Best UI/UX practices
  - Long-term maintainability
  - Code readability and human-friendliness
  - Technical feasibility
- Document findings in `knowledge.md`

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
docs/
├── knowledge.md              # Central knowledge base
├── todo.md                   # Master todo tracking
├── step_plan.md             # Master step plan index
├── todos/                   # Individual task files
│   └── YYYYMMDD_HHMMSS_todo_taskname.md
└── step_plans/              # Individual step plan files
    └── YYYYMMDD_HHMMSS_steps_plan_taskname.md
```

#### File Naming Best Practices
- **Date Format**: YYYYMMDD (ISO 8601 standard)
- **Time Format**: HHMMSS (24-hour format)
- **Separators**: Use underscores (_) only
- **Task Names**: Use lowercase, no spaces, descriptive
- **Avoid**: Special characters, spaces, inconsistent formatting

### 5. Documentation Standards

#### Task Documentation Requirements
Each todo file must contain:
- **Task Description**: Clear, concise objective
- **Acceptance Criteria**: Measurable success conditions
- **Dependencies**: Prerequisites and blockers
- **Estimated Effort**: Time/resource requirements
- **Status Updates**: Progress tracking

#### Step Plan Documentation Requirements
Each step plan file must contain:
- **Overview**: High-level approach
- **Detailed Steps**: Sequential, actionable items
- **Resource Requirements**: Tools, skills, dependencies
- **Risk Assessment**: Potential challenges
- **Validation Criteria**: How to verify completion

### 6. Maintenance Procedures

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

### Example Todo Task File
```markdown
# Todo Task: Create Landing Page
**Created**: 2025-07-10 20:30:00
**Status**: Pending
**Priority**: High
**Estimated Completion**: 2025-07-15

## Task Description
Create a responsive landing page for the project that includes hero section, features overview, and call-to-action.

## Acceptance Criteria
- [ ] Responsive design works on mobile and desktop
- [ ] Page loads under 3 seconds
- [ ] All images are optimized
- [ ] SEO meta tags are implemented

## Dependencies
- Brand guidelines finalized
- Content copywriting completed

## Notes
- Follow existing design system
- Ensure accessibility compliance
```

### Example Step Plan File
```markdown
# Step Plan: Create Landing Page
**Created**: 2025-07-10 20:30:00
**Associated Todo**: 20250710_203000_todo_makelandingpage.md

## Overview
Develop a high-converting landing page using modern web technologies with focus on performance and user experience.

## Detailed Steps
1. **Design Phase**
   - Review brand guidelines
   - Create wireframes
   - Design mockups

2. **Development Phase**
   - Set up development environment
   - Implement HTML structure
   - Add CSS styling
   - Implement JavaScript interactions

3. **Testing Phase**
   - Cross-browser testing
   - Mobile responsiveness testing
   - Performance optimization

4. **Deployment Phase**
   - Deploy to staging
   - Review and approval
   - Deploy to production

## Resource Requirements
- Design tools (Figma/Adobe XD)
- Development environment
- Testing devices/browsers
- Deployment pipeline access

## Risk Assessment
- **Risk**: Design approval delays
- **Mitigation**: Early stakeholder involvement
- **Risk**: Performance issues
- **Mitigation**: Regular performance testing

## Validation Criteria
- All acceptance criteria met
- Performance benchmarks achieved
- Cross-browser compatibility confirmed
- Stakeholder approval received
```

---

*This document serves as the comprehensive guide for AI IDE project documentation. Keep it updated as processes evolve and improve.*