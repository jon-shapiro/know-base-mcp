# Repository Separation Plan - Three System Architecture

**Plan ID**: P001  
**Created**: August 06, 2025  
**Status**: DRAFT  
**Implementation**: Plan C - Structured Separation  

## 🎯 STRATEGIC OVERVIEW

### Architecture Vision
Transform current know-base-mcp into three distinct, focused systems that enable reusable PM capabilities, multi-industry guide generation, and clean content deployment.

### Business Benefits
- **Reusable PM System**: know-docs becomes generic project management tool for any software project
- **Multi-Industry Generator**: know-base-mcp supports cannabis → stereo → other industry knowledge bases
- **Clean Deployment**: jmp-content provides runtime-ready content for website integration
- **Separation of Concerns**: Clear boundaries prevent confusion between PM and project files

---

## 🗂️ THREE SYSTEM ARCHITECTURE

### **System 1: know-docs** (Reusable PM System)
```
know-docs/ (Replaces existing repository)
├── README.md                     # PM system overview & usage
├── pm/
│   ├── templates/               # Epic/Story/Task/Analysis/Plan templates
│   ├── registry/                # Work tracking and active work dashboard
│   └── examples/                # Working PM examples from know-base-mcp
├── docs/
│   ├── processes/               # PM processes and workflows
│   ├── integration/             # AI session integration guide
│   └── usage/                   # How to use PM system in projects
└── tools/
    ├── cleanup/                 # File cleanup and maintenance tools
    └── migration/               # Database migration preparation tools
```

**Extraction Strategy**: Copy PM system from know-base-mcp, enhance for generic reuse
**Timeline**: Extract after T001/T009 complete (Phase 2)

### **System 2: know-base-mcp** (Product-Specific Guide Generator)
```
know-base-mcp/ (Current repo, cleaned)
├── README.md                     # Cannabis guide generator for JMP
├── mcp-server/                   # MCP server implementation
├── components/                   # Component creation/conversion tools
├── cannabis/
│   ├── jmp/                     # JMP-specific patterns, branding, terminology
│   ├── compliance/              # Design compliance patterns (not regulatory)
│   └── context/                 # Cannabis industry context and examples
├── conversion/
│   ├── liquid-to-components/    # Existing liquid → modular conversion
│   └── ascii-to-liquid/         # ASCII mockups → liquid components
├── docs/
│   ├── design/                  # MCP construct design
│   ├── requirements/            # Process testing requirements
│   └── validation/              # Process testing results
└── pm-reference/                # Link to know-docs PM system (not local PM)
```

**Evolution Strategy**: Remove PM files, add industry knowledge architecture
**Timeline**: Clean after PM extraction (Phase 3)

### **System 3: jmp-content** (Runtime Content Output)
```
jmp-content/ (New repository)
├── README.md                     # Integration guide for any landing page
├── src/                          # PRODUCTION: Runtime-ready content (like know-docs/docs-copy/src)
│   ├── guides/                  # Generated guide content (11ty + liquid)
│   ├── _includes/               # Liquid component library
│   ├── _layouts/                # Page layout templates
│   └── assets/                  # Framework-agnostic CSS/JS (no Tailwind dependencies)
├── demo/                         # DEMO: Standalone demonstration files
│   ├── index.html               # Demo landing page
│   ├── demo-styles/             # Demo-specific CSS/styling
│   ├── demo-nav/                # Demo navigation and layout
│   └── demo-assets/             # Demo images and branding
├── integration/
│   ├── examples/                # Integration examples for different frameworks
│   ├── migration/               # Tools for rebasing into other landing pages
│   ├── demo-removal/            # Scripts to remove demo files for production
│   └── compatibility/           # Framework compatibility guides
└── archive/                     # Previous versions and rollback
```

**Creation Strategy**: Output destination for know-base-mcp generator
**Timeline**: Create when first content generation ready (Phase 3+)

