# Document Consolidation & Target Repository Structure
**Organized target state for know-docs migration before build phase**

**Created**: August 06, 2025  
**Purpose**: Define systematic document organization eliminating overlap and ensuring complete coverage  
**Migration Strategy**: Bulk move using bash script + systematic consolidation

---

## 🎯 **DOCUMENT OVERLAP ANALYSIS**

### **Critical Overlaps Identified**
1. **Vision Documents**: 3 versions across repos need consolidation
2. **Architecture Documents**: 2 versions with different focus areas
3. **Component Specifications**: Scattered across multiple locations
4. **User Scenarios**: Duplicated content in multiple files
5. **PRD Documents**: Multiple versions with different scopes

### **Source Document Mapping**
| Document Type | know-base Location | know-base-mcp Location | Status | Consolidation Strategy |
|---------------|-------------------|----------------------|--------|----------------------|
| **Vision** | /docs/vision/know-base-user-vision.md | None | Complete | Use as foundation |
| **PRD** | /PRD-Know-Base.md | None | Complete | Use as primary |
| **Architecture** | /Architecture-Know-Base.md | None | Complete | Use as technical base |
| **Component Specs** | /docs/components/ (17/30) | /foundation-docs/components/ | Partial | Merge and complete |
| **User Scenarios** | /docs/user-scenarios/ | /foundation-docs/user-scenarios/ | Overlap | Consolidate workflows |
| **Getting Started Mockup** | /docs/reference/getting-started-mockup-complete.md | None | Complete | Reference standard |

---

## 📁 **TARGET REPOSITORY STRUCTURE (know-docs)**

### **Complete Directory Structure**
```
know-docs/
├── README.md                           # Master project overview with registry links
├── docs/
│   ├── vision/                         # Strategic vision and scope
│   │   ├── know-base-jmp-vision.md     # [MERGE] User vision + JMP specifics
│   │   ├── mvp-scope-definition.md     # [CREATE] Clear MVP boundaries
│   │   └── product-roadmap.md          # [CREATE] Timeline and phases
│   ├── requirements/                   # Complete requirements documentation
│   │   ├── prd-know-base-jmp.md        # [MERGE] PRD + JMP customization
│   │   ├── use-case-registry.md        # [MIGRATE] From know-base-mcp
│   │   ├── quality-standards.md        # [CREATE] 8+/10 quality criteria
│   │   └── success-metrics.md          # [EXTRACT] From PRD
│   ├── architecture/                   # Technical architecture and design
│   │   ├── system-architecture.md      # [MERGE] Architecture + MCP design
│   │   ├── mcp-server-specs.md         # [CREATE] MCP server architecture
│   │   ├── component-system.md         # [EXTRACT] From architecture
│   │   └── unity-integration.md        # [CREATE] Unity Landing integration
│   ├── components/                     # Complete component library
│   │   ├── component-registry.md       # [MERGE] All component lists
│   │   ├── essential/                  # 8 MVP components
│   │   │   ├── hero-section.md         # [MIGRATE] From know-base
│   │   │   ├── message-box.md          # [MIGRATE] From know-base
│   │   │   ├── section-wrapper.md      # [MIGRATE] From know-base
│   │   │   ├── feature-card.md         # [MIGRATE] From know-base
│   │   │   ├── grid-layout.md          # [MIGRATE] From know-base
│   │   │   ├── three-columns.md        # [MIGRATE] From know-base
│   │   │   ├── section-header.md       # [CREATE] Missing spec
│   │   │   └── help-footer.md          # [CREATE] Missing spec
│   │   ├── enhancement/                # 8 enhancement components
│   │   │   ├── back-to-top.md          # [CREATE] Missing spec
│   │   │   ├── quick-start-wrapper.md  # [CREATE] Missing spec
│   │   │   ├── benefits-section.md     # [CREATE] Missing spec
│   │   │   ├── animated-link.md        # [MIGRATE] From know-base
│   │   │   ├── admin-interface.md      # [CREATE] Missing spec
│   │   │   ├── feature-overview.md     # [CREATE] Missing spec
│   │   │   ├── site-template-sections.md # [CREATE] Missing spec
│   │   │   └── tv-location-sections.md # [CREATE] Missing spec
│   │   └── cannabis/                   # Industry-specific customizations
│   │       ├── compliance-patterns.md  # [CREATE] Cannabis-specific components
│   │       └── industry-terminology.md # [CREATE] Cannabis terminology
│   ├── workflows/                      # User workflows and processes
│   │   ├── content-creation.md         # [MERGE] User flows + day-in-the-life
│   │   ├── knowledge-management.md     # [MERGE] Context + knowledge capture
│   │   ├── quality-assurance.md        # [EXTRACT] From workflows
│   │   ├── deployment.md               # [MERGE] Content promotion + deployment
│   │   └── visual-iteration.md         # [EXTRACT] From user scenarios
│   ├── reference/                      # Standards and examples
│   │   ├── getting-started-mockup.md   # [MIGRATE] ASCII mockup standard
│   │   ├── unity-landing-inventory.md  # [MIGRATE] From know-base-mcp
│   │   ├── component-examples.md       # [CREATE] Component usage examples
│   │   └── cannabis-guidelines.md      # [CREATE] Industry-specific guidance
│   └── user-guide/                     # System usage documentation
│       ├── mcp-setup.md                # [CREATE] MCP server setup
│       ├── conversational-workflows.md # [CREATE] How to use system
│       └── troubleshooting.md          # [CREATE] Common issues
├── src/                                # Implementation code
│   ├── mcp-server/                     # MCP server implementation
│   ├── components/                     # Component library implementation
│   ├── templates/                      # Guide and content templates
│   └── assets/                         # CSS, images, cannabis-specific assets
├── examples/                           # Working examples and demos
│   ├── migrations/                     # Example guide conversions
│   ├── new-content/                    # Example new content creation
│   └── workflows/                      # Complete workflow demonstrations
├── tests/                              # Testing framework and validation