# Vibe Coding Instructions - AI-Optimized TDD Framework

**Version**: 2.0  
**Framework**: Kent Beck TDD + AI-Optimized Development  
**Compatible**: Cursor, Windsurf, VS Code + AI Extensions

## Credits & Methodology

This framework integrates **Kent Beck's Test-Driven Development (TDD)** and **Tidy First** methodologies with AI-optimized development practices.

**TDD Methodology Credit**: [Kent Beck](https://github.com/KentBeck/BPlusTree3/blob/main/rust/docs/CLAUDE.md) - Original TDD principles and Red-Green-Refactor cycle

**Core Principles Applied**:
- Always follow the TDD cycle: Red → Green → Refactor
- Write the simplest failing test first
- Implement minimum code needed to make tests pass
- Separate structural changes from behavioral changes (Tidy First)
- Maintain high code quality throughout development

## Project Structure Overview
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

## 🚀 Project Initialization (New Team Members)

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

## �💻 Development Phase Prompts

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

## 🤖 AI Integration Commands

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

---

## 📚 Quick Reference Guide

| Phase | Primary Files | Key Commands | Success Criteria |
|-------|---------------|--------------|------------------|
| **Security Setup** | .gitignore, .dockerignore, .env.example | Create ignore files | No sensitive data tracked |
| **Init** | ai-ide-instructions.md, knowledge.md | "Use Context7" | Framework understood |
| **Plan** | plan.md, todo.md | Select next test | Clear roadmap |
| **Design** | designer-guidelines.md | Create component specs | Testable designs |
| **Develop** | programmer-guidelines.md | "go" command | TDD cycle complete |
| **Test** | tester-guidelines.md | Run test suite | All quality gates pass |
| **Deploy** | All docs updated | Validate compliance | Production ready |

---

**🎯 Ready to Start?** Choose your role above and follow the corresponding prompts. Remember: this framework combines Kent Beck's TDD with AI-optimization for maximum development effectiveness.