---

## 📅 IMPLEMENTATION TIMELINE

### **Phase 1: Foundation Planning** (August 6-7, 2025)
**Current Work Continues** with separation awareness:
- Complete T009: File Inventory Review with separation context
- Approve T001: PM Requirements Analysis 
- Create detailed migration plans for each system
- Update file organization to support clean extraction

**Deliverables**:
- Repository separation plan (this document)
- Updated file cleanup process including decisions lifecycle
- Enhanced strategic initiation with decisions review
- T009 completion with separation-aware file annotations

### **Phase 2: PM System Extraction** (August 8-10, 2025)
**Extract and Enhance PM System**:
- Create new know-docs repository (replace existing)
- Copy PM system from know-base-mcp with generic enhancements
- Create PM system documentation and usage guides
- Test PM system independence with example project
- Update know-base-mcp to reference external PM system

**Deliverables**:
- Fully functional know-docs PM system repository
- PM system extraction documentation
- Updated know-base-mcp with PM references
- PM system reuse documentation

### **Phase 3: Cannabis Project Focus** (August 11-15, 2025)
**Clean and Focus Cannabis Generator**:
- Remove PM files from know-base-mcp (keeping reference links)
- Organize cannabis-specific content and patterns
- Design multi-industry knowledge base architecture
- Plan jmp-content output repository structure
- Begin MCP server design with clean focus

**Deliverables**:
- Clean know-base-mcp focused on guide generation
- Multi-industry architecture design
- jmp-content repository plan
- MCP server design foundation

### **Phase 4: Multi-Industry Implementation** (August 16+, 2025)
**Build Multi-Industry Capabilities**:
- Implement cannabis industry knowledge base
- Create industry template framework for future expansion
- Build jmp-content output system
- Test with cannabis → stereo expansion scenario

---

## 🔧 DECISIONS FILE LIFECYCLE INTEGRATION

### **Update File Cleanup Process**
Add to existing `COMMANDS.md --cleanup` command:
```markdown
### Decisions Review & Cleanup
- Review all decisions in docs/decisions/
- Mark outdated decisions as SUPERSEDED
- Archive decisions older than 6 months  
- Update docs/decisions/decisions-index.md with active decisions only
```

### **Update Strategic Initiation Process**
Add to `STRATEGIC-INITIATION-SYSTEM.md` Phase 2:
```markdown
### Step 2C: Active Decisions Review
**File**: docs/decisions/decisions-index.md (active decisions only)
**Strategic Validation Required**: 
After loading, demonstrate understanding of strategic decisions affecting current work
```

---

## 🎯 IMMEDIATE EXECUTION PLAN

### **Step 1: Update Process Files** (Next 30 minutes)
1. Update file cleanup process to include decisions lifecycle
2. Update strategic initiation to include decisions review  
3. Create decisions index template
4. Document process updates

### **Step 2: Begin T009** (Today)
1. Start file inventory review with separation context
2. Annotate files with system assignment (PM vs. Cannabis vs. Output)
3. Identify extraction/migration requirements
4. Plan missing files for each system

### **Step 3: Approve & Execute** (This week)
1. Review and approve this separation plan
2. Complete Phase 1 foundation work
3. Prepare for PM system extraction
4. Begin Phase 2 implementation

---

## ❓ APPROVAL QUESTIONS

1. **Timeline**: Does the 4-phase timeline work for your schedule?
2. **System Names**: Approve know-docs, know-base-mcp, jmp-content naming?
3. **PM System Scope**: Generic reusable vs. documentation-project-focused?
4. **Multi-Industry Priority**: Cannabis → stereo → others expansion plan priority?
5. **Implementation Approach**: Any concerns about structured separation approach?

---

**Status**: AWAITING APPROVAL  
**Next Action**: Your approval to proceed with process updates and T009 execution  
**Implementation**: Ready to begin immediately upon approval
